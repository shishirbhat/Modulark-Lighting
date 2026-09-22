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

---

# Addendum 2026-09-22 — Core scope, component certification, test validity

## 7. Does the Core (sensor + charging pod) need BIS?

**CRS is a closed, enumerated list of ~65 notified categories by serial
number.** It is not a blanket rule covering all electronics. The only
question is whether the Core matches an entry.

**Assessment: probably out of scope, but unresolved.** O2 stands.

| Out of scope | Strength |
|---|---|
| Not a luminaire — contains no light source | Strong |
| Not a power bank — no portable output | Strong |
| Not a power adapter — uses an external certified one | Strong, **conditional** |
| Not notified IT equipment (laptop, tablet, printer…) | Strong |
| Not a dimmer in the power-path sense — sends wireless commands only, never in the Field's power path | Moderate |

| In scope / risk | Assessment |
|---|---|
| Lighting notification covers "lamps, luminaires, modules, drivers and **dimmers**." If BIS reads a wireless controller as a dimmer, the Core is in. | **The real risk. Cannot be resolved from public sources.** |
| IS 15885 Part 2/Sec 13 covers DC-supplied electronic control gear for LED modules, built-in and independent | Weak — the Core supplies no power to the LEDs; the Pack does |
| An SMPS placed **inside** the Core would pull it into IS 13252 / IEC 62368-1 | **Entirely within our control — do not do this** |

### Design rules that follow

1. **The mains adapter stays external and BIS-certified.** Never integrate
   an SMPS into the Core to save cost. This is the single decision that
   most improves the Core's chance of being out of scope. Reinforces D5.
2. **If the Core is ruled in scope, certify to IS/IEC 62368-1:2023, not
   IS 13252.** IS 13252 Part 1 and IS 616 are withdrawn on **1 November
   2028**. Certifying to the outgoing standard means paying twice.

## 8. New open question — O6

**Does the Field module's internal constant-current LED driver require
separate registration under IS 15885 Part 2/Sec 13, or is it covered as
built-in control gear by the luminaire's own registration?**

Normal practice is the latter — built-in control gear is tested as part of
the luminaire. But if BIS requires separate registration that is another
model and roughly another ₹1L. **Add to the consultant's brief.**

## 9. Using BIS-certified components does not remove registration

Asked and answered: **it does not, and it saves zero days.**

- CRS applies to the **final assembled product**, not its components.
- IS 10322 Part 1 is explicit: **LED modules are integral components of the
  luminaire and are tested as assembled in the luminaire.**
- Only four BOM categories have any BIS certification available at all:
  cells (IS 16046 — locked, D4), encapsulated AC-DC modules and adapters
  (IS 13252 — locked, D5), mains LED drivers (IS 15885 — **not applicable**,
  the Field is SELV), and LED modules (IS 16103 — **do not pursue**, the
  registered Indian supply base is CRI 80 and would cost us the CRI 95
  differentiator).
- Everything else — MCU, sensors, pogo pins, magnets, PCB, passives,
  diffuser, aluminium — has **no BIS category to be certified under**.

**What certified components do buy:** a clean Critical Component List (CCL)
that passes verification without argument, and lower first-pass failure
risk in the mains path. Worth the ~₹450–550/kit premium. Not a shortcut.

## 10. Scheduling trap — test reports expire in 90 days

**BIS test reports are valid for 90 days from issue** and must reach BIS
before expiry.

Consequences:
- You **cannot** test early to get ahead. The report will expire.
- Design freeze must be genuinely final before a sample reaches the lab.
- Testing and application submission must be tightly sequenced.

Build this into Phase C timing in `05-ROADMAP-120-DAY.md`.

## 11. Closed avenues — do not re-investigate

Four separate routes around the ~90-day BIS CRS timeline have been
researched and all are closed:

| Route | Status |
|---|---|
| Battery-powered products fall outside scope | **Closed.** IS 10322:2026 added a normative annexure on battery/EDLC-operated luminaires |
| HSE exemption (<100 units/model/year) | **Closed.** Requires three-phase, or >16 A single-phase, or >1.5 m × 0.8 m |
| Air gap bypasses the glow-wire test | **Closed.** Moves the part from tier 1 to tier 2; it is still tested at 650°C |
| Building from BIS-certified components | **Closed.** CRS certifies the finished product; components are tested as assembled |

**The 90 days is fixed and starts when the design is frozen and the lab is
booked. The only lever is freezing sooner.** Future sessions should not
spend time re-litigating this — fill the window instead (pre-orders,
firmware, store, photography all run inside it at no schedule cost).

## 12. Correction — Class III / battery operation does NOT shrink the test matrix

A claim circulated internally that because the product is battery-powered
and Class III / SELV, the lab "skips insulation, leakage and surge tests"
and the matrix "shrinks to IP rating and thermal rise only", giving a
30–45 day timeline. **This is wrong and acting on it will fail the test.**

**What Class III actually removes:** electric-shock and dielectric tests —
insulation resistance, leakage current, dielectric strength. Real, but
narrow.

**What Class III does NOT remove.** IEC 60598-1's requirements cover
classification, marking, mechanical construction, electrical construction
and photobiological safety, none of which are voltage-class dependent:

- **Glow-wire 650°C on non-metallic parts** — applies regardless of voltage
  class. Our diffuser still faces it. See §2.
- **Photobiological safety, IEC 62471** — risk group classification
- **Thermal rise, marking, mechanical, construction, endurance**

**Why this matters financially:** believing the matrix is "IP + thermal
only" means skipping qualification of the certified PC diffuser — the
single gating item for our certification. That failure surfaces at the lab,
roughly six weeks and ~Rs 40k in.

**On the timeline:** the 24–30 month estimate in `05-ROADMAP-120-DAY.md` was
never driven by high-voltage testing. It is driven by **capital
availability** (Modulus revenue). Our architecture has been SELV-only and
mains-free since `CLAUDE.md` rule 1 was written. Arguments that "battery
operation escapes the mains timeline" address a constraint this project
never had.

**On the battery annexure:** IS 10322:2026 added its normative annexure on
battery/EDLC-operated luminaires to bring them explicitly **into** scope.
It is not an exemption. See §11, which already records this.

**Pre-certified cells** (D4) remain correct and already banked — buying
BIS-registered cells under IS 16046 avoids registering cells ourselves.
That is a real saving, not a new discovery, and it does not shorten the
luminaire's own test plan.
