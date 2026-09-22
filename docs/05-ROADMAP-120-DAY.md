# 120-day plan to first shipped revenue

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
