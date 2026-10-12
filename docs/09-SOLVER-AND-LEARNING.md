# The solver and the learning model

The firmware layer. `01-PRODUCT-ARCHITECTURE.md` covers the hardware that
runs this; nothing here changes a LOCKED hardware decision.

Everything below runs on the Core's ESP32-S3 and **never leaves the
house** — no app, no account, no cloud inference.

## 1. Why closed loop

A smart bulb is **open loop**: told to go to 40% at 2700 K, with no idea
what the room looks like afterwards. It does not know the sun is still up,
the TV is on, or that someone opened a curtain.

The Core measures the actual light in the room and commands the available
sources to reach a target *room state* — a level and a colour, landing on
the surfaces that should carry it.

**The consequence that matters: daylight enters the maths as a measured
input, not a predicted one.** That is what removes schedules, weather
lookups, location permissions and the internet connection in one move.

## 2. The transport matrix

At install the Core runs a **calibration sweep**: each source is driven
alone for a couple of seconds while the Core records its effect. That
builds a per-room **light transport matrix `M`** — how much each source
contributes to what the Core measures.

`M` is small enough for a microcontroller and sharpens itself during
ordinary use. It is objective physics: it changes when furniture moves or
a wall is repainted, and at no other time.

Open design question: the sweep must be tolerable to sit through. If it
reads as the product being broken on first use, it needs to be
backgrounded or shortened. `[CONFIRM — needs a real user, not an opinion]`

## 3. The solve

Minimise `‖Mw + d − t‖²` subject to `0 ≤ wᵢ ≤ 1`, where

| Term | Meaning |
|---|---|
| `M` | transport matrix, from the calibration sweep |
| `w` | per-source drive levels — what we are solving for |
| `d` | measured daylight and other uncontrolled light |
| `t` | target room state, selected by the dial |

Small constrained least squares. Milliseconds on the S3. Latency is a
non-requirement — a good transition takes 20–30 seconds by design.

**The dial selects a target state, not a brightness.** Read / Relax /
Cook / Guests are points in `t`.

### Extra constraints ride the same solve

- **Pack charge per source.** A Pack at 15% is dropped from the solution
  and the target is met another way.
- **Staggered depletion.** Prefer solutions that spread charge use, so one
  Pack asks for attention every few days rather than three on one evening.
- **Preferred placement**, and a penalty on using many sources at low
  level rather than a few at a sensible level.

### A known v1 limitation

With the Switch deferred (`00-DECISIONS.md`), **v1 cannot turn off an
existing overhead fitting.** A 6500 K tube cannot be out-shouted by a few
watts of warm light, so in rooms where the overhead stays on, `d` includes
a large uncontrollable term and the achievable target set shrinks.

This is a real constraint on the v1 demo, not a bug. Choose demonstration
rooms accordingly, and treat it as an argument for the Switch in v1.5.

## 4. What is being sensed

The Core measures light arriving **at one point** — itself. A room's
appearance is a luminance distribution across surfaces. These are not the
same thing, and the gap is the hardest unsolved piece in the product.

**Design rule: solve in a small perceptual feature space**, not in raw lux
at a point and not in raw pixels. A handful of features — mean wall
luminance, wall-to-ceiling ratio, contrast range, average CCT — is what
`t` and `M` should be expressed in. The imager exists to supply those
features, not to be an image.

Fixing this feature set is a prerequisite for the calibration sweep,
because the sweep records into it. `[CONFIRM — settle before firmware]`

## 5. Learning the household

Goal: if they dim on grey afternoons for a week, the next grey afternoon
is already dim.

### Keep two models apart

| Model | What | Behaviour |
|---|---|---|
| **Physics** | the transport matrix `M` | objective; changes only with furniture or paint |
| **Preference** | which `t` they want in a given context | subjective; drifts over time |

**Never let one contaminate the other.** If a repaint updates the
preference model, the household's taste is corrupted by a painter.

### Context vector

Time of day (cyclic), weekday/weekend, measured outdoor level and colour,
day length (which gives season for free), presence, room.

With Sky deferred (`00-DECISIONS.md`), outdoor conditions come from the
Core's own spectral and lux sensors rather than a window unit. Weather
stays a *measured fact* either way — the system recognises a light
signature it has seen before. No weather API, no location.

### The only learning signal is an override

Every dial turn is a labelled example. There is no app, no preferences
screen and no training mode.

Algorithm is **deliberately small** — nearest-neighbour weighting over the
context vector, or context bins with running averages. A household
produces a few overrides a day; a neural net would overfit badly.

Three guards:

1. **Confidence gating** — act only after 3+ consistent observations.
2. **Recency decay** — roughly an 8-week half-life, so habits can change.
3. **Back off on disagreement** — if a context's overrides are bimodal
   (two people want different things), hold the default and stop learning
   that slot.

### Do not identify individuals

It costs hardware and it costs trust. Time of day is a good enough proxy.
See `research_notes/.../dpdp_and_claims.md` before any feature that would
change this.

### Visible and reversible

One line of explanation — *dimmer on grey afternoons — learned* — and a
hold-the-dial gesture meaning **forget that**. A household that cannot
see or undo what the system learned will not trust it.
