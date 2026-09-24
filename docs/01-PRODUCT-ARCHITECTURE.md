# v1 product architecture

Three SKUs. Everything else is deferred (`00-DECISIONS.md`).

## Power topology — the rule that shapes everything

```
   Mains 230V AC
        |
        v
  [ BIS-registered encapsulated AC-DC module ]   <-- mains stops here
        |                                             (sealed, pre-certified)
        v
   SELV DC (<= 50V)  ------> Core electronics
        |                    Pack charging bays
        v
   Pack (Li-ion, bought BIS-registered cell)
        |
        v  pogo pins + magnets
   Field module  (SELV DC only, no mains, no internal cell)
```

**No Modulark-made enclosure ever contains mains voltage.** This is what
makes the aluminium-and-certified-diffuser construction sufficient. See
`02-COMPLIANCE.md` section 2.

## Core — sensing brain and dock

| | |
|---|---|
| Role | Senses the room, solves for a target light field, commands Field modules, charges 3 Packs |
| Enclosure | Aluminium extrusion body + CNC-machined end caps, anodised. Extrusion die is ~₹25–60k versus ₹6–10L for injection tooling |
| Power | External **BIS-certified** adapter. Interior SELV DC only |
| MCU | ESP32-S3 (the solver needs more headroom than a C3) |
| Sensors | AS7341 spectral, VEML7700 lux, LD2410 mmWave presence `[CONFIRM O5]`, conventional imager (OV5640 class, ~₹400) |
| Input | Rotary encoder dial with detents |
| Radio | Requires WPC ETA |
| BIS | Scope unresolved — `[CONFIRM O2]`. May be outside CRS entirely |

**Do not specify the Prophesee GenX320.** See `00-DECISIONS.md`, DEFERRED.

## Field module — wall luminaire

| | |
|---|---|
| Role | Circular wall light, CRI 95, dual-channel tunable warm/cool |
| Enclosure | CNC-turned aluminium ring + back plate, anodised |
| Diffuser | **Bought certified PC** with GWIT/GWFI data. Never printed |
| Structure | PCB on **metal standoffs to the aluminium body**. No internal plastic frame |
| Power | **Pack only. No internal cell, no mains** |
| MCU | ESP32-C3 (~₹150 at 100 qty — note ₹120 was optimistic) |
| Radio | Requires WPC ETA |
| BIS | **CRS required.** Critical path. Section `[CONFIRM O1]` |

Per-unit calibration is required if we claim closed-loop colour accuracy —
warm and cool channel LED binning varies. Budget 5–10 min/unit against a
reference sensor.

## Pack — swappable battery

| | |
|---|---|
| Role | Powers a Field module; swaps into the Core to charge |
| Enclosure | CNC aluminium shell |
| Cell | **Bought BIS-registered, IS 16046** |
| Interface | Pogo pins + magnets |
| Output | **No USB host output.** This is load-bearing for compliance — see `00-DECISIONS.md` D3 |
| BIS | Cell only, discharged by purchase. Assembly coverage `[CONFIRM O3]` |

## Kit composition

**Core ×1 + Field ×3 + Pack ×3 — ₹29,999**

Packs match Fields 1:1 because Fields carry no internal cell. The original
3-Field / 2-Pack kit could not power all three modules; this is resolved.

## Supply-chain risk

**The AS7341 is the single point of failure.** Lead times run 12–26 weeks
at our volume, it is allocation-prone, and distributors impose MOQs. At
26-week allocation the entire line stops.

**Action: dual-source it or design a fallback path now, before the first
production order.** Every other part is 1–8 weeks.
