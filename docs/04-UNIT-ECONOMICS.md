# Unit economics — v1, CNC aluminium, direct sales

Single source of truth for cost figures. Do not duplicate elsewhere.
Labour costed at **₹170/hr** (replacement cost of an assembly technician,
~₹28k/month fully loaded), not founder opportunity cost. Founder time is
tracked separately as a capacity constraint in `03-MANUFACTURING.md`.

## Cost build-up

| | Field @100 | Field @500 | Pack @100 | Pack @500 | Core @100 | Core @500 |
|---|---|---|---|---|---|---|
| Electronic parts | 1,050 | 924 | 510 | 447 | 2,600 | 2,280 |
| Certified PC diffuser | 120 | 105 | — | — | — | — |
| CNC aluminium, anodised | 750 | 450 | 350 | 210 | 1,100 | 700 |
| Metal standoffs / fasteners | 40 | 35 | — | — | — | — |
| BCD + SWS on imported PCBA | 198 | 175 | 80 | 70 | 400 | 350 |
| Assembly + test + flash | 115 | 100 | 43 | 38 | 200 | 175 |
| Packaging | 150 | 130 | 60 | 50 | 300 | 260 |
| **COGS** | **2,423** | **1,919** | **1,043** | **815** | **4,600** | **3,765** |

## Kit = Core ×1 + Field ×3 + Pack ×3

| Volume | Kit COGS |
|---|---|
| @100 units | **₹14,998** |
| @500 units | **₹11,967** |

## Price sensitivity — direct sales, no channel cut

Fixed monthly cost assumed **₹2.1 lakh** (founder salary ₹60k, CA and
compliance ₹15k, workspace and power ₹20k, tools ₹10k, marketing ₹30k,
amortised compliance ₹50k). GST treatment is unresolved — see O4.

### At qty 100

| Price | GST case | Net realisation | Contribution | GM | Break-even |
|---|---|---|---|---|---|
| ₹24,999 | 18% mixed | ₹21,186 | ₹6,188 | 29.2% | 34 kits/mo ❌ |
| ₹24,999 | 5% luminaire | ₹23,809 | ₹8,811 | 37.0% | 24 kits/mo ⚠️ |
| **₹29,999** | **18% mixed** | **₹25,423** | **₹10,425** | **41.0%** | **20 kits/mo ✅** |
| **₹29,999** | **5% luminaire** | **₹28,570** | **₹13,572** | **47.5%** | **16 kits/mo ✅** |
| ₹34,999 | 18% mixed | ₹29,660 | ₹14,662 | 49.4% | 14 kits/mo ✅ |

### At qty 500

| Price | GST case | Contribution | GM | Break-even |
|---|---|---|---|---|
| ₹24,999 | 18% mixed | ₹9,219 | 43.5% | 23 kits/mo |
| **₹29,999** | **18% mixed** | **₹13,456** | **52.9%** | **16 kits/mo** |
| ₹29,999 | 5% luminaire | ₹16,603 | 58.1% | 13 kits/mo |

## Why ₹29,999 and not less

- **₹17,999 was below cost after tax.** The original kit at ₹17,999 with
  18% GST and a 25% designer cut lost roughly ₹3,270 per unit. Growth was
  the failure mode.
- **₹24,999 breaks even at 34 kits/month in the worst GST case** — above a
  realistic solo build ceiling. It only works if the 5% rate is confirmed
  and volume reaches 500. Too fragile to launch on.
- **₹29,999 breaks even at 20 kits/month against a ~28–45 kit ceiling** and
  survives the worst GST case. This is the floor price, not an aspiration.

At capacity (~45 kits/month) that is ~₹13.5L/month revenue and roughly
₹2.5L/month operating profit.

## Working capital

| | |
|---|---|
| Component payment | 100% upfront — no supplier terms at our volume |
| Parts landed | Day 45–60 (AS7341 risk: up to 26 weeks) |
| Batch assembled | Day 75–90 |
| Direct-sale collection | **Day 0 with pre-orders** — versus day 190+ through designers |
| Inverted-duty ITC refund lag | 60–120+ days on the 18%-vs-5% spread |

**Direct sales collapse the cash cycle from ~7 months to near zero.**
Taking 50% pre-order deposits funds components before they are bought and
roughly halves the working capital requirement. This is the single largest
cash-flow lever available and it costs nothing.

## Estimates that were wrong in the original plan

| Original | Corrected | Impact |
|---|---|---|
| ESP32-C3 at ₹120 | ₹150–175 at 100 qty | Minor, but the BOM was ~20% light throughout |
| Field module at ₹2,499 | COGS alone is ₹2,423 | Priced below a mass-produced Wipro batten at ₹2,690 |
| Pack at ₹1,299 | COGS ₹1,043 → 14% GM as priced | Unsellable at that margin |
| Kit at ₹17,999 | Needs ₹29,999 | Repriced |
| GenX320 "unpriced" | ~₹27,000/module | Cannot exist in v1 |
| 3-Field / 2-Pack kit | 3 Field / 3 Pack | Original kit could not power all modules |
