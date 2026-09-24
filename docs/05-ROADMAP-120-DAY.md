# 120-day plan to first shipped revenue

> **SUPERSEDED IN PART — see REVISION 2026-09-22 at the end of this file.**
> Capital assumptions below are not currently met, the build/certify order
> is corrected there, and the pre-order funding mechanism is withdrawn.

Objective: cheapest and fastest legal path to a shipped, premium,
BIS-registered product sold direct. Total cash requirement **~₹15.2 lakh**,
of which ~₹4.5L can be covered by pre-order deposits.

**The gate is BIS CRS on the Field module: ~90 days, not compressible.
Everything else is scheduled to fit inside that window at no schedule cost.**

## Phase A — Days 0–14: rulings (₹0.65L)

Do this before spending anything else. It is the cheapest money in the plan
and it can change the whole schedule.

| Action | Cost |
|---|---|
| BIS compliance consultant: resolve O1, O2, O3 (Field section, Core scope, Pack coverage) | ₹40k |
| CA written opinion: GST rate, composite vs mixed supply, HSN (O4) | ₹25k |
| WPC consultant: confirm 24 GHz delicensing for LD2410 (O5) | included |

**Decision point:** if O2 returns "Core is outside CRS", the Core can ship
on WPC ETA alone in ~6 weeks. That is a sellable product months earlier.

## Phase B — Days 0–45: prototype to frozen design (₹3.2L)

| Action | Cost |
|---|---|
| 3 PCBA spins × 3 boards, incl. shipping and duty | ₹1.2L |
| CNC prototype parts, 3 iterations, local job shop | ₹0.7L |
| Components for prototypes | ₹0.5L |
| Bench tools not already owned | ₹0.4L |
| Spectrometer (needed to defend the CRI 95 claim) | ₹0.4L |

Design freeze on the Field module by **day 45**. Nothing after this point
may change its enclosure, diffuser, driver or wiring without restarting
BIS.

## Phase C — Days 45–135: compliance, in parallel (₹3.2L)

| Action | Cost | Duration |
|---|---|---|
| **BIS CRS, Field module** — lab booking + testing + application | ₹1.4L | **90 days — critical path** |
| WPC ETA × 3 models (₹10k govt + RF test each) | ₹1.5L | 2–6 weeks |
| BIS-registered cell sourcing and samples | ₹0.3L | 4–8 weeks |

## Phase D — Days 45–120: commercial, in parallel (₹0.6L)

Runs free inside the BIS window. Founder does design and build at ₹0 cash.

| Action | Cost |
|---|---|
| Product photography — **do not skimp, this is where premium is won** | ₹0.5L |
| Store: Next.js + Supabase + Razorpay, domain, hosting | ₹0.1L |
| Brand, copy, landing page, pre-order flow | ₹0 (in-house) |

**Open pre-orders at ₹29,999 with a 50% deposit from ~day 60.** Legal
before certification; shipping is not. This validates the price and funds
Phase E before components are bought.

## Phase E — Days 90–150: first batch, 30 kits (₹5.5L)

| Action | Cost |
|---|---|
| Components for 30 kits @ ~₹15,000 | ₹4.5L |
| Packaging, 300-unit MOQ | ₹1.0L |

30 kits × ₹29,999 = **₹9.0L revenue.** At 50% deposits, ~₹4.5L arrives
before the components are ordered.

## Cash summary

| Phase | Cost |
|---|---|
| A — rulings | ₹0.65L |
| B — prototype | ₹3.2L |
| C — compliance | ₹3.2L |
| D — commercial | ₹0.6L |
| E — first batch | ₹5.5L |
| Buffer (~15%) | ₹2.0L |
| **Total** | **~₹15.2L** |
| Less pre-order deposits | −₹4.5L |
| **Net capital at risk** | **~₹10.7L** |

Down from the ~₹30L minimum under the original four-SKU, 3D-printed,
designer-channel plan. The savings come from: three SKUs instead of four,
no printer farm, no injection tooling, ₹0 design, and direct sales
collapsing the cash cycle.

## Gate conditions — do not pass without these

| Gate | Condition |
|---|---|
| Before Phase B | O1–O5 answered in writing |
| Before Phase C | Field design frozen; AS7341 dual-sourced or a fallback designed |
| Before Phase E | **≥20 pre-orders collected as real money at ₹29,999** |
| Before scaling past 45 kits/mo | Hire assembly help or outsource assembly — this is the hard solo ceiling |

