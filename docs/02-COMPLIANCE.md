# Compliance: what needs BIS, what doesn't, and the design rules that follow

All figures dated 2026-09. Anything marked `[CONFIRM]` is not verified
against a primary source — do not act on it as fact.

## 1. The BIS matrix

| SKU | Regime | Standard | Status | Cost | Time |
|---|---|---|---|---|---|
| **Field module** (wall luminaire) | **BIS CRS — required** | IS 10322 Part 5, 2026 series. Section `[CONFIRM O1]` | Mandatory. No exemption available. | ₹50k–1.5L application + ₹25–60k testing | 4–6 wks after testing; **3–4 months realistic** |
| **Core** (dock/controller) | **Unresolved `[CONFIRM O2]`** | IS 13252 / IEC 62368-1 if in scope | Not a luminaire. May be outside CRS entirely if it uses an external certified adapter and is SELV-only. | ₹0 if out of scope; ₹50k–1L if in | 0 or 3–4 months |
| **Pack** (battery, no USB out) | **Cell only** | IS 16046 (cell) | Discharged by buying BIS-registered cells. Pack-as-assembly coverage `[CONFIRM O3]` | ₹0 own-registration | 0 |
| **Mains adapter** | Buy BIS-certified off the shelf | IS 13252 | Never manufacture this. | ₹0 | 0 |
| **All radio SKUs** | **WPC ETA — required** | Self-declaration route | Cheap, fast, lifetime validity per model. | ₹10,000 govt fee/model + ₹30–80k RF test/model | **2–6 weeks** |
| **Switch** (deferred) | Possibly **ISI, not CRS** | IS 3854 / IEC 60669 class | ISI requires a BIS inspection of the factory premises. Deferred out of v1 for this reason. | — | — |

**v1 realistic compliance total: ₹5–7 lakh, 3–4 months, with the Field
module's BIS CRS as the sole critical path.**

### Routes that are NOT available to us

- **Battery-powered exemption — does not exist.** IS 10322:2026 expanded
  scope to all electric light sources and added a normative annexure
  specifically covering battery/EDLC-operated luminaires. Portable
  emergency lights, table lamps and solar LED products are all notified.
- **HSE exemption (<100 units/model/year) — not available.** MeitY
  S.O. 1246(E) requires three-phase supply, OR single-phase above 16 A, OR
  dimensions exceeding 1.5 m × 0.8 m. A wall light meets none of these.
- **Selling before registration — not an option.** Manufacturing, selling,
  distributing or storing-for-sale a notified product without CRS
  registration is an offence under the BIS Act 2016, exposing directors
  personally. Pre-orders are legal; shipping is not.

## 2. Glow-wire: the correct reading of the standard

A misunderstanding was circulating internally and is corrected here.
**Getting this wrong costs a failed test, ~6 weeks and ~₹40k in lab fees.**

IEC 60598-1 / IS 10322 Part 1 tests non-metallic parts in **two tiers**:

| Tier | Scope | Severity |
|---|---|---|
| 1 | Insulating parts **retaining current-carrying parts** in position | 650°C, up to 850°C for certain classes |
| 2 | **All other parts of insulating material** — enclosures, diffusers, decorative parts | **650°C — still tested** |

**An air gap between plastic and live parts moves a part from tier 1 to
tier 2. It does NOT remove the part from testing.** There is no
configuration in which a plastic part inside a luminaire escapes the probe
entirely. Any plan premised on "bypassing the glow-wire test" is wrong.

### What actually works

Do not try to win the test. Remove the plastic from the fire-risk path so
there is nothing contentious to test:

1. **Aluminium enclosure** — glow-wire applies to non-metallic parts only.
   The body is out of scope by material.
2. **Metal standoffs, PCB mounted to the aluminium** — deletes the internal
   plastic structural frame entirely. Nothing internal to test.
3. **Bought certified PC diffuser** — the diffuser is unavoidably tier 2,
   so inherit the supplier's GWIT/GWFI material certification rather than
   generating our own.
4. **BIS-registered encapsulated AC-DC module** — mains-side fire risk is
   sealed inside a pre-certified black box. Interior is SELV DC.

Net result: **no uncertified plastic anywhere in the fire-risk path.** That
is the sentence to put in front of a test engineer. It is accurate, it is
defensible, and it is the same design.

### A note on framing

Items 1–4 are correct engineering and standard industry practice, not
loopholes. Presenting them to a lab or to BIS as a way to dodge a test
invites adversarial scrutiny and, after any field incident, looks like
intent. Describe the design by what it is: mains confined to a certified
module, SELV interior, metal structure, certified diffuser.

## 3. Why a 3D-printed enclosure was abandoned

Independent of cost, printing cannot be certified durably:

- PETG, PLA and ASA all fail the 650°C glow-wire test. FR filaments exist
  at ₹4,000–9,000/kg but print poorly and are barely available in India.
- FDM parts are anisotropic and layer-porous. A lab may pass a submitted
  coupon, but batch-to-batch consistency cannot be demonstrated.
- CRS registration names a factory address subject to surveillance
  sampling. Hobbyist filament carries no material certificates, batch
  numbers or IPQC records — exactly what surveillance asks for.

## 4. GST — unresolved, and material

Public sources conflict. One set reports LED lights moved to **5%** under
the September 2025 GST 2.0 rationalisation; others still show **12%** under
HSN 9405 10 00, which cannot be current since the 12% slab was abolished.
**Treat the rate as unknown until a CA confirms it in writing (O4).**

Two points we are confident about:

- **The kit is likely a mixed supply.** Under CGST s.8(b), bundling goods
  at different rates for a single price attracts **the highest rate on the
  whole value** — 18% on the full ₹29,999. Selling components at their own
  rates instead is worth roughly ₹3,100 per kit. Model both.
- **We will run an inverted duty structure.** We pay 18% IGST on imported
  PCBAs and collect 5% on luminaires. The excess is refundable under CGST
  s.54(3), but refunds take 60–120+ days. **This is a working-capital line,
  not a P&L line.**

## 5. Customs on imported PCBAs

- India's de minimis is **₹0** — every shipment is assessed, including
  prototypes.
- Bare PCBs (HSN 8534) are 0% BCD. **Populated boards are not.**
- Assembled PCBA lands at roughly **10–20% BCD depending on
  classification, plus 10% Social Welfare Surcharge on the BCD**. BCD and
  SWS are real costs. IGST is recoverable as ITC (subject to the refund lag
  above).
- Get the HSN classification ruled before the first production shipment —
  misclassification penalties exceed the duty saved.

## 6. Sequencing

**BIS CRS on the Field module is the only critical path.** Nothing
compresses it below ~90 days. Therefore:

1. Resolve O1–O5 first (~₹65k, ~2 weeks). Cheapest money in the plan.
2. Freeze the Field design and book the lab. This starts the 90-day clock.
3. Run WPC ETA in parallel — 2–6 weeks, does not gate anything.
4. Everything else (firmware, store, photography, packaging) fits inside
   the BIS window at no schedule cost.
5. Take pre-orders during the window. Legal, funds the batch, and validates
   the ₹29,999 price before inventory is committed.
