# Legal entity, registrations and sequencing

**No legal entity currently exists.** Earlier documents referred to
"Modulark Tech Labs Pvt Ltd" as operating; that was inaccurate and is
corrected here.

The founder is a **minor**. A minor cannot hold a DIN, cannot be a director
(Companies Act 2013), and a minor's contracts are void ab initio (Indian
Contract Act s.11). **An adult acts as proprietor/director and signs
everything.** A minor may hold gifted fully-paid shares with a guardian
voting, but cannot subscribe to the MOA at incorporation.

## The inversion that had to be fixed

The plan was "get Modulus revenue, then register a company." This cannot
run in that order: invoicing a school and receiving payment requires an
entity and a bank account, neither of which a minor can hold.

**The entity comes first. It just does not have to be a company.**

## Recommended: sole proprietorship now, decide on Pvt Ltd at the BIS gate

| | Sole proprietorship | Private limited |
|---|---|---|
| Setup cost | **~Rs 0** | ~Rs 8–15k |
| Annual compliance | **~Rs 0** | ~Rs 15–25k/yr (CA, ROC, audit) |
| Invoice customers | Yes | Yes |
| **Udyam registration** (free, Aadhaar + PAN, no separate entity) | Yes | Yes |
| **80% BIS fee concession** (micro) | Yes | Yes |
| MSME 75% testing subsidy | Yes | Yes |
| **DPIIT startup recognition** | **No — not eligible** | Yes |

A Pvt Ltd costs Rs 15–25k/year regardless of revenue. Pre-revenue that is a
pure drain with no offsetting benefit except DPIIT.

**Converting later does not cost the startup clock.** Per the DPIIT office
memorandum dated 30.06.2021, on conversion from proprietorship to Pvt Ltd
or LLP, recognition may be backdated to commencement of the
proprietorship.

## Decision point: before the BIS application, not before Modulus revenue

BIS registration names the **entity and the premises**. Registering under a
proprietorship and then converting likely means re-applying or
transferring — real cost, real delay.

The natural decision point is at 3–4 schools signed, when certification is
being paid for anyway and the Pvt Ltd's ~Rs 20k/year can be judged against
actual revenue.

## Corrected sequence

```
1. Adult registers SOLE PROPRIETORSHIP + bank account     ~Rs 0
2. UDYAM REGISTRATION (free, ~15 min)                     ~Rs 0   <- gates the 80% BIS concession
3. Modulus invoices schools -> first revenue
4. Breadboard prototype, in parallel, from step 1         ~Rs 5,000
5. At 3-4 schools: DECIDE ENTITY (proprietorship or Pvt Ltd)
6. Consultant rulings (A2/A3, B13)                        ~Rs 65k
7. Freeze design -> lab testing
8. DRAFT BIS APPLICATION DURING TESTING                   <- report expires in 90 days
9. File application on report issue -> 4-6 weeks
10. Legal sales. Build to orders, not to inventory
```

## GST

Services threshold is **Rs 20 lakh** turnover (Rs 10L in special category
states), so Modulus will likely sit below mandatory registration initially.
Two reasons to register voluntarily anyway:

1. Schools frequently require a GST invoice.
2. Without registration there is **no input tax credit** on imported PCBAs
   later — relevant to the inverted duty structure in
   `02-COMPLIANCE.md` §4.

## Open items

| # | Item | Why now |
|---|---|---|
| E1 | **MCA name availability check on "Modulark"** | It will go on packaging, a BIS certificate and a domain. Cheap now, very expensive to change after the BIS registration carries it |
| E2 | **Trademark search on "Modulark"** | Same. Check before the brand is committed anywhere |
| E3 | Confirm the adult signatory's availability for Udyam, bank, GST and all vendor contracts | Everything depends on it |

## Two gaps corrected in the founder's sequence

**"Once the test report is back, mass-produce."** The report is not
permission to sell. The BIS application follows, 4–6 weeks. And the report
expires 90 days from issue, so the application must be drafted **during**
testing and filed the day the report lands.

**"Mass-produce."** Break-even is 22 kits/month against a solo assembly
ceiling of ~28–45 (`04-UNIT-ECONOMICS.md`, `03-MANUFACTURING.md`). Build to
confirmed orders. Over-ordering inventory is the fastest way to lose the
Modulus money.

---

## Udyam registration notes (2026-09-23)

Registration started as a **sole proprietorship in the founder's mother's
name**. She is the proprietor and sole legal owner.

### Employee count field — not an issue

MSME classification depends **only on investment in plant and machinery
and on turnover** (micro: investment up to Rs 2.5 cr, turnover up to
Rs 10 cr). The employee-count field is statistical and does **not** affect
micro/small/medium status, and therefore does not affect the 80 percent BIS
fee concession. Udyam details are editable later in any case.

### Founder's age — not an issue

At 15 the founder is an **adolescent**, not a **child**, under the Child
and Adolescent Labour (Prohibition and Regulation) Act 1986 as amended
2016. Adolescents aged 14–18 may be employed except in hazardous
processes; the 2016 amendment reduced that schedule from 83 items to 3.
The enterprise is also a family enterprise.

`[CONFIRM]` Before physical assembly begins, confirm with the CA that
nothing in the assembly process falls under the remaining hazardous-process
schedule. Home-scale soldering is very unlikely to, but it is a cheap
question.

## GOVERNANCE GAP — co-founder has no legal standing

A co-founder has been mentioned. **A sole proprietorship has exactly one
owner.** As currently structured:

| Party | Legal ownership |
|---|---|
| Founder's mother (proprietor) | **100% of the business, its revenue and all IP** |
| Founder (minor) | **Nothing** |
| Co-founder | **Nothing** |

This is the correct structure for now and is not a problem in itself. It
becomes one only if the co-founder believes they hold a stake, contributes
for a long period, and later discovers they do not. That misunderstanding —
not business failure — is the most common way young founding teams break.

### Action: write the understanding down now

Not a contract. Both founders are minors, so an agreement between them is
void ab initio and unenforceable. The purpose is to prevent divergent
memories, not to create legal rights. A dated one-page note signed by both,
recording:

1. What each person is contributing
2. The intended split when a real entity exists
3. **That equity accrues over time, not on day one.** Someone who leaves
   after three months should not retain a founder's share
4. What happens if either person leaves
5. That IP belongs to the business, not to either individual

### Formalisation point

The same point as the entity decision: **at the BIS gate / Pvt Ltd
conversion**, when shares exist and can be issued properly. If the
co-founder is also a minor, the same constraints apply — no DIN, no
directorship, contracts void; gifted fully-paid shares with a guardian
voting are possible.

### New open item

| # | Item |
|---|---|
| E4 | Founder-understanding note written and signed by both founders. Zero cost, twenty minutes, do before further work accumulates |