**If pre-orders do not reach 20 at ₹29,999, stop.** You will have spent
~₹7.5L, not ₹30L, learning that the price does not clear the market. That
is the whole point of sequencing it this way.

## What would still kill this

1. **Pre-orders come in below 20.** The ₹29,999 price is the entire
   thesis. No price below ~₹25,000 clears the cost base solo.
2. **The Core is ruled inside CRS** and adds ₹1L plus 3 months.
3. **AS7341 allocation** freezes the line with inventory half-built.
4. **GST is ruled 18% mixed supply** and the Field section turns out to
   require a costlier test route — compresses margin to the point where
   break-even approaches the ceiling.
5. **Modulus revenue never arrives.** The funding premise for this division
   is a SaaS product whose payment gateway is still unverified. Verify it
   this week; it costs nothing and it underwrites everything above.

---

# REVISION 2026-09-22 — funding reality and corrected sequence

**The 120-day plan above assumed ~₹15.2L of available capital. That capital
does not exist.** The plan is not cancelled, but its timeline is now gated
by Modulus SaaS revenue, not by BIS.

## Corrected sequence — the original order was inverted

Previously implied: fund → certify → build. **This is wrong and wastes
money.**

```
  BUILD  →  FREEZE  →  CERTIFY  →  PRODUCE
  ~Rs 0     no cost    Rs 1.4L+     Rs 5.5L+
  START     gate       90 days
  NOW
```

BIS tests a physical sample of a frozen design — a product that does not
yet exist cannot be certified. And test reports **expire 90 days from
issue**, so certifying before you can produce wastes the fee entirely.

**Consequence: prototyping is not blocked on money.** Start now. Capital is
only required at the certification gate.

## Funding source: Modulus SaaS

| Schools signed | Annual revenue @ ~Rs 40k | Unlocks |
|---|---|---|
| 2 | Rs 0.8L | Phase A rulings |
| 5 | Rs 2.0L | Prototype PCBAs, CNC samples |
| 3–4 | Rs 1.5L | **Phase C compliance, post-MSME concessions** (see `02-COMPLIANCE.md` §13) |
| 10 | Rs 4.0L | Phase C compliance at pre-concession cost |
| 35–40 | Rs 15L | Full original plan |

`[ESTIMATE]` — pricing and pipeline unconfirmed. Note Indian school
procurement clusters February–April for the June academic year.

**Realistic: first legal hardware sale 24–30 months out under this plan.**

## OPEN STRATEGIC DECISION — "brain first"

Not locked. Founder decision required before capital is committed.

If the Core is ruled **outside CRS scope** (question O2 / A2), Modulark
could ship the Core alone as a local no-cloud controller commanding
existing Matter or Zigbee bulbs, deferring the Field module entirely.

| | Full v1 kit | Brain-first |
|---|---|---|
| Certification | BIS CRS + WPC | **WPC ETA only** |
| Compliance cost | Rs 5–7L | **~Rs 60–90k** |
| Compliance time | 90+ days | **2–6 weeks** |
| Capital to first sale | Rs 15.2L | **~Rs 2L** `[ESTIMATE]` |
| Proves the solver (the actual IP) | Yes | **Yes** |

Trade-off: loses the complete-system positioning and cedes CRI control to
third-party bulbs. Gains roughly 18 months.

**This elevates O2/A2 to the single highest-value question in the project.**

## Do now, at ~Rs 0

1. Breadboard the solver — ESP32 dev board + AS7341 + VEML7700 breakouts,
   ~Rs 3,000–5,000. This is the IP.
2. Get Modulus accepting payments. Requires an adult on the merchant
   account. This is the funding tap.
3. Enter Youth Co:Lab / India STEM Innovation Challenge. Seed grants of
   Rs 2.2–5L would fund Phases A and C outright.

## Governance note

The founder is a minor. A minor cannot hold a DIN or be a director
(Companies Act 2013), and a minor's contracts are void ab initio (Indian
Contract Act s.11). **An adult director/signatory executes all contracts:**
BIS applications, lab agreements, vendor POs, merchant accounts.

**Do not take customer pre-orders or deposits** for any product not yet
BIS-registered. Superseded guidance elsewhere in this file suggesting
pre-orders as a funding mechanism is **withdrawn**.
