# Rejected ideas — do not relitigate without new information

Distinct from the DEFERRED table in `00-DECISIONS.md`. Deferred items are
postponed and expected back. **These are killed.** Each died for a stated
reason, most of them physics rather than preference.

Reopen one only with new information that defeats the reason given — not
because it sounds appealing again.

| Idea | Why it died |
|---|---|
| **Electrochromic film over tubes** | Clear→amber EC film is not a commodity part, and the approach only ever worked on tubes. |
| **The Collar** — socket pass-through adapter | One per fixture, gets unscrewed and lost. A switch-level actuator does the job better. (That actuator is itself now DEFERRED — see `00-DECISIONS.md`.) |
| **Plate as the brain** — sensing built into the wall-switch plate | The switch box is the worst sensing position in a room: behind a door, facing a wall. Sensing and actuation had to be separated, which is why the Core is standalone. |
| **LiFi as room radar** | LiFi is a comms technology and needs receivers. Room-scale time-of-flight needs sub-nanosecond timing; phosphor-converted LEDs are orders of magnitude too slow. The literature on LiFi sensing requires *dense* photodetector arrays — more hardware, not less. |
| **Photomemristor "sentient glass"** | An integrated DVS-memristor device is an open research problem, not a component that can be bought. |
| **Metamaterial white-light beamforming** | Metasurfaces are dispersive: white light gives rainbows, not a clean spot. The working route to beam steering is DMD, which is why Halo is deferred to v3 rather than rejected. |
| **Phone-flicker doomscroll detection** | Phone PWM ranges roughly 240–3840 Hz and many panels are flicker-free, so flicker is not a reliable signal. If this is ever wanted, the detectable version is a small bright high-CCT patch in an otherwise dark luminance field, plus mmWave posture. |
| **"Forces you to sleep" framing** | A light that fights its owner gets returned. Melatonin and sleep claims are also regulated territory — see `research_notes/.../dpdp_and_claims.md` before any health-adjacent marketing copy. |
| **Schools as a market** | Ruled out explicitly by the founder. Modulus remains the cash engine; nothing in this division points at that market. |

## Working notes

Two process rules earned during the design sessions. Both are cheap to
follow and expensive to skip.

1. **Check what a source actually says, not that one exists.** Several
   AI-generated concepts arrived with citations that did not support the
   claim attached to them. This is the reason for the `[CONFIRM]` tag
   convention in this repo.
2. **Market figures go stale and are directional.** Anything load-bearing
   gets re-checked against a primary source before money moves.
