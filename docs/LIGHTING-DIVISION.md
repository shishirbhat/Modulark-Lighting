# Modulark Lighting — context and conclusions

Everything decided in the session of 2026-09-14 → 09-21, written so a new
session (or a person) can pick this up cold without re-deriving it. Nothing
here is built yet. The live, editable version of the technical spec is at
https://claude.ai/code/artifact/c935bc64-a33e-4eef-be50-956525eed225

---

## Where this sits

**Modulark Tech Labs Pvt Ltd** has three intended arms:

| Arm | What | State |
|---|---|---|
| **Modulus** | School management platform (separate repository) | Built, unmonetised — live Razorpay still unverified |
| **Modulark Aero** | Drones | Intended, nothing built |
| **Lighting** (this doc) | Room-level ambient lighting system | Design only |

A division is not a legal entity — it costs nothing to create, needs only an
MOA object clause that covers it. Modulus is the cash engine; see
`docs/EXPANSION.md` for how that is meant to pay for the rest.

**Sequencing that was agreed and should not be quietly dropped:** Modulus must
verify a live payment and adopt per-pupil pricing before this division spends
real money. A hardware line funded by a product that cannot yet take money is
funded by savings.

---

## The core insight

> Every lighting company controls lights. Nobody controls the room.

A smart bulb is **open loop** — told to go to 40% at 2700K, with no idea what
the room looks like afterwards. It does not know the sun is still out, the TV
is on, or someone opened a curtain.

This system is **closed loop**. A sensing node measures the actual light in the
room — level and colour — and commands whatever sources exist to reach a target
state:

> *Living room, evening: 120 lux, 2700K, on the walls rather than the ceiling.*

Three consequences that matter commercially:

1. It improves with data — every room teaches it what targets people keep.
2. Once it speaks Matter it can solve a room containing **other brands' lights**,
   which makes it a layer over the category rather than another product in it.
3. No app, no account, no internet. Setup and flakiness are what kill smart
   lighting in Indian homes.

Positioning line: **everyone else sells you lights, we sell you the room.**

---

## Product line-up

Names are placeholders.

| Product | What it is | Power | Ships |
|---|---|---|---|
| **Core** | The dock: brain, room sensors, the dial, charges 3–4 packs | Mains | v1 |
| **Field module** | The light itself | Powered mount or swap pack | v1 |
| **Pack** | Swappable battery; doubles as a phone power bank | — | v1 |
| **Switch** | Breaks the existing overhead circuit (clip-on plate or inline relay) | Mains | v1 |
| **Sky** | Window disc measuring daylight before it reaches the room | Solar | v1 add-on |
| **Affordable tier** | Standalone CRI-95 tunable batten, curve baked in, no system | Mains | v1.5 |
| **Spine** | Low-voltage ribbon; modules anywhere along a wall | One plug per room | v2, pro |
| **Halo** | Beam-steering hero luminaire (DMD) | Mains | v3, fame product |

**Four SKUs ship v1.**

### Pricing (working estimates, ~5k units, ex-tax — need real quotes)

| Product | BOM | Price | GM |
|---|---|---|---|
| Core | ₹2,200–3,500 | ₹7,999 | 56–72% |
| Field module | ₹550–700 | ₹2,499 | 72–78% |
| Pack | ₹350–500 | ₹1,299 | 62–73% |
| Switch (plate) | ₹400–600 | ₹1,999 | 70–80% |
| Switch (inline relay) | ₹200–300 | ₹1,299 | 77–85% |
| Sky | ₹400–600 | ₹1,499 | 60–73% |
| Affordable batten | ₹400–550 | ₹1,199 | 55–65% |
| Spine, 2m | ₹600–900 | ₹1,999 | 55–70% |

**Starter kit: Core + 3 Field + 2 Packs + 1 Switch = ₹17,999.** Separately
₹20,093. Kit BOM ~₹6,200 → ~65% GM.

Channel: D2C ~65% net · designer specification (20–25% cut) ~45–48% ·
retail (30–40% cut) ~30–38%. **Designer specification goes first** — best
margin and the credibility channel.

Pricing rules: anchor against the room not the bulb · never discount the Core
(it is the lock-in) · packs and modules are the repeat line.

---

## Architecture

### Field module — three-layer cylinder

Wall disc (magnet + optional power) → swap pack (battery) → light head
(LEDs, driver, radio, touch).

**Pack-to-head power is concentric ring contacts, not USB.** Inner pad plus
outer ring, pogo pins on gold pads. Rotationally symmetric so it mates at any
angle with no alignment; self-wiping so contacts survive; magnets align and
retain but never conduct. Power only — state of charge is read by voltage and
coulomb counting. **The pack must be electronically dead until mated** (hall
sensor or handshake) or a loose pack is a short-circuit hazard.

**Swap ergonomics:** twist the whole cylinder off the disc, split the halves in
your hand, twist back. Never make people unstack it on the wall.

