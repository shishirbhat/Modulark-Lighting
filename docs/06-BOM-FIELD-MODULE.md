# Bill of materials — Field module, 1 unit

Authoritative source for **component-level** costs. Rolled-up product and
kit costs live in `04-UNIT-ECONOMICS.md`.

Quantities and prices are for a **100-unit build**. All prices are
`[ESTIMATE]` until validated against a real quote — treat this as a
procurement worklist, not a costed BOM. At prototype quantities (1–10)
expect **1.5–2× these unit prices**.

Configuration: SELV only, Pack-powered, no mains, no internal cell,
CNC aluminium enclosure, dual-channel tunable CRI 95.

## Compute and radio

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 1 | ESP32-C3-MINI-1-N4 module | 1 | ₹180 | ₹180 | LCSC or Mouser India (landed). Indian resellers quote ₹195–330 — see note A |

## LED subsystem — the differentiator, do not value-engineer

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 2 | CRI 95+ LED, warm ~2700K, 2835 or 3030 | 10 | ₹14 | ₹140 | YUJILEDS store (CRI 95+ 2835L/3030 G03/G04), or Nichia 757 series via authorised distributor |
| 3 | CRI 95+ LED, cool ~5000K, 2835 or 3030 | 10 | ₹14 | ₹140 | Same supplier and bin family as #2 |

## LED driver — dual channel, boost constant-current

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 4 | Boost CC driver IC (AL8862 / MP3428 / TPS61165 class) | 2 | ₹65 | ₹130 | LCSC, Mouser India, Digi-Key India |
| 5 | Power inductor | 2 | ₹18 | ₹36 | LCSC |
| 6 | Schottky diodes, current-sense resistors, driver caps | 1 set | ₹40 | ₹40 | LCSC |

## Power path

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 7 | 3.3 V buck or LDO regulator | 1 | ₹35 | ₹35 | LCSC |
| 8 | Reverse-polarity protection / eFuse | 1 | ₹40 | ₹40 | LCSC |
| 9 | Bulk and decoupling caps, passives (~40 parts) | 1 set | ₹60 | ₹60 | LCSC |

## Pack interface

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 10 | Pogo pin / spring contact | 4 | ₹25 | ₹100 | Mill-Max via Digi-Key for quality; IndiaMART for generic |
| 11 | N52 neodymium magnet | 4 | ₹20 | ₹80 | IndiaMART / local magnet suppliers |

## Optical

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 12 | PC diffuser disc, **must carry GWIT/GWFI material data** | 1 | ₹130 | ₹130 | Indian PC/acrylic fabricator, or a luminaire component supplier. See note B |

## PCB

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 13 | Main control PCB, FR4, 2-layer | 1 | ₹55 | ₹55 | JLCPCB / PCBWay |
| 14 | LED board, **aluminium-core MCPCB** (thermal) | 1 | ₹85 | ₹85 | JLCPCB aluminium PCB service |

## Thermal and fasteners

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 15 | Thermal interface pad, MCPCB to body | 1 | ₹18 | ₹18 | Local / Robu |
| 16 | M2.5 stainless screws + **metal standoffs** (rule 2, `CLAUDE.md`) | 1 set | ₹45 | ₹45 | Local fastener supplier |

## Enclosure

| # | Item | Qty | Unit | Ext | Source |
|---|---|---|---|---|---|
| 17 | CNC aluminium body ring, anodised | 1 | ₹480 | ₹480 | Local CNC job shop; anodising is a separate batched step |
| 18 | CNC aluminium back plate, anodised | 1 | ₹270 | ₹270 | Same |

**Parts subtotal: ₹2,064**

## Services, duty and labour

| # | Item | Cost | Note |
|---|---|---|---|
| 19 | PCBA assembly, 2 boards, amortised setup + joints | ₹130 | Order in batches of 100+, panelise above 50 |
| 20 | Inbound freight share | ₹60 | |
| 21 | BCD + SWS on imported PCBA | ₹198 | Not recoverable. IGST is recoverable, BCD/SWS is not |
| 22 | Assembly, test, flash, colour calibration (40 min @ ₹170/hr) | ₹115 | |
| 23 | Retail packaging share | ₹150 | 300-unit MOQ |

## **Total, 1 Field module @ 100-unit build: ₹2,717**

This is **₹294 above the ₹2,423 modelled in `04-UNIT-ECONOMICS.md`**,
mainly because the ESP32-C3 was underpriced at ₹150. Economics doc updated.

---

## Note A — ESP32-C3 pricing reality

Indian resellers (Robocraze ₹249, DNA Tech ₹331, Digi-Key India ₹323,
IndiaMART ~₹195) are well above the ~₹150 originally modelled. LCSC direct
lands nearer ₹160–180 after duty at volume. **Get a quote before
finalising.** Robocraze advertises up to 30% bulk discount.

## Note B — the diffuser is the only plastic in the product

It is the sole non-metallic part in the fire-risk path and it **will** face
the 650°C glow-wire test (`02-COMPLIANCE.md` §2). Requirements:

- Polycarbonate, not acrylic — acrylic will not pass
- Supplier must provide **GWIT/GWFI material data on file**, in writing
- Never 3D printed (`CLAUDE.md` rule 3 and 4)

Qualify this supplier early. A diffuser without material data blocks
certification regardless of how good the rest of the build is.

## Note C — LED procurement is a working-capital item, and a trap

YUJILEDS CRI 95+ parts ship on **4,000–5,000 pc reels**. One reel of each
colour covers roughly 400–500 modules — several batches. That is ~₹50–70k
tied up early, but it buys reel pricing and, critically, **a single
consistent bin**.

**Do not buy unbranded "CRI 95" LEDs from marketplace sellers.** Two
reasons: the claim is undefendable at certification, and inconsistent
binning destroys closed-loop colour accuracy, which is the entire product
premise. This is not a line to save money on.

## Note D — AS7341 risk does not apply here

The 12–26 week AS7341 lead time affects the **Core**, not the Field module.
Nothing in this BOM has a lead time beyond ~8 weeks.

## Procurement sequence

1. Qualify the **diffuser supplier** and get GWIT/GWFI data in writing — this gates certification
2. Order **one reel each** of warm and cool CRI 95 LEDs — long-lead, single-bin
3. Quote the **CNC job shop**; negotiate a held program to avoid repeat setup charges
4. Everything else is 1–4 week commodity stock
