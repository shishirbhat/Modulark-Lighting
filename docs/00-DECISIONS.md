# Decision log

Status values: LOCKED (do not revisit), OPEN (needs a ruling), DEFERRED.

## LOCKED

| # | Decision | Rationale |
|---|---|---|
| D1 | **Enclosures are CNC-machined aluminium, anodised.** No injection tooling, no 3D-printed production parts. | Cost-competitive with printing at low volume, cheaper above ~500 units, passes flammability by being metal, and reads as premium. Removes the single biggest compliance blocker. |
| D2 | **3D printing is prototyping only.** | An FDM part cannot carry material certificates or batch traceability, so it cannot survive BIS surveillance. |
| D3 | **The Pack has no USB host output.** | Renaming a power bank does not change its classification; removing the output port does. Kills IS 13252 exposure at zero cost. |
| D4 | **Cells are bought BIS-registered under IS 16046.** | Avoids ~₹1L and ~3 months of own-registration. |
| D5 | **Mains terminates in a BIS-registered encapsulated AC-DC module.** Interior is SELV DC only. | Standard practice. Confines mains fire risk to a pre-certified sealed component. |
| D6 | **No internal plastic structural frame.** PCB mounts to the aluminium body on metal standoffs. | Leaves no internal insulating part for the glow-wire probe to test. |
| D7 | **Diffusers are bought certified PC** with GWIT/GWFI data. | Diffuser is unavoidably a non-metallic part and must meet 650°C. Inherit the supplier's certification. |
| D8a | **No customer pre-orders or deposits** for any product not yet BIS-registered. Founder is a minor with no capital to refund; an adult director carries the liability. Earlier pre-order guidance is withdrawn. | Legal and financial exposure |
| D8 | **Direct-to-consumer only for v1. No interior-designer channel.** | A 20–25% channel cut does not survive the v1 cost base. Revisit only after volume manufacturing. |
| D9 | **Field modules carry no internal cell. They are Pack-powered.** | Saves ~₹330/Field, removes a second battery SKU to certify, and fixes the Field:Pack count mismatch. Kit is now 3 Field + 3 Pack. |
| D10 | **Kit price is ₹29,999.** | ₹17,999 was below cost after tax. ₹24,999 breaks even above a realistic solo build ceiling. ₹29,999 breaks even at ~20 kits/month against a ~28–45 kit ceiling. See `04-UNIT-ECONOMICS.md`. |
| D11 | **Industrial and brand design is done in-house by the founder at ₹0 cash cost.** | Founder decision. Note: product photography is NOT in this exclusion and is budgeted — it is where a premium claim is won or lost. |
| D12 | **v1 is three SKUs: Core, Field, Pack.** | Smallest shippable system. Halves the compliance bill versus four SKUs. |

## OPEN STRATEGIC DECISION

| # | Decision | Status |
|---|---|---|
| S1 | **"Brain first"** — ship the Core alone as a local controller for third-party Matter/Zigbee bulbs, deferring the Field module. Cuts capital to first sale from ~₹15.2L to ~₹2L and compliance from 90+ days to 2–6 weeks, **if** the Core is ruled outside CRS. Trades away complete-system positioning and CRI control. | **Awaiting founder decision.** Depends on O2/A2 |

## DEFERRED

| Item | Why deferred |
|---|---|
| **Switch** (mains light killer) | Highest compliance exposure of any SKU. A mains switch may fall under ISI (Scheme I) rather than CRS, and ISI requires a physical BIS inspection of the manufacturing premises. Do not design this into v1. |
| **Prophesee GenX320 event imager** | Module price ~₹27,000; bare-die unpriced and unavailable at our volume without an NDA we will not get. Cannot exist in a ₹7,999-class product. Use a conventional imager (OV5640 class, ~₹400) for v1. Revisit at v3. |
| Sky (solar daylight sensor) | Not on the revenue path. |
| ₹1,199 CRI-95 batten | Separate BIS model, mass-market price point, different business. |
| Spine (powered wall ribbon) | v2. |
| Halo (DMD beam-steering luminaire) | v3, not expected to be profitable. |

## OPEN — needs a ruling before capital is committed

| # | Question | Who answers | Why it matters |
|---|---|---|---|
| O1 | Which IS 10322 Part 5 **section** applies to the Field module? `[CONFIRM]` | BIS compliance consultant | Determines the test plan and the lab quote. Field is a wall-mounted, battery-operated, non-emergency luminaire; the section mapping is not obvious from public sources. |
| O2 | Is the **Core** inside CRS scope at all? | BIS compliance consultant | The Core is a sensor/controller/charger dock, not a luminaire. If it is outside CRS and uses an external BIS-certified adapter, it needs only WPC ETA — which removes months from the critical path. |
| O3 | Is the **Pack** covered by the Field's registration as an accessory, or does it need its own? | BIS compliance consultant | Decides whether we carry one registration or two. |
| O4 | GST: is the kit a **composite supply** (5% if the luminaire is the principal supply) or a **mixed supply** (18% on the whole value)? And the correct HSN. | Chartered accountant, in writing | Swings contribution by ~₹3,100 per kit. |
| O5 | Is 24–24.25 GHz confirmed delicensed in India for the LD2410 mmWave sensor? `[CONFIRM]` | WPC consultant | If not, the presence sensor must change. |

**O1–O5 together cost roughly ₹65,000 in professional fees. They are the
cheapest money in the entire plan. Spend it before any tooling, inventory
or lab booking.**
