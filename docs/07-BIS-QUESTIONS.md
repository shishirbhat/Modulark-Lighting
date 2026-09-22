# Compliance question list — who to ask, and exactly what

Every open question across the project, routed to the body that can
actually answer it. Questions are written to be sent verbatim.

## Routing — send to the wrong body and you lose weeks

| Body | Answers | How |
|---|---|---|
| **MeitY** | **Whether a product is notified** under the CRS Order. Scope and classification. | Written query to the IPHW division. The CRS Order is a MeitY order |
| **BIS** (Registration Dept / regional office / CRS portal helpdesk) | **How to register** a product already known to be in scope. Process, CCL, marking, surveillance, variants | CRS portal helpdesk, or written query to the regional office |
| **BIS-recognised / NABL lab** | Test plan, applicable clauses, sample count, quote, lead time | Direct enquiry — get 2–3 quotes |
| **WPC (DoT)** | Radio: frequency permissions, ETA route | eServices portal |
| **Chartered Accountant** | GST rate, supply classification, HSN, refunds | Engagement, **in writing** |
| **Customs broker** | HSN for imported PCBA, clearance risk | Engagement |

## How to ask

1. **Get every answer in writing.** A verbal or phone answer from an
   official is not binding and cannot be relied on later.
2. **Quote the specific standard, clause, part and section** you are asking
   about. Vague questions get vague answers.
3. **Attach a one-page product description** with photos or a render, a
   block diagram showing the power topology, voltages, and a parts list.
4. **Frame every question as seeking correct classification, never as
   seeking to avoid a requirement.** "Which section applies to this
   construction?" not "how do we avoid the glow-wire test." The second
   framing invites adversarial scrutiny and is on record permanently.
5. Expect 2–6 weeks for a written MeitY or BIS response. **Run a paid
   consultant in parallel** — they get faster answers and know precedent.

---

## A. To MeitY — scope and notification (highest value, ask first)

**A1.** Modulark manufactures a wall-mounted LED luminaire powered solely
by a detachable low-voltage lithium-ion battery pack, with no mains
connection to the luminaire. Is this product notified under the Electronics
and IT Goods (Requirements for Compulsory Registration) Order? If so, under
which serial number of the Schedule, and against which Indian Standard?

**A2.** We also manufacture a companion control unit that: contains **no
light source**; is powered by an **external, separately BIS-registered**
AC-DC adapter; is **never in the power path** of the luminaire; and
communicates with the luminaire only by wireless command signal. Is this
control unit notified under the Order? Specifically, does the term
"dimmer" as used in the lighting notifications extend to a wireless
controller that does not switch, regulate or carry the luminaire's supply
current?

**A3.** The same control unit contains charging bays for our proprietary
battery packs. It has **no USB or other output port** capable of powering
third-party devices. Is such a charging function notified — for example as
a power bank, charger or power adapter — or is it outside the Order?

**A4.** Our battery pack is sold both within a system kit and as a spare
part for our own luminaire. It has **no output port for third-party
devices**. Is it notified in its own right, or is it treated as a component
of the registered luminaire?

---

## B. To BIS — registration mechanics

**B1.** Which section of IS 10322 (Part 5), 2026 series, applies to a
wall-mounted, battery-operated, non-emergency general-purpose LED
luminaire? `[resolves O1]`

**B2.** Our luminaire contains a **built-in** DC-supplied constant-current
LED driver, operating from a nominal 3.7 V lithium-ion pack. Is this
built-in control gear covered by the luminaire's own registration under
IS 10322, or does it additionally require separate registration under
IS 15885 (Part 2/Sec 13)? `[resolves O6]`

**B3.** For the Critical Component List, what documentation is required for
components that have **no BIS notified category** — for example the
microcontroller module, sensors, connectors and magnets? Is a manufacturer
datasheet sufficient?

**B4.** For the polycarbonate diffuser, is a **material-level GWIT/GWFI
certificate from the resin supplier** accepted on the CCL, or must the
finished diffuser part itself be tested?

**B5.** Our enclosure is CNC-machined aluminium, and the PCB is mounted to
it on metal standoffs. There is **no internal plastic structural part**.
Which non-metallic parts, if any, remain subject to glow-wire testing in
this construction?

**B6.** What are BIS's requirements for the **registered manufacturing
premises** — minimum facilities, process controls, records? What is
inspected or sampled during surveillance, and how much notice is given?

