# Corporate Structure: MOA Objects Clause, and One-Entity vs Two (Modulark Tech Labs Pvt Ltd)

_Research current as of 22 September 2026. Note on sourcing: the agent proxy in this environment blocked direct access to rbi.org.in, indiacode.nic.in, indiacorplaw.in and several primary-source domains. Findings below therefore rely on search-engine synthesis of primary documents plus professional-firm commentary (AZB, Saraf Partners, JSA, S.S. Rana, TaxGuru, CAclubindia). Where a figure could not be corroborated against a primary source it is flagged in **Gaps**. The report-writer should treat exact rupee figures for state stamp duty and professional fees as indicative ranges, not quotations._

---

## (A1) Objects clause drafting post-Companies Act 2013 — Section 4(1)(c) and the 2017 Amendment

### Takeaway
Section 4(1)(c) of the Companies Act 2013 collapsed the 1956 Act's three-part "main / ancillary / other objects" structure into a **single consolidated objects statement**, and — critically — the Companies (Amendment) Act 2017's proposal to allow a **universal/unrestricted objects clause was dropped before enactment**. So India did **not** adopt the UK-style "any lawful business" default: a specific objects clause remains mandatory, and a company whose MOA is worded only for software does **not** thereby acquire power to manufacture hardware.

### Cited Findings
- Section 4(1)(c) requires the memorandum to state "the objects for which the company is proposed to be incorporated and any matter considered necessary in furtherance thereof" — a single objects statement, replacing the 1956 Act's split into main objects, objects ancillary/incidental to the main objects, and "other objects" — [CAIRR / ca2013.com, Section 4 Memorandum](https://ca2013.com/memorandum/) (accessed via search synthesis; direct fetch blocked)
- The Companies (Amendment) Bill 2017 **originally proposed** replacing the objects clause with a universal formula: a company could simply state that it may "engage in any lawful act or activity or business, or any act, activity or business to pursue any specific object or objects" — [IndiaCorpLaw, "Object Clause under the Companies (Amendment) Bill: A Flip-Flop"](https://indiacorplaw.in/2017/08/15/object-clause-companies-amendment-bill-flip-flop/)
- That proposal was **removed before enactment**. The Standing Committee on Finance objected that a universal objects clause "may lead to creation of bogus entities" and that "a well stated object clause instilled confidence amongst the investors and creditors of the company." The suggestion was accepted in amendments circulated 5 April 2017 and **status quo was restored** in the Bill as passed by the Lok Sabha on 27 July 2017 — [IndiaCorpLaw](https://indiacorplaw.in/2017/08/15/object-clause-companies-amendment-bill-flip-flop/)
- "The universal objects clause couldn't find its place in the Amendment Act" — [Lexology, Companies (Amendment) Act 2017 – An analysis](https://www.lexology.com/library/detail.aspx?g=96e04bfc-2f10-4fbd-bef1-57cfeee2e1af)
- The Companies (Amendment) Act 2017 (Act No. 1 of 2018) was passed by Lok Sabha 27 July 2017, Rajya Sabha 19 December 2017, and received Presidential assent 3 January 2018 — [NFCG, The Companies (Amendment) Act 2017 (PDF)](https://www.nfcg.in/UserFiles/THE-COMPANIES-AMENDMENT-ACT-2017.pdf)

### Inferences
- **The single most important correction to a common founder misconception:** many Indian founders and even some advisers believe the 2017 Amendment made objects clauses irrelevant because "the Act removed the objects clause." It did not — the amendment was proposed, publicly discussed, and then withdrawn. Section 4(1)(c) stands substantially as originally enacted. Any advice premised on "objects don't matter any more in India" is wrong.
- The practical consequence of the 2013 Act's single-statement structure is that companies (and SPICe+ templates) responded by drafting **long, broad, omnibus objects clauses** rather than short ones — the drafting incentive runs toward breadth, which is why there is a real chance Modulark's existing MOA already covers hardware.
- Because "and any matter considered necessary in furtherance thereof" is part of the statutory formula, activities genuinely incidental to a stated object are covered without separate enumeration. But manufacturing physical goods is not "incidental" to developing software — it is a distinct line of business with its own capital, plant, workforce and liability profile.

### Gaps
- Could not fetch indiacode.nic.in or the MCA's consolidated Act text directly (egress blocked) to quote the verbatim current statutory text of s.4(1)(c) including any post-2017 amendment marginal notes. The report-writer should verify the exact wording against indiacode.nic.in before quoting it as a quotation rather than a paraphrase.

---

## (A2) Is the doctrine of ultra vires still alive in India? Consequences of acting outside objects

### Takeaway
Yes — the doctrine survives in India and is stronger here than in the UK, precisely because India did **not** adopt the universal objects clause. An ultra vires act is **void ab initio and incapable of ratification even by unanimous shareholder consent**. But the honest practical assessment for a small private company is that the realistic risk is not a regulator prosecuting: it is a **counterparty, insurer, acquirer or investor using it against you** in a dispute or in diligence.

### Cited Findings
- *Ashbury Railway Carriage & Iron Co Ltd v Riche* (1875) LR 7 HL 653 is the foundational authority: a contract outside the company's objects is void and cannot be ratified by the shareholders, however unanimous — classic and uncontested statement of the doctrine (well-established case law; see summary in [Wikipedia, Objects clause](https://en.wikipedia.org/wiki/Objects_clause))
- *A. Lakshmanaswami Mudaliar v Life Insurance Corporation of India*, AIR 1963 SC 1185 — the Supreme Court of India held that a donation by an insurance company to a charitable trust (for the promotion of technical/business education) was **ultra vires** the company's objects, because the objects permitted charitable payments only out of profits and connected with the insurance business; the directors were held liable to make good the money. The case is the standard Indian authority that the doctrine applies with full force in India and that **directors who authorise an ultra vires application of funds can be personally liable to refund it**. (See discussion in Indian company law commentary; primary citation AIR 1963 SC 1185.)

### Inferences (practical vs theoretical risk — be honest with the founder)
This is where commentary tends to be either alarmist or dismissive. The accurate picture has four distinct layers, and they carry very different weights for Modulark:

1. **Contract voidness — theoretical but real tail risk.** An ultra vires contract is void, not merely voidable. In practice, nobody voids a supply contract for LED drivers on this ground; but if the company is ever in litigation with a large counterparty (say a component supplier or a B2B lighting customer refusing to pay), ultra vires is a live defence they can raise, and it is a defence *the company itself cannot cure by ratification*. It is asymmetric: it can only ever be used against Modulark, never by it (the company cannot plead its own ultra vires to escape a bad bargain, and third parties dealing in good faith have some protection, but the doctrine of constructive notice of the MOA — a public document on MCA21 — weakens that protection in India).
2. **Director liability — the sharpest edge.** *Lakshmanaswami Mudaliar* establishes that directors who apply company funds to an ultra vires purpose can be ordered to restore those funds personally. For a founder putting seven figures of SaaS cash into tooling, inventory and a workshop lease for a business the MOA does not authorise, this is the clause that should actually motivate the fix. If the hardware line fails and a creditor or a later investor-controlled board looks for recovery, "the directors spent ₹X crore on a business the company had no power to carry on" is a coherent claim.
3. **ROC penalties — genuinely low.** There is no specific penal section in the 2013 Act headed "carrying on business outside objects," and ROCs do not proactively audit whether a small private company's activities match its MOA. The realistic regulatory exposure is close to nil in the ordinary course.
4. **The real-world trigger: diligence and insurance.** The moment this bites is (a) a seed/Series A investor's legal DD, where "the company carries on a manufacturing business not covered by its objects" is a standard finding requiring a pre-closing condition precedent to rectify; (b) a product liability insurer resisting a claim on the ground the insured activity was not one the company was empowered to carry on; (c) an acquirer's DD on a later sale of either line; (d) a bank or lending partner's KYC/constitutional-document check. For Modulark, with a fintech-adjacent product where a **lending partner will run diligence on the borrower-facing entity**, this is not hypothetical.

**Bottom line to give the founder:** the probability of enforcement action is low; the probability that an unamended MOA costs him time, leverage or money at a financing, an insurance claim or an exit is high. The fix costs a few thousand rupees and a few weeks. Do it before spending money on the hardware line, not after.

### Gaps
- Could not verify via a primary-source database whether any post-2013 Indian judgment has narrowed *Lakshmanaswami Mudaliar*. Treat the doctrine's continued vitality as well-settled textbook law rather than as a freshly verified 2026 holding.

---

## (A3) Practical test — does Modulark's existing MOA already cover hardware manufacturing?

### Takeaway
The founder must actually read his own filed MOA before doing anything else. Companies incorporated through **SPICe+ (INC-32/33/34)** frequently carry broad omnibus objects; there is a meaningful chance manufacturing is already covered. The MOA is a public document retrievable from MCA21.

### Cited Findings
- The MOA is filed with the ROC at incorporation (e-MOA in Form INC-33 for SPICe+ incorporations) and is a public document available through the MCA21 portal (mca.gov.in) under **"View Public Documents" (VPD)** or **"Get Certified Copies"** — [MCA21 portal, mca.gov.in](https://www.mca.gov.in/)
- Section 4(1)(c) requires the objects to be stated, so whatever is on file is the operative limit of the company's capacity — [CAIRR, Section 4](https://ca2013.com/memorandum/)

### Inferences — exactly what to do and what to look for

**Step-by-step retrieval:**
1. Go to mca.gov.in → MCA Services → Master Data / **View Public Documents**. Search by CIN or company name "MODULARK TECH LABS PRIVATE LIMITED".
2. VPD requires login and a per-company viewing fee (nominal, historically ₹100 for 3-hour access to a company's documents; verify current fee on the portal). Documents are grouped — look under **"Incorporation Documents"**.
3. Download the **e-MOA (INC-33)** or the scanned MOA attached to the incorporation form (SPICe / SPICe+ / INC-7 depending on vintage). If the founder already has the incorporation kit from the CS who incorporated the company, it will be in there — faster and free.
4. Alternatively "Get Certified Copies" gives a stamped certified copy (needed if a bank, insurer or investor wants proof).

**What language to look for — this is the test:**
Manufacturing is covered if Clause III(A) (or the single objects clause) contains something in the family of:

> "To manufacture, assemble, design, develop, fabricate, import, export, buy, sell and otherwise deal in electrical, electronic, electro-mechanical and opto-electronic goods, apparatus, appliances, instruments, components, fittings and accessories of every description, including lighting fixtures, luminaires, lamps, LED products, drivers, controls and allied products..."

Key verbs to hunt for: **manufacture, assemble, fabricate, produce, process**. Key nouns: **electrical, electronic, electro-mechanical, apparatus, appliances, goods, hardware, lighting, luminaires, LED**.

**What will NOT cover it:**
A purely software-worded clause — e.g. "to carry on the business of designing, developing, marketing, licensing and maintaining computer software, software as a service, mobile and web applications, information technology services, and to provide IT-enabled services..." — does **not** authorise manufacturing physical goods. Neither does a clause permitting the company "to deal in" or "to trade in" goods, which covers buying and reselling but arguably not manufacture. Nor is manufacturing rescued by the residual "and any matter considered necessary in furtherance thereof," which reaches only matters genuinely incidental to a stated object.

**A trap worth flagging:** some SPICe+ MOAs are *narrower* than founders expect, because the incorporating CS tailored the objects to the NIC code declared at incorporation to avoid ROC queries. Do not assume breadth.

**Drone line (Modulark Aero):** the same test applies. If the MOA is software-only, the drone business is *also* already ultra vires — meaning the company may already be operating outside its objects today, which strengthens the case for amending now and drafting the amendment to cover **software + hardware manufacture + unmanned aerial systems + trading/import/export** in one pass, rather than amending twice.

### Gaps
- Could not confirm the **current** MCA21 View Public Documents fee (the ₹100/3-hour figure is the long-standing rate but the portal has been revised under MCA21 V3). Founder should check at the point of use.
- Cannot inspect Modulark's actual MOA — no CIN was supplied and it is not in the repository. This is the single most important unknown in part (A) and should be the founder's first action item.

---

## (A4) How to alter the objects clause — Section 13 procedure

### Takeaway
Altering the objects clause of a **private** company requires a **special resolution (75%)** of members plus filing of **Form MGT-14 within 30 days**. **No Central Government / Regional Director approval is required** for an objects alteration (CG approval under s.13 attaches to a change of *registered office from one state to another*, not to objects). For a founder-controlled private company this is administratively easy — the hard part is drafting, not approval.

### Cited Findings
- Section 13 of the Companies Act 2013 governs alteration of the memorandum; alteration requires a special resolution — [Compliance Checklist for amending the object clause of a company, SCC Online](https://www.scconline.com/blog/post/2021/02/17/compliance-checklist/)
- MGT-14 must be filed with the ROC; the filing fee is set by the Companies (Registration Offices and Fees) Rules 2014 and scales with **authorised capital** — [LegalWiz, Form MGT-14](https://www.legalwiz.in/blog/form-mgt-14-filing-requirements); [IndiaFilings, MGT-14](https://www.indiafilings.com/learn/mgt-14)
- Delay in MGT-14 filing attracts additional fee; for a delay of up to 30 days the fee is doubled (escalating multiples thereafter) — [MGT-14: Filing Requirements, Due Date & Fees, EquityList](https://www.equitylist.co/blog-post/mgt-14)

### Inferences — exact sequence

1. **Board meeting.** Issue at least 7 days' notice (s.173(3)). Board resolution to: (a) approve the proposed alteration of Clause III of the MOA and the specific new sub-clause text; (b) approve calling an EGM (or place the item at the next AGM); (c) approve the notice and explanatory statement under s.102; (d) authorise a director/CS to sign and file.
2. **Notice of general meeting.** 21 clear days' notice to members, directors and auditors (s.101), with an **explanatory statement under s.102** setting out the reasons for the alteration. Shorter notice is possible with consent of 95% of members entitled to vote — in a two- or three-founder company this is routine, and a **shorter-notice EGM held the same week is entirely normal practice**.
3. **EGM — special resolution.** Passed by not less than three-fourths of votes cast (s.114). Objects alteration under s.13(1) is expressly a special-resolution matter.
4. **File Form MGT-14** with the ROC **within 30 days** of passing the resolution (s.117(1)). Attachments: certified true copy of the special resolution, the notice of the general meeting with the explanatory statement, and the **altered MOA** (both marked-up and clean versions in practice).
5. **ROC processing / registration.** The alteration takes effect on registration by the Registrar. MGT-14 for a special resolution is generally processed on an STP (straight-through-processing) basis; expect an approval/acknowledgement rather than a substantive adjudication, though the ROC can raise a resubmission query on drafting.

**Section 13(8) — not applicable here.** s.13(8) restricts a company that has **raised money from the public through a prospectus** and still has unutilised prospectus money from changing its objects unless a special resolution is passed and the dissenting shareholders are given an exit offer (with additional disclosure by advertisement, Rule 32 of the Companies (Incorporation) Rules 2014). A private limited company that has never issued a prospectus is outside this entirely. **Confirmed not applicable to Modulark.**

**Central Government / Regional Director approval — NOT required for objects.** Under s.13(4) read with s.13(7), CG (delegated to the Regional Director) approval is required for alteration of the **registered office clause where the registered office shifts from one State to another**. There is no CG approval requirement for altering the **objects** clause of a private company. (Name-change alterations engage a different CG/ROC process.) So the whole exercise is: board → members → ROC filing.

**NIC code / business activity code.** The NIC-2008 code declared in SPICe+ (and carried in the company's MCA master data) describes the principal business activity. Adding a manufacturing line should be reflected: (a) the objects clause itself should reference the activity; (b) the **annual return in Form MGT-7 / MGT-7A** requires the principal business activities of the company with NIC codes — update this at the next filing to show the manufacturing activity (NIC Division 27 covers manufacture of electrical equipment; Group 274 covers manufacture of electric lighting equipment). There is no separate standalone "change NIC code" form for an existing company outside these filings; the practical vehicle is MGT-7/7A plus the amended MOA. Some advisers also file **Form INC-28 / GNL-2** in specific cases — not required here.

### Gaps
- Could not verify from a primary MCA source whether any 2025–26 MCA circular altered the MGT-14 process or introduced a V3-portal variant of the form. The report-writer should note the procedure as stable but flag MCA21 V3 form-version churn as a practical annoyance.
- The precise NIC-2008 sub-class for LED luminaire manufacture (likely 27400) was not verified against the MCA NIC code list in this research pass.

---

## (A5) Timeline and cost of the objects alteration

### Takeaway
This is a **cheap and fast** exercise: realistically **₹15,000–₹50,000 all-in** and **3–6 weeks elapsed**, dominated by professional fees and stamp duty, not government fees. The MGT-14 filing fee itself is ₹300–₹600.

### Cited Findings
- MGT-14 filing fee by authorised (nominal) share capital, under Rule 12 / the Companies (Registration Offices and Fees) Rules 2014 — [EquityList, MGT-14 fees](https://www.equitylist.co/blog-post/mgt-14); corroborated in structure by [Patron Accounting, SH-7 filing: stamp duty, ROC fee slabs](https://www.patronaccounting.com/blog/sh-7-filing-costs-stamp-duty-roc-fee-slabs-common-rejection-reasons):

| Authorised (nominal) share capital | MGT-14 / ROC document filing fee |
|---|---|
| Less than ₹1,00,000 | ₹200 |
| ₹1,00,000 to ₹4,99,999 | ₹300 |
| ₹5,00,000 to ₹24,99,999 (sources render the upper bound as ₹25,99,999) | ₹400 |
| ₹25,00,000 / ₹26,00,000 to ₹99,99,999 | ₹500 |
| ₹1,00,00,000 and above | ₹600 |

- Delay up to 30 days doubles the fee; further delay escalates in multiples — [EquityList](https://www.equitylist.co/blog-post/mgt-14)
- Stamp duty on instruments is a **State subject**; rates vary by State and are levied under the relevant State Stamp Act / Schedule I of the Indian Stamp Act as adapted — [Stratjuris, Decoding Indian Stamp Duty Requirement for IP instruments](https://stratjuris.com/decoding-indian-stamp-duty-requirement/)

### Inferences — realistic budget and calendar

**Costs:**
| Item | Realistic amount | Notes |
|---|---|---|
| MGT-14 ROC filing fee | ₹300–₹600 | Per the slab table above; for a typical startup with ₹1–10 lakh authorised capital, **₹300–₹400** |
| Stamp duty on the altered MOA | **Nil to ~₹1,000 in most States for an objects-only alteration** | Stamp duty on the MOA is charged at incorporation and on **increases in authorised capital**; an objects-only alteration with no capital change usually attracts little or no fresh duty. Where charged, State schedules for "Memorandum of Association" range from ₹200 (several States) to ₹1,000+; Maharashtra, Delhi, Karnataka, Tamil Nadu and Gujarat all differ. **Confirm with the CS for the State of the registered office.** |
| Company Secretary / professional fees | **₹8,000–₹35,000** | Covers drafting the new objects sub-clauses, board and EGM papers, minutes, MGT-14 filing and the digitally signed certification. Metro CS firms quote at the upper end; a small-town practitioner or an online filing platform (IndiaFilings, LegalWiz, Vakilsearch) at the lower end. Budget ~₹15,000 for competent drafting — **do not cheap out on the drafting**, because the whole point is to get breadth right in one pass. |
| Certified copies / incidentals | ₹500–₹2,000 | VPD/certified copy fees, notarisation, courier |
| **Total** | **≈ ₹15,000–₹50,000** | Realistic central estimate ~₹20,000–₹25,000 |

**Timeline (from decision to registered alteration):**
- Day 0–7: instruct CS, draft new objects clause (the real bottleneck — get it broad enough to cover lighting hardware, drones, trading, import/export and future adjacent hardware).
- Day 7: board meeting (7 days' notice, or shorter with consent).
- Day 7–28: 21 clear days' EGM notice — **or compress to a few days** with 95% shorter-notice consent, which a founder-controlled company can do trivially.
- EGM + special resolution: 1 day.
- MGT-14 filing: within 30 days; in practice file within a week.
- ROC registration: typically **3–15 working days** on STP, longer if a resubmission query is raised.

**Realistic elapsed time: 2–3 weeks on the shorter-notice route; 5–6 weeks if the full 21-day notice period is observed.** This is not a project. It should not delay the hardware plan by a single month if started now.

### Gaps
- **State-specific stamp duty on an altered MOA could not be pinned down to a citable schedule entry.** I did not find a reliable consolidated table of State stamp duty on MOA *alteration* (as distinct from incorporation or capital increase). This is genuinely State-specific and the report should say so rather than give a false-precision number. The founder's State of registered office was not supplied.
- Professional fee figures are market estimates from general knowledge of Indian CS pricing, not sourced quotations — flag as indicative.

---

## (A6) Knock-on consequences of adding a manufacturing line

### Takeaway
Adding manufacturing triggers a cluster of small, cheap, mostly-registration obligations rather than any single large one. The two that most often surprise founders are **GST additional place of business** (must be added *before* operating from the workshop) and the **municipal trade licence**. **Factories Act 1948 almost certainly does NOT apply** to a small assembly workshop, and **electronics assembly is a CPCB White category activity now exempt from both Consent to Establish and Consent to Operate** — a significant 2024–25 liberalisation.

### Cited Findings

**Pollution control — the best news in this section:**
- The CPCB's White Category covers activities with a Pollution Index below 25 and negligible pollution potential. The 2016 CPCB categorisation lists 39 White-category sectors including **"electrical and electronic item assembling (completely dry process)"** — [Spans Envirotech, CPCB Industry Categorization](https://spans.co.in/knowledge/cpcb-industry-categorization-red-orange-green-white/); [TeamLease RegTech, White-category Industries in India](https://www.teamleaseregtech.com/blogs/117/white-category-industries-in-india-an-overview/)
- Non-polluting White category industries are now **exempt from obtaining both Consent to Establish (CTE) and Consent to Operate (CTO)** — [Business Standard, "'White Category' industries no longer need State Pollution Board approval" (Nov 2024)](https://www.business-standard.com/industry/news/white-category-industries-no-longer-need-state-pollution-board-approval-124111302019_1.html)
- The exemption is not unconditional: such industries "shall **intimate the Board** about their operations and **self-declared compliance** with environmental laws," per the SOP prescribed under the MoEFCC notification — [TeamLease RegTech](https://www.teamleaseregtech.com/blogs/117/white-category-industries-in-india-an-overview/); [Upstox, Govt exempts white category industries from dual environmental approvals](https://upstox.com/news/business-news/latest-updates/govt-exempts-white-category-industries-from-dual-environmental-approvals-check-the-list/article-128569/)
- State boards have implemented this: e.g. the Gujarat PCB formally exempted White Category industries from CTE and CTO in June 2025 — [GPCB exemption circular, 19 June 2025 (PDF)](https://uncomplycate.com/wp-content/uploads/2025/06/GPCB-exempts-White-Category-Industries-from-Requirement-of-Consent-to-Establish-and-Consent-to-Operate-June192025.pdf); [Environment Notifications](https://environmentnotifications.in/white-category-industries/)

### Inferences — the checklist

1. **Articles of Association — generally NO change needed.** The AoA governs internal management (share transfers, board, meetings); it does not enumerate businesses. Adding a manufacturing line does not itself require an AoA amendment. *Exception:* check whether the AoA contains any borrowing limit, business-restriction covenant, or investor-consent matter that a new capital-intensive line would breach. Table F-based AoAs will not.
2. **NIC code / MGT-7A** — update principal business activity at the next annual return (NIC Division 27, electrical equipment; lighting equipment falls in Group 274). See (A4).
3. **GST.** Two points. (a) If the workshop is at a different address in the **same State** as the existing registration, add it as an **additional place of business** by amending the registration in **Form GST REG-14** (non-core/core field amendment; additional place of business is a core field requiring officer approval, typically 15 working days). (b) If the workshop is in a **different State**, a **separate GST registration for that State is mandatory** — GST is State-wise. The old concept of separate registration for "business verticals" within a State was replaced by the option of **separate registration for multiple places of business within a State** (s.25(2) CGST Act read with Rule 11) — optional, and usually **not worth it** for Modulark because it forces inter-unit supplies to be treated as taxable supplies with invoicing between the units. Recommendation: one GSTIN per State, workshop added as an additional place of business. Also add the new HSN codes for luminaires (Chapter 94, heading 9405) to the registration/invoicing setup.
4. **Udyam / MSME registration.** Free, online, self-declaration at udyamregistration.gov.in on the basis of PAN and GSTIN. **Worth doing**: it unlocks the MSMED Act s.15/16 delayed-payment protection (buyers must pay within 45 days or pay compound interest at 3× the RBI bank rate), priority sector lending, and various State manufacturing subsidies and electricity-duty concessions. Note the Income Tax Act s.43B(h) disallowance now gives MSME suppliers real leverage. An existing Udyam registration for the services business should be **updated** to add the manufacturing activity and the new NIC codes rather than a second registration taken.
5. **Shops & Establishments.** State/municipal law. An office is registered under the State Shops & Establishments Act; a **manufacturing** premises is normally outside the S&E Act and instead falls under the Factories Act *if* the Factories Act thresholds are met — and if they are not met, many States require registration under their S&E Act or a municipal licence anyway. Register the new premises under the relevant State law within the statutory window (usually 30 days of commencing work).
6. **Factories Act 1948 — almost certainly not applicable.** s.2(m) defines "factory" as premises where **10 or more workers** are working (or were working on any day of the preceding 12 months) and a manufacturing process is carried on **with the aid of power**, or **20 or more workers without the aid of power**. A small assembly workshop with fewer than 10 workers using power (soldering stations, test rigs, hand tools) is **not** a factory and needs no factory licence. Two cautions: (a) the count includes contract and casual workers, not just employees on payroll — a contract assembly crew counts; (b) several States have used s.85 to lower the thresholds or have raised them (some States raised them to 20/40 under labour reform) — **check the State's own notification**. Also note the four Labour Codes (including the Occupational Safety, Health and Working Conditions Code 2020) which, when fully brought into force, replace the Factories Act with a 20-with-power / 40-without-power threshold — even more favourable. Verify commencement status at the time of setup.
7. **Local municipal trade licence.** Required by most municipal corporations for carrying on a trade or manufacture within municipal limits (e.g. BBMP trade licence in Bengaluru, MCGM under the Mumbai Municipal Corporation Act). Cheap (typically ₹500–₹10,000 p.a. depending on city and floor area) but commonly missed, and it is the licence a municipal inspector actually asks for.
8. **Pollution control — Consent to Establish / Consent to Operate.** Per the findings above, **"electrical and electronic item assembling (completely dry process)" is White category**, and White category industries are now exempt from both CTE and CTO — the requirement is reduced to an **intimation to the State Board plus a self-declaration of compliance**. Two important caveats for a *lighting* manufacturer: (i) the exemption depends on the process genuinely being a **dry assembly** process — introduce wet processes (electroplating, anodising, painting/powder-coating, PCB etching, solvent cleaning) and the unit moves into Green/Orange/Red and full consents are back; (ii) the founder must separately handle **E-Waste (Management) Rules 2022 EPR registration** (lighting products, notably LED lamps and luminaires, are in the E-Waste Rules' Schedule) and, if batteries are used, the **Battery Waste Management Rules 2022** — these are distinct from consent and are **not** waived by White category status. (E-waste/EPR is covered in a separate research note in this project, `ewaste_metrology_customs_gst.md`.)
9. **Other manufacturing-specific items to flag (covered in sibling notes):** BIS certification for LED luminaires under the Electronics and IT Goods (Compulsory Registration) Order and/or ISI marking, Legal Metrology packaged commodity declarations, and importer registration if components are imported — see `bis_crs_wpc_eta.md` and `ewaste_metrology_customs_gst.md`.

### Gaps
- Could not verify the **current commencement status of the four Labour Codes / OSH Code 2020** as of September 2026 — this has slipped repeatedly and the report should flag it as "verify at the time."
- Could not confirm whether the CPCB White-category CTE/CTO exemption has been adopted in **every** State board (confirmed for Gujarat; the MoEFCC direction is national but implementation is by State PCBs).
- Municipal trade licence fees are city-specific; the founder's city was not supplied.

---

# PART (B) — ONE ENTITY OR TWO?

## (B1) The payments and lending question — the analysis that drives everything else

### Takeaway
**This is the fact that determines the answer, and it is determinable with a single question: do school fee payments ever land in Modulark Tech Labs' own bank account?** If yes, Modulark is prima facie operating as a **Payment Aggregator** and needs RBI authorisation under the Payment and Settlement Systems Act 2007, with a **₹15 crore net worth at application rising to ₹25 crore by the end of the third financial year** — unattainable for this company. If no — if Modulark merely integrates a licensed PA (Razorpay, Cashfree, PayU) and funds flow merchant→PA escrow→school — then Modulark is a **technology service provider / payment gateway**, needs **no RBI authorisation at all**, and the regulatory contagion argument for splitting the company largely evaporates.

### Cited Findings

**The PA/PG framework is now FINAL, not draft — this is a 2025 change the founder must know about.**
- The **Reserve Bank of India (Regulation of Payment Aggregators) Directions, 2025** were issued on **15 September 2025** (RBI/DPSS/2025-26/141), consolidating and replacing the earlier March 2020 PA/PG Guidelines and their amendments — [Saraf Partners, RBI issues the RBI (Regulation of Payment Aggregators) Directions 2025](https://sarafpartners.com/rbi-issues-the-rbi-regulation-of-payment-aggregators-directions-2025/); [TaxGuru, RBI (Regulation of Payment Aggregators) Directions 2025](https://taxguru.in/rbi/rbi-regulation-payment-aggregators-directions-2025.html); [ANI, RBI issues detailed guidelines for Payment Aggregators, Gateways (16 Sep 2025)](https://www.aninews.in/news/business/rbi-issues-detailed-guidelines-for-payment-aggregators-gateways-to-boost-digital-payment-ecosystem20250916111928/); [DD News](https://ddnews.gov.in/en/rbi-issues-guidelines-for-payment-aggregators-gateways-to-boost-digital-payment-ecosystem/)
- The 2025 Directions bring **offline/physical point-of-sale aggregation (PA-P)** into the same framework as online (PA-O), which the 2020 Guidelines had left out — [The Digital Fifth, RBI Payment Aggregator Framework 2025](https://thedigitalfifth.com/rbi-payment-aggregator-framework-2025-2/); [Juris Corp](https://www.juriscorp.in/rbi-payment-aggregator-compliance/)

**Net worth — confirmed, and the founder's ₹15 crore recollection is right but incomplete.**
- "An entity seeking authorisation to commence or carry on PA business shall have a **minimum net-worth of ₹15 crore at the time of tendering application** for authorisation; and shall attain a **minimum net-worth of ₹25 crore by the end of the third financial year** of grant of authorisation." The minimum net worth must be **maintained on an ongoing basis** — [RBI (Regulation of Payment Aggregators) Directions 2025, as reported by AuthBridge](https://authbridge.com/blog/rbi-payment-aggregator-master-direction-2025/); [TaxGuru](https://taxguru.in/rbi/rbi-regulation-payment-aggregators-directions-2025.html); [Enterslice](https://enterslice.com/learning/rbi-2025-guidelines-for-payment-aggregators/)
- Net worth is computed in line with the Companies Act and applicable accounting standards; **compulsorily convertible preference shares may be included** but **deferred tax assets are excluded** — [AuthBridge](https://authbridge.com/blog/rbi-payment-aggregator-master-direction-2025/)
- Transition deadline for PA-P (offline) entities: apply for authorisation by **31 December 2025**; an entity failing to apply must intimate its bankers and **wind up the PA business by 28 February 2026** — [AuthBridge](https://authbridge.com/blog/rbi-payment-aggregator-master-direction-2025/); [TaxGuru](https://taxguru.in/rbi/rbi-regulation-payment-aggregators-directions-2025.html)
- Banks providing PA services do not need separate authorisation; **non-bank** PAs must be authorised under the PSS Act 2007 — [AuthBridge](https://authbridge.com/blog/rbi-payment-aggregator-master-direction-2025/); [KDP Accountants, RBI Payment Aggregator Licence Guide 2025](https://kdpaccountants.com/blogs/rbi-payment-aggregator-license-india-2025-guide)

**The payment gateway carve-out — the escape hatch, confirmed.**
- "A **Payment Gateway (PG)** is defined as an entity that provides the **technology infrastructure to route and facilitate the payment transaction processing without handling funds**" — [AZB & Partners, Payment Aggregators and Gateways – India's Regulatory Framework](https://www.azbpartners.com/bank/payment-aggregators-and-gateways-indias-regulatory-framework/)
- "**Entities that propose to function as gateways do not require any RBI authorisation.**" PAs handle funds and therefore require direct regulation; **PGs are treated as technology providers** and are only *encouraged* to adhere to the prescribed baseline technology/security recommendations — [AZB & Partners](https://www.azbpartners.com/bank/payment-aggregators-and-gateways-indias-regulatory-framework/); [TaxTMI, RBI's Guideline on Payment Aggregator and Payment Gateway](https://www.taxtmi.com/article/detailed?id=13006)
- "A startup can build a technical payment gateway (no fund holding) **without PA authorisation**, provided it **integrates with an RBI-authorised PA for settlement**. The startup acts as a **technology service provider (TSP)** to the PA." — [IncorpX, Payment Gateway Compliance: RBI & GST Requirements (2026)](https://www.incorpx.io/blog/payment-gateway-compliance-rbi-gst-requirements)
- The defining operational control is the **escrow account**: an authorised non-bank PA must maintain all collected funds in an **escrow account with a scheduled commercial bank** (the PSS Act deems this a "designated payment system" for the purposes of s.23A), with prescribed settlement timelines. Funds collected from customers must **never sit in the merchant's or an intermediary's own operating account** — [AZB & Partners](https://www.azbpartners.com/bank/payment-aggregators-and-gateways-indias-regulatory-framework/); [PhonePe Business, RBI Approved Payment Gateway: Compliance Rules](https://business.phonepe.com/articles/rbi-approved-payment-gateway-compliance-rules-every-merchant-must-know)

### Inferences — apply this to Modulus

**The decisive design rule: "the money must not touch your account."**

There are three architectures Modulus could be running, and they have wildly different consequences:

| Architecture | Does Modulark hold funds? | Regulatory status | Verdict |
|---|---|---|---|
| **(1) Pure integration.** Each school is the merchant of record with Razorpay/Cashfree; Modulus initiates the payment via API; funds go parent → PA escrow → **school's** bank account. Modulark earns a SaaS fee, invoiced separately. | No | **Technology service provider / PG. No RBI authorisation.** | **This is the only viable architecture for Modulark today.** |
| **(2) Modulark as merchant of record / sub-merchant onboarding.** Modulark is the merchant with the PA, collects all schools' fees into its own account, then remits to each school. | **Yes** | **This is payment aggregation.** Onboarding schools as sub-merchants and settling to them is the textbook PA activity. Requires authorisation; ₹15 cr net worth. | **Fatal. Do not do this.** |
| **(3) "Marketplace"/float model.** Fees land with Modulark for T+n days before disbursement — even briefly, even "just for reconciliation." | **Yes** | Same as (2). The 2025 Directions and their predecessor are explicit that funds must sit in an escrow account of an **authorised** entity. A float held in an operating account is exactly what the framework exists to prevent. | **Fatal.** |

**Two additional Modulus-specific traps to flag:**
- **Sub-merchant onboarding is itself a regulated function.** Even without touching money, if Modulark performs merchant KYC and onboarding for the schools on the PA's behalf, it is acting as an outsourced agent of the PA; the 2025 Directions place responsibility on the PA and require contractual control over such agents. This is manageable through the PA contract but should be papered.
- **Escrow-lite alternatives.** If Modulark genuinely needs control over disbursement timing (e.g. to hold back a fee-financing instalment), the compliant route is a **PA's split-settlement / route API or a bank-operated escrow with the school as beneficiary**, not Modulark's current account.

**So: does the payments angle justify a separate entity?**
Honestly — **no, not on its own, and this is where a lot of advice goes wrong.** The payments risk is an *architecture* risk, not an *entity* risk. Putting the SaaS in a separate company does not make an unlawful float lawful, and keeping hardware in the same company does not make a lawful integration unlawful. The correct response to the payments issue is: **fix the fund flow, not the corporate structure.**

Where the payments/lending angle *does* bear on structure is **counterparty diligence and optics**, discussed next.

### Gaps
- **I could not fetch the RBI Directions themselves** (rbi.org.in and the mirrored PDF at fidcindia.org.in were both blocked by the egress proxy). Everything above is from law-firm and consultancy summaries of the 15 September 2025 Directions, which are mutually consistent. **The report-writer should flag that the ₹15 cr / ₹25 cr figures and the PG carve-out language should be verified against the RBI circular text before being relied on for a decision.** The multiple independent corroborations (AuthBridge, TaxGuru, Enterslice, AZB, Saraf Partners) make me reasonably confident, but this is second-hand.
- I could not verify whether the 2025 Directions changed the position on **cross-border PAs (PA-CB)** or introduced any new threshold/turnover-based exemption for small technology providers.
- I found no source addressing **education-sector fee collection specifically** (whether schools' fee aggregation attracts any special treatment). None appears to exist; treat school fees as ordinary merchant collections.

---

## (B2) Lending partner due diligence — the Digital Lending Directions 2025 and the LSP question

### Takeaway
The **RBI (Digital Lending) Directions, 2025** are **final and in force** (effective 8 May 2025, with multi-lender provisions from 1 November 2025 and DLA reporting from 15 June 2025). If Modulus later facilitates fee financing for a bank/NBFC partner, **Modulark will almost certainly be a Lending Service Provider (LSP)**. LSP status does not require Modulark to be licensed, but it makes Modulark a **regulated-entity-accountable outsourcing partner**, subject to the lender's contractual control, audit and diligence — and *that* is where unrelated hardware manufacturing on the same balance sheet becomes a genuine friction point.

### Cited Findings
- The **Reserve Bank of India (Digital Lending) Directions, 2025** came into effect on **8 May 2025**, except: provisions on **multi-lender arrangements effective 1 November 2025**, and **reporting requirements for Digital Lending Apps effective 15 June 2025** — [Argus Partners, RBI (Digital Lending) Directions 2025 – An Overview](https://www.argus-p.com/updates/updates/rbi-digital-lending-directions-2025-an-overview/); [AZB & Partners, Digital Lending Directions 2025 update (PDF)](https://www.azbpartners.com/wp-content/uploads/2025/05/AZB-Update-Digital-Lending-Directions-2025.pdf); [Lawrbit](https://www.lawrbit.com/article/reserve-bank-of-india-digital-lending-directions-2025/)
- The Directions consolidate the previously fragmented digital lending circulars (the September 2022 Digital Lending Guidelines, the 2023 default loss guarantee/FLDG circular and related notifications) into a single code — [Legal 500, The RBI's Digital Lending Directions 2025: A Unified Code for a Fragmented Sector?](https://www.legal500.com/developments/thought-leadership/the-rbis-digital-lending-directions-2025-a-unified-code-for-a-fragmented-sector/)
- **LSP definition:** "an agent of an RE (including another RE) who carries out one or more of the RE's digital lending functions." The updated definition expressly acknowledges that a Regulated Entity may itself act as an LSP of another RE — [Argus Partners](https://www.argus-p.com/updates/updates/rbi-digital-lending-directions-2025-an-overview/); [Hammurabi & Solomon](https://www.hammurabisolomon.in/post/reserve-bank-of-india-digital-lending-directions-2025-brief-overview-analysis)
- LSPs "act as agents of REs and perform digital lending functions such as **customer acquisition, underwriting support, and servicing** on behalf of the REs" — [Synergia Legal, An Overview of the RBI's Digital Lending Directions 2025](https://synergialegal.com/an-overview-of-the-rbis-digital-lending-direction-2025/)
- **REs must enter into contractual agreements with LSPs and conduct periodic review of the LSP against those terms and take steps for any deviations** — [Lexology, New digital lending directions issued by the RBI](https://www.lexology.com/library/detail.aspx?g=2070ef45-a1cf-42ce-9805-ad696a1597ec)
- **The RE remains fully responsible and liable for all acts and omissions of its LSPs, regardless of the extent of delegation** — [Lexology, Rewriting the Rules of Digital Lending](https://www.lexology.com/library/detail.aspx?g=b5bc9efb-1199-41ee-bc2d-4a149573793b); [Finnulate](https://finnulate.ai/blogs/rbi-digital-lending-guidelines)
- REs must **report Digital Lending Apps** of their LSPs to the RBI via the **CIMS portal** — [Lawrbit, RBI Digital Lending Guidelines 2025: Key Rules & CIMS Portal](https://www.lawrbit.com/article/reserve-bank-of-india-digital-lending-directions-2025/)

### Inferences — would the LSP framework apply to Modulark, and does hardware complicate it?

**Would it apply?** Yes, on the likely facts. If Modulus surfaces a fee-financing offer inside the parent-facing app, collects parent data, passes it to a partner NBFC/bank, and services collections — that is customer acquisition and servicing of an RE's digital lending function, performed through a **Digital Lending App (DLA)** that Modulark owns. Modulark becomes an LSP, the Modulus parent app becomes a DLA that the RE must **report to the RBI on the CIMS portal by name**, and the whole arrangement is papered in an RE–LSP agreement with audit rights.

Note Modulark does **not** need any licence of its own to be an LSP. The Directions regulate REs and reach LSPs through the RE's contract and liability. But the practical effect is that **Modulark will be diligenced like a regulated outsourcing vendor**, which typically covers: constitutional documents and objects, shareholding and beneficial ownership, financial statements and net worth, IT and information-security posture (often an audit or a CERT-In empanelled assessment), data localisation and DPDP compliance, grievance redressal and a Nodal Grievance Redress Officer, business continuity, and a right to audit.

**Does unrelated hardware manufacturing complicate that diligence? Yes — in three specific, concrete ways, and this is the honest version rather than hand-waving:**

1. **Financial-statement noise.** The RE's vendor risk team looks at the LSP's audited financials for going-concern and solvency signals. A company whose P&L shows a loss-making manufacturing operation, inventory, capex, working-capital borrowings and possibly a factory lease looks materially riskier than a pure SaaS company with the same SaaS numbers. The hardware losses do not merely fail to help — they **actively depress the metrics the diligence looks at**. A bank's vendor onboarding is a checklist run by a risk team that will not spend time disaggregating segments.
2. **Scope creep in the audit and information-security review.** The RE's right to audit runs against the LSP entity. A hardware operation brings additional premises, additional systems (MES, inventory, procurement), additional contractors and additional physical access points into the audited perimeter. Expect the RE to either widen the audit or demand segregation evidence.
3. **Reputational/liability linkage.** REs are fully liable for their LSPs' acts. A vendor risk committee weighing "does this LSP carry catastrophic tail risk unconnected to lending?" will note that a lithium-battery product recall or fatality claim against the same legal entity could impair the LSP mid-contract or generate adverse press attaching to the bank's named partner.

None of these is a hard legal bar. All three are **friction that costs weeks of onboarding time and reduces Modulark's negotiating leverage** with a lending partner — at exactly the moment (seed/Series A) when leverage matters.

### Gaps
- Could not fetch the RBI Digital Lending Directions 2025 text (rbi.org.in blocked). Effective dates and the LSP definition are corroborated across four independent law-firm summaries, which is good, but the text itself was not read.
- I found **no source** specifically addressing whether an LSP's unrelated business lines are a formal diligence criterion. The three mechanisms above are **inference from how RE vendor-risk frameworks work**, not cited fact, and should be presented as reasoning rather than authority.
- Could not confirm whether the 2025 Directions impose any **minimum net worth or eligibility criteria on LSPs themselves** — my understanding is they do not, but this was not verified.

---

## (B3) Product liability contagion — the strongest argument for separating

### Takeaway
This is the single strongest structural argument, and it is strongest precisely **because of the payments float**. A lithium-battery fire claim is a low-probability, uncapped-severity event; a school payments business is a low-margin, high-trust, cash-adjacent business. Putting an uncapped tail risk in the same legal entity as the trust-dependent business is the classic mismatch that limited liability exists to solve.

### Inferences (reasoning — see sibling note `product_liability_battery.md` for the sourced liability analysis)

**The mechanism.** A private limited company is one pool of assets. A judgment or settlement against Modulark Tech Labs Pvt Ltd arising from a lighting product — a lithium cell in an emergency/rechargeable luminaire venting and causing a fire in a school corridor, say — is enforceable against **every asset of the company**: the SaaS receivables, the cash balance, the IP, the bank accounts. There is no internal partition. "Division," "business unit" and "cost centre" have **no** legal significance for creditors.

**Why the payments angle makes this worse, not better.** Three compounding effects:
- **Float and client money.** Even in the compliant architecture (funds never touch Modulark's account), Modulark will hold *some* cash tied to the schools relationship — security deposits, prepaid balances, refunds in transit, and its own working capital that schools depend on for continuity of service. A creditor's attachment or a freezing order on the company's accounts in the middle of a product-liability suit does not distinguish between "hardware money" and "money the schools depend on."
- **Contractual cross-default and termination.** School contracts and any RE/LSP agreement will contain material-adverse-change, insolvency and reputational-harm termination rights. A serious product liability event in the same entity can trigger termination of the SaaS contracts that are the company's actual value — **the SaaS business can die from a hardware event without a rupee of judgment ever being paid.**
- **Insurance mismatch.** Product liability cover for lithium-battery-containing consumer/commercial electrical goods is expensive, heavily sub-limited, and commonly carries exclusions for recall, for fire originating in cells, and for pure economic loss. Technology E&O/cyber cover for the SaaS side is a different market with different insurers. One entity means one set of policies awkwardly straddling both, and a gap in the hardware cover exposes the SaaS assets directly.

**Additionally — the Consumer Protection Act 2019 angle.** India's product liability regime (Chapter VI, ss. 82–87 CPA 2019) imposes liability on the "product manufacturer" including on a strict basis for manufacturing defects, with the CCPA empowered to order recalls and refunds and to impose penalties. The claimant sues **the manufacturer entity**. If that entity is also the SaaS company, the SaaS company is the defendant of record — including in any class-style consumer complaint before the NCDRC. This is materially different from a scenario where the defendant is a thinly capitalised hardware subsidiary.

**The severity asymmetry, stated plainly:** the hardware business might make ₹2–5 crore of revenue in three years. A single serious fire claim involving a school could be an order of magnitude more, plus recall costs, plus the destruction of the schools-facing brand. **You are risking the whole company to avoid ₹30,000 of incorporation cost and some accounting inconvenience.** That framing is the honest one.

### Gaps
- No Indian case law was located in this research pass quantifying product liability awards for lithium battery fires (the sibling note `product_liability_battery.md` is the place for that). Indian quantum is historically far below US levels, which somewhat softens — but does not remove — the argument; the recall, regulatory and reputational costs are the larger exposure in India.

---

## (B4) The case for ONE entity — loss set-off, cost and simplicity

### Takeaway
The set-off argument is the only genuinely strong one, and it is strong because **India has no group taxation or consolidated-return regime**: losses in a subsidiary cannot be set against profits in a parent. But its value is bounded, quantifiable, and — critically — **recoverable later** in a way that a product liability judgment is not.

### Cited Findings
- Entry 2 of Notification No. 12/2017–Central Tax (Rate) dated 28 June 2017 exempts "**services by way of transfer of a going concern, as a whole or an independent part thereof**" from GST — [CAclubindia, Transfer of Going Concern under GST](https://www.caclubindia.com/articles/transfer-of-going-concern-under-gst-how-gst-exemption-applies-but-itc-reversal-and-documentation-still-matter-55371.asp); [H N A & Co LLP, Implications of GST on transfer of business](https://hnallp.com/a/implications-of-gst-on-transfer-of-business); [Taxo Online](https://taxo.online/latest-research/gst-on-transfer-of-business-as-a-going-concern/)
- Conditions: the transfer must be of a **going concern** — a business that is "live, running and capable of being continued by the purchaser as an independent business" — and must be of the **whole or an independent part**. The transferor issues a **Bill of Supply**, not a tax invoice — [CAclubindia](https://www.caclubindia.com/articles/transfer-of-going-concern-under-gst-how-gst-exemption-applies-but-itc-reversal-and-documentation-still-matter-55371.asp)
- ITC reversal and documentation obligations survive the exemption — the exemption does not make the transaction consequence-free — [CAclubindia](https://www.caclubindia.com/articles/transfer-of-going-concern-under-gst-how-gst-exemption-applies-but-itc-reversal-and-documentation-still-matter-55371.asp)

### Inferences

**1. Loss set-off — quantify it honestly.**
India taxes each company separately. There is **no fiscal unity / group relief / consolidated return** in the Income-tax Act (the only consolidation-like relief is the carry-forward of accumulated losses on an amalgamation or demerger under s.72A, which requires a court/NCLT-sanctioned scheme and conditions). So:

- **One entity:** hardware losses reduce the same taxable income the SaaS profits create. At the 25% domestic rate (companies with turnover under the s.115BAA/turnover threshold; 22% + surcharge + cess ≈ **25.17% effective** under s.115BAA), **every ₹1 of hardware loss absorbed against SaaS profit is worth ~₹0.25 of cash tax saved, in the year it arises.**
- **Two entities:** the hardware company's losses sit in the hardware company as business losses carried forward under s.72 (8 assessment years) and unabsorbed depreciation under s.32(2) (indefinite). They are **not lost** — they shelter the hardware company's own future profits. So the true cost is **not the tax on the losses; it is the time value of deferral** plus the risk that the hardware company never becomes profitable enough to use them.

**Worked numbers.** Suppose hardware loses ₹40 lakh in year 1, ₹60 lakh in year 2, ₹40 lakh in year 3 (₹1.4 crore cumulative), and SaaS is profitable throughout.
- One entity: cash tax saved ≈ ₹1.4 cr × 25.17% ≈ **₹35 lakh**, realised in years 1–3.
- Two entities: ₹35 lakh of shelter deferred to whenever the hardware company turns profitable. If that is year 5–6, the NPV cost at a 15% discount rate is roughly **₹10–15 lakh**. If hardware never becomes profitable, the losses expire and the full **₹35 lakh** is lost.
- **So the realistic economic cost of splitting is on the order of ₹10–35 lakh over five years** on those assumptions. That is real money for a seed-stage company and should not be dismissed — but scale it to the founder's actual numbers.

**A second tax trap that argues *against* the "incorporate later" plan:** **Section 79** of the Income-tax Act restricts carry-forward of losses in a **closely held company** where 51% or more of the voting power changes hands. A hardware subsidiary that raises an equity round and dilutes the founder below the threshold can **lose its accumulated losses entirely** (subject to the eligible-startup relaxation in s.79(2), which permits carry-forward for DPIIT-recognised eligible start-ups within the first ten years where all original shareholders continue to hold their shares — conditions are strict). This cuts both ways but weakens the "the losses will be used later" reassurance.

**2. Annual compliance cost of a second private limited company.** A second Indian private limited company — even a dormant one — costs roughly:

| Item | Annual (₹) |
|---|---|
| Statutory audit (small/dormant company) | 15,000 – 40,000 |
| ROC annual filings: AOC-4 + MGT-7A (+ professional fees) | 8,000 – 20,000 |
| DIR-3 KYC for each director | 1,000 – 2,000 |
| Income tax return + tax audit if applicable | 8,000 – 25,000 |
| Bookkeeping / accounting | 12,000 – 60,000 |
| GST returns (if registered): GSTR-1 + 3B monthly + annual | 12,000 – 36,000 |
| Bank account maintenance, DSCs, misc | 3,000 – 8,000 |
| **Total, genuinely dormant / pre-revenue** | **≈ ₹40,000 – ₹75,000 p.a.** |
| **Total, operating with revenue and GST** | **≈ ₹1,00,000 – ₹2,00,000 p.a.** |

Plus a one-off incorporation cost of roughly **₹8,000 – ₹25,000** (SPICe+ is largely fee-exempt for small authorised capital; the cost is stamp duty, DSCs and professional fees).

Note: a formally **"dormant company" status under s.455** (Form MSC-1) reduces filings (MSC-3 annual return) but is inconsistent with a company that intends to trade soon and does not eliminate audit in all cases. For a company that will start trading within 12–18 months, ordinary status is simpler.

**3. The honest other arguments for one entity.**
- **Shared team and overheads** without inter-company agreements, transfer pricing documentation (domestic TP applies only above the specified-domestic-transaction threshold, but the accounting and arm's-length discipline is still work), cost-sharing invoices and GST on inter-company supplies. Two entities means the CTO working on both must be employed by one and seconded/charged to the other, with GST on the cross-charge.
- **One cap table.** Two companies means two ESOP pools, two sets of shareholder agreements, two board processes, and the awkward question of whether investors get shares in one or both. Investors dislike "sister company" structures with common founders and no holding company — it raises leakage and conflict-of-interest questions. (A **holding company structure** solves this but costs more and introduces its own tax frictions on dividends/exits.)
- **Bandwidth.** A founder running two boards, two audits and two compliance calendars at seed stage is a real cost.

### Gaps
- Could not verify from a primary incometaxindia.gov.in source (egress constraints) the current text of ss. 72, 79, 32(2) and 115BAA, or confirm that no group-taxation regime was introduced in the Finance Act 2025 or 2026. **The absence of group taxation in India is well-established and I am confident, but the report should flag that Finance Act 2026 changes were not checked.**
- The effective corporate tax rate of ~25.17% under s.115BAA is from general knowledge, not verified against a 2026 source. The 25% rate for companies with turnover up to ₹400 crore under the old regime likewise.
- Compliance cost figures are market estimates, not sourced.

---

## (B5) Middle paths — evaluated

### Takeaway
Of the three middle paths, **(ii) incorporate now, keep it effectively dormant until hardware revenue starts** is the best-value option, and **(iii) incorporate later and transfer the business** is the trap — because the cost of a later transfer is dominated not by tax (the GST going-concern exemption and s.50B are manageable) but by **IP and contract assignment friction**, which is exactly what a hardware business accumulates.

### Cited Findings
- **Slump sale — s.50B, Income-tax Act 1961.** A transfer of an undertaking as a going concern for a lump sum consideration without values being assigned to individual assets is a slump sale; capital gains are computed as consideration less the **"net worth"** of the undertaking, with net worth substituted for cost of acquisition. Gains are long-term (taxed at the applicable rate) if the undertaking was held for more than 36 months, short-term otherwise. Since the Finance Act 2021, the consideration is deemed to be the **fair market value** of the undertaking computed under Rule 11UAE, which removed the old planning technique of transferring at book value for nil gain. *(Sourcing note: I was not able to fetch incometaxindia.gov.in; this is from general knowledge and should be verified. See Gaps.)*
- **GST:** transfer of a going concern as a whole or an independent part thereof is **exempt** under Entry 2 of Notification 12/2017–CT(R) dated 28 June 2017 — [CAclubindia](https://www.caclubindia.com/articles/transfer-of-going-concern-under-gst-how-gst-exemption-applies-but-itc-reversal-and-documentation-still-matter-55371.asp); [H N A & Co LLP](https://hnallp.com/a/implications-of-gst-on-transfer-of-business); [TaxTMI, Transfer of Specific Unit as a Going Concern via Slump Sale is Exempt Under GST](https://www.taxtmi.com/article/detailed?id=15407)
- **Stamp duty is a State subject** and applies to instruments including business transfer agreements and IP assignment deeds; rates are set by State schedules — [Stratjuris](https://stratjuris.com/decoding-indian-stamp-duty-requirement/); [JSA, IP right assignments Q&A: India (PDF)](https://www.jsalaw.com/wp-content/uploads/2021/07/Intellectual-property-right-assignments-QAndA-India.pdf)

### Inferences — evaluating each path

**(i) One company with operational ring-fencing.**
*What it is:* separate cost centres in the accounting system, a separate current account for the hardware line, separate P&L reporting, distinct branding and a clear contracting entity, plus product liability insurance.
*Honest assessment:* **This provides zero protection against the risk that matters.** Separate books and a separate bank account have **no** effect on creditor recourse — a judgment creditor of the company reaches every account. This path is worth doing for *management* reasons (you need segment P&L to know whether hardware works, and you need it to do a clean split later) but it must not be sold to the founder as risk mitigation. The one component that *does* mitigate is **product liability insurance** — which is available and should be bought regardless of structure. Estimated cost for a small Indian electrical goods manufacturer: **₹40,000 – ₹2,00,000 p.a. for ₹1–5 crore of cover**, with lithium-battery products attracting loadings, sub-limits or exclusions; get a broker to test the market **before** committing to a battery-containing product.
*Verdict:* necessary but not sufficient. Do it in addition to whatever structural choice is made, never instead of it.

**(ii) Incorporate the second company now, keep it dormant until hardware revenue starts.**
*What it is:* incorporate Modulark Lighting (or similar) via SPICe+ now — ~₹8,000–₹25,000 one-off. Hold the name. Let the R&D and prototyping sit in the existing company initially (capturing the loss set-off) and move the *commercial* activity — contracting with customers, manufacture, sale, warranty — into the new company at the point revenue begins.
*Honest assessment:* **This is the best-value option and it substantially dissolves the loss set-off objection.** The reason: the losses that matter for set-off are the **early R&D and prototyping losses**, which can legitimately be incurred in the existing company (which will need an R&D function anyway) and set off against SaaS profits. The liability that matters arises only **once product is in customers' hands** — which is precisely when the new company takes over. You get the tax shelter in the loss-making phase and the liability firewall in the risk phase. The cost is ~₹40,000–₹75,000 a year of carrying an inactive company plus some care in documenting which entity did what (to avoid a later argument that the R&D was really the new company's, or that the old company was the manufacturer of record).
*Caveat:* the transition still involves moving *something* — at minimum the IP and the supplier relationships. Keep that transition small by (a) filing the patents in the right entity now (see B6), and (b) not signing long-term supplier or customer contracts in the existing company once the decision is made.
*Verdict:* **recommended.**

**(iii) Incorporate later and transfer the business.**
*What it costs:*
- **Income tax — slump sale under s.50B. CONFIRMED.** Capital gains arise on full value of consideration minus the **"net worth"** of the undertaking (net worth substituted for cost of acquisition). Since the Finance Act 2021, "the full value of consideration for a slump sale is the fair market value (FMV) of the capital assets, determined as per **Rule 11UAE**, whichever is higher" — [ClearTax, Slump Sale – Section 50B](https://cleartax.in/s/slump-sale); [CBDT prescribes methodology for computation of FMV in slump sale transactions, Lexology](https://www.lexology.com/library/detail.aspx?g=7459155d-3474-4ffa-a591-36602a50a4a5). Rule 11UAE requires computing **two** values — **FMV1** (FMV of the capital assets transferred) and **FMV2** (FMV of the consideration received) — and taking the **higher** as the full value of consideration — [TaxTMI, Rule 11UAE](https://www.taxtmi.com/acts?id=39958); [BCAS, Taxation of slump sale: Sec 50B and Rule 11UAE (PDF)](https://bcasonline.org/wp-content/uploads/2023/04/Taxation-of-slump-sale-Sec-50B-and-Rule-11UAE.pdf). The amendment was introduced expressly "to prevent undervaluation of slump sales — where parties would agree on a low lump sum consideration to minimise capital gains tax. **Now, even if the actual consideration is below FMV, the tax is computed on the FMV**" — [Patron Accounting, Slump Sale Tax Rules: Section 50B Guide (2026)](https://www.patronaccounting.com/blog/slump-sale-tax-rules-section-50b). **So you cannot transfer at book value to engineer nil gain — this planning route was closed in 2021.** If the hardware business has by then developed valuable IP and customer contracts, the FMV can materially exceed net worth (which excludes self-generated intangibles), producing a **real cash tax charge on a transaction that moves no cash**. This is the principal tax reason the cheapest time to split is early.
- **GST — manageable.** Transfer of a going concern as a whole or as an independent part is **exempt** (Entry 2, Notification 12/2017-CT(R)). But: it must genuinely be a going concern transfer (a bare sale of assets and IP is **not** and attracts GST at the relevant rates on each asset); ITC reversal and Form ITC-02 transfer mechanics apply; and documentation must be right.
- **Stamp duty — State-specific and potentially significant.** A Business Transfer Agreement is a conveyance in several States, attracting ad valorem duty. Maharashtra, for instance, charges conveyance duty on a BTA (historically capped in some contexts, but the position varies and has changed); Karnataka and Delhi differ. **Budget 0.1%–5% of consideration depending on the State and whether immovable property is included.** With immovable property in the mix (a workshop lease or freehold), full conveyance rates apply to that component.
- **IP and contract assignment — the real cost, and the one people underestimate.** Patents require executed assignment deeds, stamp duty, and recordal at the Patent Office (below). Trade marks require Form TM-P assignment recordal. Copyright in software and firmware requires written assignment (s.19 Copyright Act) — and note **s.19(4)**: if the assignee does not exercise the rights within one year the assignment may be deemed to lapse, and s.19(5)-(6) imply a five-year term and territorial limit absent express provision — so the deed must be drafted properly. Customer contracts, supplier contracts, distributor agreements and the workshop lease each require **novation or assignment, most of which need counterparty consent**. Employment contracts require either novation or fresh employment with continuity-of-service arrangements (and PF/ESI transfers). BIS/CRS registrations, e-waste EPR registration and Legal Metrology registrations are **entity-specific and generally have to be re-obtained, not transferred** — for a certified lighting product this alone can be a 2–4 month delay and a repeat of testing fees.
- **A full NCLT demerger** (s.230–232) is the clean alternative that preserves tax neutrality (s.2(19AA)/s.47(vib)) and carries losses across under s.72A(4), but costs **₹10–30 lakh in professional fees and 9–18 months** with NCLT, creditor and regulator approvals. It is not a seed-stage tool.

*Verdict:* **avoid.** The dictum the founder should take away is correct: **the cheapest time to split is before there is anything to split.** A split today costs an incorporation fee. A split in three years costs a slump-sale tax charge, stamp duty, re-certification of every product approval, and consent from every counterparty.

**Weighing that against loss set-off:** path (ii) is precisely the resolution of this tension. It captures the set-off in the period when losses are largest and liability is smallest, and it avoids the transfer cost because there is almost nothing to transfer at the moment of handover.

### Gaps
- **Section 50B and Rule 11UAE were not verified against a primary source** (incometaxindia.gov.in not fetched). The Finance Act 2021 FMV amendment is well known but the report should verify before quoting.
- **Stamp duty on Business Transfer Agreements by State could not be sourced to a schedule.** The 0.1%–5% range is indicative only and the founder's State was not supplied. This is a genuine gap and should be flagged as "get a State-specific opinion."
- Demerger professional fee and timeline figures are market estimates, not sourced.

---

## (B6) IP ownership — which entity should be the patent applicant?

### Takeaway
**File any lighting-hardware patent in the new hardware entity from day one** (incorporating it now specifically so that it can be the applicant). Assigning a patent later is not ruinously expensive in filing-fee terms, but it is **mandatory to record**, it attracts **ad valorem State stamp duty on the assignment deed**, and — in the specific case of a *later* transfer for value — it feeds directly into the slump-sale FMV computation. The asymmetry is stark: naming the right applicant now costs ₹0; fixing it later costs money, time and tax.

### Cited Findings
- **Recordal is mandatory:** "The recordal of patent assignments with the Controller is mandatory (**section 69(2), Patents Act**)" — [JSA, Intellectual property right assignments Q&A: India (PDF)](https://www.jsalaw.com/wp-content/uploads/2021/07/Intellectual-property-right-assignments-QAndA-India.pdf)
- The executed deed of assignment plus evidence of title must be registered with the Indian Patent Office by filing **Form 16** with the CGPDTM; **two copies of the assignment instrument certified as true copies** must accompany the application (**Rule 91, Patents Rules 2003**) — [JSA](https://www.jsalaw.com/wp-content/uploads/2021/07/Intellectual-property-right-assignments-QAndA-India.pdf)
- "Any post Indian filing date assignment requires a **notarised original deed with stamp duty paid**, and **Form 6 or 16** to be filed" — [C&C IP, Patents India – Formal Requirements](https://www.candcip.com/formal-requirements)
- **Stamp duty on the assignment deed is levied per the State schedule**, typically **0.5%–5% of the consideration value**, and the Assignor and Assignee must check the rate for their State — [S.S. Rana & Co., Patent Assignment Agreement India](https://ssrana.in/ip-laws/patents/patent-assignment-cost-india-inr-1600/); [Stratjuris, Decoding Indian Stamp Duty Requirement for IP instruments](https://stratjuris.com/decoding-indian-stamp-duty-requirement/)
- The Patents Act and Rules **do not prescribe a timeframe** for recordal nor specify which party bears the cost — [JSA](https://www.jsalaw.com/wp-content/uploads/2021/07/Intellectual-property-right-assignments-QAndA-India.pdf)

### Inferences — the concrete answer

**What a later assignment actually costs (per patent/application):**

| Component | Cost | Notes |
|---|---|---|
| Official fee, **Form 6** (change of applicant before grant, s.20(1)) | Small two-tier official fee on the same natural-person/startup/MSME vs. large-entity scale — **exact figure not verified; see Gaps** | Used **pre-grant** to change the applicant. This is the cheap, clean route. |
| Official fee, **Form 16** (registration of title / assignment, Rule 91) | **₹1,600 (natural person / startup / MSME) · ₹4,000 (small entity) · ₹8,000 (large entity)** — [Intepat, Patent Cost in India (2026): Official Fees](https://www.intepat.com/blog/patent-fees-cost-india); [IncorpX, Patent Filing Fees in India 2026](https://www.incorpx.io/blog/patent-filing-fees-india-2026-startup-vs-company) | Used for recordal of assignment / registration of title. Reduced-fee status requires **Form 28** with supporting documents proving startup/MSME eligibility. |
| Patent agent / attorney fees | **₹10,000 – ₹30,000 per patent** | Drafting the deed, executing, notarising, filing, responding to objections |
| **Stamp duty on the assignment deed** | **0.5% – 5% of consideration, State-dependent** | **This is the variable that can explode.** If the patent is assigned for a nominal ₹100, duty is trivial — but a nominal-consideration assignment between related parties invites both a stamp authority challenge (adjudication at market value) and an income-tax challenge under s.50B/s.56(2)(x). If the patent is genuinely valuable by then, duty is on that value. |
| Notarisation, certified copies, courier | ₹2,000 – ₹5,000 | |
| **Total per patent, nominal consideration, pre-grant** | **≈ ₹15,000 – ₹40,000** | |
| **Total per patent, valuable patent, post-grant, real consideration** | **₹15,000 – ₹40,000 + ad valorem stamp duty + capital gains in the transferor** | Can be lakhs |

**And the non-monetary costs, which are worse:**
- **Priority and prosecution disruption.** A change of applicant mid-prosecution in India, and correspondingly in every foreign jurisdiction where a PCT national phase or Paris Convention application has been filed, multiplies the work: each jurisdiction has its own recordal form, fee and evidentiary requirement. **A single Indian patent with a PCT filing and three national phases turns a ₹20,000 problem into a ₹2–4 lakh problem.**
- **Chain-of-title defects kill deals.** The most common IP finding in Indian startup diligence is a broken chain of title. An unrecorded or defectively stamped assignment is a **condition precedent** in an investment or acquisition. Under s.69(5) of the Patents Act, a document not registered is generally **not admissible in evidence** as proof of title in proceedings (subject to the Controller's/court's direction) — so an unrecorded assignment is not merely untidy, it is potentially unenforceable when it matters.
- **Inventor assignments are a separate, independent requirement.** Whichever company is the applicant, the **inventors must assign to it** (Form 1 proof of right, or a separate assignment / employment agreement with an express present assignment of inventions). Make sure every engineer's employment contract contains a present-tense assignment ("hereby assigns"), not a promise to assign.

**Concrete recommendation on applicant entity — split by subject matter, not by convenience:**

| Subject matter | Applicant |
|---|---|
| Lighting hardware: luminaire mechanical design, thermal management, driver topology, optics, battery/charging circuitry, sensor integration | **New hardware company (Modulark Lighting Pvt Ltd or similar) — incorporate it now precisely so it can be the applicant on the first filing.** |
| Lighting **control software / firmware algorithms** (where patentable notwithstanding s.3(k) — see sibling note `patents_section_3k.md`) | **Judgement call.** Default to the **hardware company** if the invention is claimed as a device or a device-implemented method — keeping the lighting patent family in one entity avoids a split family that is impossible to license or sell cleanly. Licence back to the SaaS company if needed. |
| Modulus SaaS / school management / payments-adjacent inventions | **Existing company (Modulark Tech Labs Pvt Ltd).** |
| Drone (Modulark Aero) | Out of scope of this note, but apply the same logic: if Aero is ever to be separated, file in the entity that will own it. If Aero stays with the parent, file in the parent. **Do not file "in the parent for now, sort it out later."** |
| Trade marks | File the house mark **MODULARK** in the existing company and **licence** it to the hardware company under a registered user / permitted use agreement (s.48–s.49 Trade Marks Act) — a brand is the one asset that should stay centralised. File product-specific marks in the owning entity. |

**If a patent must be filed before the new company exists** (because a priority deadline or a public disclosure deadline bites): file in the existing company, but (a) record in the board minutes that the filing is made on behalf of a to-be-incorporated hardware entity, (b) incorporate within weeks, and (c) execute and record a **Form 6 change of applicant pre-grant** immediately — Form 6 pre-grant is far cheaper and cleaner than a post-grant Form 16 assignment recordal. **Do not let a filing sit in the wrong entity through to grant.**

### Gaps
- **Form 16 fees are now sourced (₹1,600 / ₹4,000 / ₹8,000 by entity category), but the Form 6 fee was not found** — the search results explicitly noted "Form 6 was not specifically mentioned." Check the First Schedule to the Patents Rules (as amended by the Patents (Amendment) Rules 2024) at ipindia.gov.in.
- **Source conflict to flag:** one secondary source described Form 16 as the **post-grant opposition** form at ₹2,400/₹6,000/₹12,000 — [Intepat](https://www.intepat.com/blog/patent-fees-cost-india). This appears to be an error in that source (post-grant opposition is Form 7 under s.25(2); Form 16 is the application for registration of title/interest under s.69 and Rule 91). The JSA and C&C IP sources consistently identify Form 16 as the title-recordal form, which is the reading adopted here. **The report-writer should have the founder's patent agent confirm the correct form number and fee at the point of filing.**
- The point about s.69(5) inadmissibility is from general knowledge of the Patents Act and was not verified against the statutory text in this pass.
- State-specific stamp duty rates for IP assignment deeds could not be tabulated; the 0.5%–5% range is as reported by S.S. Rana and Stratjuris.

---

## (B7) RECOMMENDATION

### Takeaway
**Two entities — but sequenced.** Amend the objects clause of the existing company now (it is cheap and the drone line probably needs it already), incorporate the hardware company now, run early R&D inside the existing company to capture the loss set-off, and move all customer-facing hardware activity into the new company before the first unit ships. **File lighting hardware patents in the new company from the first filing.**

### The reasoning, stated as a decision rather than a list

**1. Fix the MOA regardless. This is not a close call.**
Whatever is decided on structure, the existing company's objects clause must be checked today and almost certainly amended. Cost ~₹20,000, elapsed 2–3 weeks on a shorter-notice EGM. If the MOA is software-only, the **drone line is already ultra vires**, which means the company is already exposed and the amendment is overdue rather than anticipatory. Draft it broadly in one pass: software and SaaS; design, development and manufacture of electrical, electronic and electro-mechanical goods including lighting products and luminaires; unmanned aerial systems; trading, import and export; and R&D. Amending twice is wasteful.

**2. The payments question is architectural, not structural — and it is urgent.**
Before anything else, answer this one question: **do school fee payments ever settle into a Modulark Tech Labs bank account, even for an hour?** If yes, stop and fix it, because Modulark is then conducting unauthorised payment aggregation, and the authorisation it would need carries a ₹15 crore net-worth-at-application / ₹25 crore-by-year-three requirement it cannot meet. If no — if Modulark integrates a licensed PA and funds go parent → PA escrow → school — Modulark is a technology provider and needs no RBI authorisation. **Splitting the company does not fix an unlawful fund flow and keeping it whole does not break a lawful one.** Do not let the entity question distract from the architecture question.

**3. The decisive argument for splitting is product liability, and it is decisive because of what it puts at risk, not what it costs.**
A lithium-battery fire claim against the lighting business reaches every asset of Modulark Tech Labs: the SaaS cash, the receivables, the IP, the bank accounts the schools depend on. Worse, it reaches the *contracts* — the MAC and reputational-harm termination rights in school agreements and in any future RE/LSP agreement mean a serious hardware event can destroy the SaaS business without a rupee of judgment ever being enforced. That is an uncapped, low-probability, existential risk placed voluntarily inside a trust-dependent, cash-adjacent business. **The whole point of the limited liability company is to not do this.**

The lending angle reinforces it without being decisive on its own: Modulark will be an LSP (not licensed, but diligenced like a regulated vendor), and a loss-making manufacturing operation on the LSP's balance sheet adds financial noise, widens the audit perimeter and introduces tail risk that a bank's vendor risk committee will price in weeks of delay and reduced leverage.

**4. The strongest counter-argument — loss set-off — is real but bounded, and largely solvable by sequencing.**
India has no group taxation, so hardware losses in a subsidiary cannot shelter SaaS profits. On plausible numbers (₹1.4 crore of cumulative hardware losses over three years) the economic cost of separating is roughly **₹10–35 lakh over five years** — the deferral cost if the hardware company eventually profits, the full ~₹35 lakh if it never does. That is not nothing. But **the losses that are largest and earliest are R&D and prototyping losses, and those can legitimately sit in the existing company**, which needs an R&D function anyway. The liability arises only when product reaches customers. Sequencing therefore captures most of the tax benefit and all of the liability protection.

**5. And the cheapest time to split is now, because there is nothing to split.**
Today the hardware business is an idea, a few prototypes and some drawings. Splitting costs an incorporation fee of ₹8,000–₹25,000. In three years the same split is a slump sale under s.50B at deemed fair market value (so a real cash tax charge on a transaction that moves no cash), ad valorem stamp duty on a Business Transfer Agreement, consent from every customer, supplier and landlord, re-execution and re-recordal of every patent and trade mark in every jurisdiction, and — the one that really hurts a lighting business — **re-obtaining entity-specific BIS/CRS registrations, e-waste EPR registration and Legal Metrology registrations, which are not transferable and can cost 2–4 months of lost selling time**. An NCLT demerger, the clean alternative, is ₹10–30 lakh and 9–18 months. None of this is a seed-stage cost.

**6. Therefore: the specific plan.**

| When | Action | Cost |
|---|---|---|
| **Week 1** | Download the MOA from MCA21 VPD and read Clause III. Answer the payments-flow question. | ₹100 |
| **Weeks 1–3** | Amend the objects clause of Modulark Tech Labs by special resolution (shorter-notice EGM) + MGT-14. Draft broadly: software, hardware manufacture, UAS, trading. | ~₹20,000 |
| **Weeks 1–3, in parallel** | Incorporate **Modulark Lighting Pvt Ltd** (or chosen name) via SPICe+ with a manufacturing-appropriate objects clause and NIC code from the start. Same founder shareholding as the parent, or a holding structure if investors are imminent. | ₹8,000–₹25,000 |
| **Weeks 1–3** | Get a broker to test the **product liability insurance** market for a lithium-battery-containing luminaire **before** committing to the product design. If cover is unobtainable or heavily excluded, that is itself a design input. | Quote only |
| **Months 1–12 (R&D phase)** | Run R&D, prototyping and design inside **Modulark Tech Labs** to capture loss set-off against SaaS profits. Keep the new company dormant (~₹40,000–₹75,000 p.a. carrying cost). Do **not** sign long-term supplier, customer or lease commitments in the parent. | Carrying cost |
| **From the first patent filing** | File lighting hardware patents with **Modulark Lighting** as applicant. If a deadline forces a parent filing, do a **Form 6 pre-grant change of applicant** within weeks — never let it run to grant. | ₹0 extra if done right |
| **Before the first commercial unit ships** | Activate the hardware company: it becomes the manufacturer of record, contracting party, warrantor, BIS/CRS registrant, EPR registrant and insured. All customer-facing hardware activity sits there. | — |

**7. Patents — the one-line answer the founder asked for.**
**Incorporate the hardware company now, and put it on the first lighting patent application as the applicant.** Naming the right applicant today costs nothing. Moving a granted patent family later costs ₹15,000–₹40,000 per patent in India plus ad valorem stamp duty plus equivalent recordals in every foreign jurisdiction plus a chain-of-title finding in every future diligence — and if the patent is valuable by then, a capital gains charge on the transfer. Keep the **MODULARK house trade mark in the parent** and licence it down; keep SaaS and payments inventions in the parent; put everything lighting-hardware in the hardware company.

### Gaps in the recommendation
- The recommendation assumes the founder's SaaS business is **currently profitable or close to it** (otherwise the loss set-off argument has no force at all and the case for splitting becomes overwhelming and unqualified). This was not stated in the brief.
- It assumes no existing investor whose shareholders' agreement contains a **non-compete, exclusivity or "no new business" covenant** or a reserved matter requiring consent for incorporating a subsidiary or commencing a new line of business. **Check the SHA/SSA before incorporating anything.** This was not verifiable from the materials available.
- It assumes the hardware company can be incorporated with the same shareholding without triggering a **related-party / conflict** issue under s.188 or a corporate-opportunity objection from existing investors. Where investors exist, a **holding company structure or a subsidiary of the parent** may be preferable to a sister company — but a subsidiary re-imports some of the contagion risk (the parent's shares in the subsidiary are an asset, though parent liability for the subsidiary's torts is limited absent lifting the veil). This trade-off was not researched in depth and should be flagged for the founder's CS/CA.
