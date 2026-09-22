# Manufacturing method

## Summary

| Stage | Method | Who |
|---|---|---|
| Enclosures | CNC machining, aluminium, anodised | Indian job shop, no tooling |
| PCBs + PCBA | Overseas turnkey (JLCPCB / PCBWay class) | Vendor |
| Specialty parts (CRI 95 LEDs) | Self-sourced — not in vendor libraries | Founder |
| Final assembly, test, calibration, pack | By hand | Founder |

## Why CNC aluminium beats both alternatives at our volume

| Field enclosure | @100 units | @1,000 units | Tooling | Glow-wire |
|---|---|---|---|---|
| 3D printed ASA | ₹501 | ₹501 | ₹0 | **Fails** |
| **CNC aluminium** | **₹750** | **₹350–500** | **₹0** | **Passes (metal)** |
| Injection moulded | — | ₹110 | ₹10L | Passes |

At 100 units CNC costs ~₹250 more per Field than printing. That premium
buys: a certifiable product, a premium finish, and — critically — the
elimination of print-farm labour. Above ~500 units CNC is also cheaper
outright.

## The hidden win: outsourcing the enclosure buys back founder time

| | 3D printed in-house | CNC outsourced |
|---|---|---|
| Print + post-process time per kit | ~2.5 hrs | **0** |
| Hand assembly + test per kit | ~3.5 hrs | ~3.5 hrs |
| **Founder hours per kit** | **~6.0** | **~3.5** |
| Print-hours per kit | 38 | 0 |
| Printers needed at 50 kits/mo | 4 (~₹4.2L capex) | 0 |
| **Realistic solo ceiling** | **~25 kits/mo** | **~28–45 kits/mo** |

This is the decision that makes the business viable. It is not primarily a
cost move — it removes the binding time constraint and the compliance
blocker at the same time.

## Enclosure sourcing

- Use a local CNC job shop; no tooling commitment, no MOQ beyond setup.
- Expect a per-part setup/programming charge on the first order; it
  amortises away on repeats. Negotiate a held program.
- Anodising is a separate vendor step — batch it.
- Order enclosures in multiples matched to PCBA batches to avoid holding
  aluminium you cannot populate.

## PCBA notes

Vendor pricing at qty 100 is roughly: setup ~$7, stencil ~$1.50, ~$3 per
unique extended component, plus ~$0.0015 per solder joint. Fixed costs
amortise fast, so **order in batches of 100+, not 20**. Panelise above 50.

**CRI 95 LEDs will not be in the vendor's parts library.** Plan on either
self-sourcing plus consignment (awkward with most vendors) or hand-placing
the LED board. Cost this honestly — it is real assembly time.

Import the boards populated, but note BCD + SWS applies (see
`02-COMPLIANCE.md` section 5).

## Assembly rules

1. PCB fastens to the aluminium body with **metal standoffs**. Never to a
   plastic boss.
2. Maintain the designed clearance between electronics and any non-metallic
   part. Document it — it is a compliance argument.
3. Per-unit colour calibration against a reference sensor before close-up.
4. Flash and functionally test every unit before packing. A returned unit
   costs more than the test.