**Light head:** dual channel 2200K + 4000K, both CRI 95, mixed by ratio.
Diffuse wall-wash optics — never a visible bright point. 1–3W. Touch top for
on/off/warmth, works with the Core dead.

### Core — sensing and the solver

| Sensor | Part | Answers |
|---|---|---|
| Spectral, 11-ch | AS7341 | What colour is the light? (RGB sensors are fooled by LED spectra) |
| Lux | VEML7700 | How much, across wide dynamic range |
| Low-res imager | OV-series, downsampled to ~32×32 on-device | Where is the light landing |
| Presence | LD2410 mmWave | Anyone here? (PIR misses a still reader) |

**Sensor decision pending:** an event-based sensor (Prophesee GenX320, 3×4mm,
edge-AI) reports only changes, ~1000× less data, and *never produces a frame*
— turning the privacy claim from a promise into a physical fact. Blocker is
cost, likely 10–50× the imager. Core only, never a module. Photomemristors are
a research frontier, not a component — not on the table.

**Calibration sweep:** at install, turn each source on alone for a couple of
seconds and record its effect. That builds a per-room **light transport
matrix** — the core IP, small enough for a microcontroller. It also sharpens
itself during ordinary use.

**The solver:** minimise ‖Mw + d − t‖² subject to 0 ≤ wᵢ ≤ 1, where M is the
transport matrix, w the per-source levels, d measured daylight, t the target.
Small constrained least squares, milliseconds. Daylight enters as a measured
uncontrollable input, which is why no schedules are ever needed.

Extra constraints ride the same solve: battery charge per source, preferred
light placement, a penalty on using many sources at low level.

**The dial selects a target state** (Read / Relax / Cook / Guests), not a
brightness.

### Radio

v1 **ESP-NOW or BLE Mesh** on ESP32-C3 (~₹120/node) — self-forming, no router,
no pairing, no cloud. v2 **Thread/Matter** — strategically the point, because
Matter is how the Core controls other companies' lights. Latency is a
non-requirement: good transitions take 20–30s. Power-line comms rejected
(inverter/UPS loads, and battery modules cannot use it).

### Power and charging

Energy math that drives everything: 3W for 4h = 12 Wh/day; a 21700 holds
~18.5 Wh. So 1.5 days at wall-wash output. **Pure-battery lighting used nightly
loses to physics.**

Four rules:

1. **The mount is the charger.** Wall disc carries contacts; a USB-C lead makes
   that module permanent. Same module, two modes.
2. **Nothing goes where a ladder is needed.** Field is a low/mid-level layer.
   The ceiling belongs to the Switch. This is also correct lighting design.
3. **Swap the battery, don't transfer charge.** Moving 18 Wh at 10W takes ~2
   hours; a swap takes 2 seconds. Dock charges 3–4 packs overnight.
4. **Charge is a solver constraint.** A pack at 15% is dropped and the target is
   met another way. Depletion is staggered so one pack asks for attention every
   few days, not five on the same evening.

One amber dot on the Core when a round is due, ~weekly. Sixty seconds, like
watering plants.

### Overhead light control

Must be switchable off — you cannot out-shout a 6500K tube with 2W of warm
light.

**The Plate (clip-on actuator faceplate) was split in two**, because the switch
is usually the worst spot in the room for sensing (behind a door, facing a
wall). So: Core is standalone and placed where it can see; Switch is a dumb
actuator. Two forms — clip-on plate (no electrician, renter-friendly, clicks,
per-brand fitment) or inline relay (electrician once, silent, invisible).

**Put the relay at the fixture, not the switch box** — Indian switch boxes
commonly break live only with no neutral available, and no-neutral relays make
LED fittings flicker.

The wall switch must always keep working as a plain switch.

---

## Learning the household

Goal: if they dim on grey afternoons for a week, the next grey afternoon is
already dim.

**Keep two models apart.** Physics (the transport matrix — objective, changes
only with furniture or paint) and preference (which target they want given
context — subjective, drifts). Mixing them means a repaint corrupts their
taste.

**Context vector:** time of day (cyclic), weekday/weekend, outdoor level and
colour from Sky, day length (season for free), presence/posture, room.

**Sky makes weather a measured fact, not a forecast.** Overcast = low level,
high CCT. Clear = the opposite. No weather API, no internet, no location — it
just recognises a light signature it has seen before.

**The only learning signal is an override.** Every dial turn is a labelled
example. No app, no preferences screen, no training mode.

**Algorithm is deliberately small** — nearest-neighbour weighting over the
context vector, or context bins with running averages. A household produces a
few overrides a day; a neural net would overfit badly. Runs on the MCU, never
leaves the house.

1. **Confidence gating** — act only after 3+ consistent observations.
2. **Recency decay** — ~8-week half-life so habits can change.
3. **Back off on disagreement** — if a context's overrides are bimodal (two
   people want different things), hold the default and stop learning that slot.