**B7.** Our PCB assemblies are **fabricated and assembled overseas** and
imported; final assembly, testing and firmware loading of the finished
luminaire occurs at our premises in India. For CRS purposes, are we the
**Indian manufacturer** of the finished luminaire, or are we treated as an
importer? Does this change the registration route or require an Authorised
Indian Representative?

**B8.** Do the **imported PCB assemblies themselves** require any BIS
registration or documentation at the time of customs clearance, given that
they are components of a product we will register, and are not notified
products in their own right?

**B9.** If we later offer the **same luminaire in different anodised
finishes or two physical sizes**, does each require a separate
registration, or can they be covered as variants of one registered model?
What defines a separate "model" for this purpose?

**B10.** What triggers **re-testing** versus a simple CCL amendment if we
subsequently change our CNC vendor, our diffuser supplier, or our LED
supplier, with no change to the electrical design?

**B11.** Please confirm the **validity period of a test report** for
submission with a registration application, and what event starts that
period. `[we understand 90 days from issue — confirm]`

**B12.** What are the **marking and labelling requirements** — where the
registration number must appear on the product, the packaging and the
literature, and the required format?

---

## C. To the BIS-recognised test lab

**C1.** Please quote a **full test plan, price and lead time** for BIS CRS
registration testing of the attached luminaire against IS 10322 (Part 5),
2026 series. Please state which section you would test to.

**C2.** How many **samples** are required, and are they destroyed?

**C3.** **Lead time** from sample receipt to issued report, and your
current queue.

**C4.** Is **photobiological safety testing (IEC 62471)** required for this
product, and if so what risk group classification do you anticipate for a
CRI 95 dual-channel warm/cool LED luminaire?

**C5.** Given a metal enclosure and a SELV-only interior with no internal
plastic structural part, **which glow-wire clause and temperature** would
you apply to the polycarbonate diffuser?

**C6.** Do you accept a **resin-supplier GWIT/GWFI certificate** for the
diffuser, or do you test the part?

**C7.** What **documentation must accompany the sample** — CDF, CCL,
schematics, layout, BOM, supplier certificates?

**C8.** Are there any aspects of this construction you would flag as
**likely to fail or cause delay** on a first submission?

---

## D. To WPC (DoT)

**D1.** Confirm that **24–24.25 GHz is delicensed** in India for low-power
short-range presence-detection radar at the power level of the LD2410
module. `[resolves O5]`

**D2.** Confirm that our devices qualify for **ETA by self-declaration**,
and specify the RF test report format and accreditation required.

**D3.** Is a **separate ETA required for each model**, and does a model
carrying both a Wi-Fi/BLE module and a 24 GHz radar module require one ETA
or two?

---

## E. To the Chartered Accountant — in writing

**E1.** Current **GST rate and HSN** for an LED luminaire post the
September 2025 rationalisation. Published sources conflict between 5% and
12%; the 12% slab appears withdrawn. `[resolves O4]`

**E2.** A kit sold at a single price containing a luminaire, a controller
and a battery pack — is this a **composite supply** with the luminaire as
principal supply, or a **mixed supply** taxed at the highest component rate
under CGST s.8(b)? What documentation or packaging supports the composite
treatment?

**E3.** Correct **GST rate and HSN for each SKU sold separately**.

**E4.** **Inverted duty structure**: we will pay 18% IGST on imported PCB
assemblies and collect a lower rate on output. Confirm eligibility for
refund of accumulated ITC under CGST s.54(3), the filing mechanics, and
realistic timelines.

---

## F. To the customs broker

**F1.** Correct **HSN classification for imported populated PCB
assemblies** that are components of an LED luminaire, and the applicable
BCD and SWS.

**F2.** Any **clearance risk** that shipments are held pending BIS
documentation, and how to pre-empt it. (See B8.)

---

## Priority

Ask in this order. The first three change the plan; the rest change the
cost.

| Order | Questions | Why first |
|---|---|---|
| 1 | **A2, A3** | If the Core is outside CRS it ships on WPC ETA alone, months earlier |
| 2 | **B1, B2** | Determine the test plan and whether there is a second registration |
| 3 | **B7, B8** | Wrong answer here means the wrong registration route entirely, plus customs risk |
| 4 | **C1–C8** | Cannot book the lab or start the 90-day clock without this |
| 5 | **E1, E2** | Worth roughly ₹3,100 per kit |
| 6 | Everything else | Cost and operational detail |

## What not to ask

Do not ask any official how to **avoid, bypass or minimise** a
requirement, and do not use the word "loophole" in any written
correspondence. Every question above is framed as seeking correct
classification for a specific construction. Keep it that way — these
records persist, and BIS surveillance and any future product-liability
proceeding can read them.