Do not identify individuals. Costs hardware and trust; time of day is a good
enough proxy.

**Visible and reversible:** one line — *dimmer on grey afternoons — learned* —
and a hold-the-dial gesture meaning **forget that**.

---

## The affordable tier

Market reality (checked Sept 2026):

| Product | Price | What |
|---|---|---|
| Commodity batten | ₹400–800 | Fixed 6500K, CRI ~70–80 |
| Wipro Next smart CCT batten | ₹2,480 | Tunable, Wi-Fi, needs app |
| Wipro CCT+RGB | ₹2,690 | As above plus colour |
| Philips Hue starter + bridge | ₹5,049–6,250 | Bridge, app, account |

**None of them competes on CRI** — high-CRI binning costs lumens per watt and
their BOM will not carry it. That is the gap.

Product: one CRI-95 tunable batten/bulb, ambient sensor, curve in firmware, no
Core/pack/dock/app/account. ₹1,199 — **half Wipro's price, better light,
nothing to set up.**

- **Never cut CRI 95.** Strip everything else. A cheap tier that renders colour
  badly is just another batten.
- **Include the radio anyway** (~₹120) so every unit is a future Core customer —
  land and expand. Cost is WPC/ETA certification alongside BIS.
- **Launch premium first.** Lead with ₹1,199 and the brand is defined as cheap,
  making the ₹17,999 kit unsellable later.
- For a tight budget the pitch is **the electricity bill**, not ambience.

---

## Rejected, with reasons — do not relitigate without new information

| Idea | Why it died |
|---|---|
| Electrochromic film over tubes | Clear→amber EC film is not a commodity; only works on tubes anyway |
| The Collar (socket pass-through adapter) | One per fixture, gets unscrewed and lost; the Switch does the job better |
| Plate as the brain | Switch location is the worst sensing spot in the room |
| LiFi as room radar | LiFi is comms and needs receivers. Room-scale ToF needs sub-ns timing; phosphor LEDs are orders of magnitude too slow. Research says LiFi sensing needs *dense* photodetectors — more hardware, not less |
| Photomemristor "sentient glass" | Integrated DVS-memristor is the field's open challenge. Not a component |
| Metamaterial white-light beamforming | Metasurfaces are dispersive — white light gives rainbows, not a spot. The working route is DMD (automotive HD-LED), parked as v3 |
| Phone-flicker doomscroll detection | Phone PWM ranges ~240–3840Hz, many are flicker-free. Use instead: a small bright high-CCT patch in a dark luminance field + mmWave posture |
| "Forces you to sleep" framing | A light that fights its owner gets returned. And melatonin claims are regulated territory |
| Schools as a market for anything new | User ruled it out explicitly. Modulus continues as the cash engine; nothing new points at that market |

---

## Open questions — resolve before tooling or certification spend

1. Can a cheap sensor infer room *appearance*? It measures light arriving at
   itself. Placement and calibration is the hardest unsolved piece.
2. How many mate cycles do the ring contacts survive?
3. What does a user-swappable lithium pack require to certify?
4. Is the calibration sweep tolerable to sit through, or does it read as broken?
5. Power cut and restore — daily in India. Must come back sane unaided.
6. Wall repainted dark: does the transport matrix self-correct quietly?
7. BIS and WPC/ETA timelines and cost. Runs in parallel with the pilot, never
   after.
8. GST slab treatment — luminaires and electronics differ.
9. Naming, for everything.

---

## Prototype — under ₹12,000, on your own ceiling

Order: (1) one Field module lit and dimming smoothly — if the light isn't
beautiful nothing else matters; (2) Core sensing trustworthy across a real day;
(3) the calibration sweep with two modules and the solver hitting a target;
(4) a crude relay Switch; (5) **live with it two weeks** — everything wrong
surfaces in week two.

Parts: ESP32-C3 ×4 ₹1,200 · AS7341 ₹500 · VEML7700 ₹150 · LD2410 ₹250 ·
OV2640 ₹400 · CRI95 strip ₹2,000 · dual-channel drivers ₹1,500 · cells +
charge boards ₹1,500 · relay/servo ₹800 · mechanical ₹2,000.

**Kill criterion:** photograph the same room, same camera, same settings —
existing batten vs the system — and show it to someone who doesn't care about
lighting. No reaction means the premium doesn't exist. Stop there.

---

## Working notes for whoever picks this up

- Three times in this session the user found real holes (charging ergonomics,
  the pack mechanism, the ladder problem) and each fix improved the product.
  Argue with them; it works.
- Market figures here came from search in Sept 2026 and are directional.
  Re-check anything load-bearing before committing money.
- Several AI-generated concepts arrived with citations that did not support the
  claim attached to them. Check what a source actually says, not that one
  exists.
