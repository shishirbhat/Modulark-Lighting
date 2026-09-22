# Indian Patent Law: Section 3(k) and a Closed-Loop Sensing-and-Luminaire Control System

**Research constraint flagged up front:** the org egress proxy on this machine blocked every primary-source domain I tried — `indiankanoon.org`, `ipindia.gov.in`, `wipo.int`, `patents.google.com`, `spicyip.com`, `bananaip.com`, `remfry.com`, `lexology.com`, `pib.gov.in`, `iiprd.com` (403 `connect_rejected`, organization policy). All full-text fetching failed. Everything below rests on web-search result summaries plus clearly-labelled legal reasoning. **I could not verify a single judgment paragraph verbatim, and I could not read the claim text of any granted Indian patent.** Where I give a quote-like formulation it is a close paraphrase and is labelled as such. Anything money- or date-specific must be re-checked against the First Schedule to the Patents Rules on ipindia.gov.in before it is relied on. I have marked the weakest items in the Gaps sections rather than smoothing them over.

---

## Q1. Current text and judicial interpretation of Section 3(k); the settled test; the "novel hardware" requirement

### Takeaway
Section 3(k) (inserted by the Patents (Amendment) Act 2002) excludes "a mathematical or business method or a computer programme per se or algorithms." The settled judicial test since *Ferid Allani* (Delhi HC 2019) is **technical effect / technical contribution**: the word *per se* is read as excluding only claims to the programme as such, so a computer-implemented invention that produces a technical effect outside the abstraction is patentable. The Delhi High Court has repeatedly held that **novel hardware is NOT required** — an examiner who demands it is applying a standard with no statutory basis, and the 2025 CRI Guidelines now say so expressly. But the corollary is harsh: where the only inventive contribution is the abstract step or the algorithm itself, refusal follows (*OpenTV*, *Blackberry*).

### Cited Findings
- Section 3(k) excludes "a mathematical or business method or a computer programme per se or algorithms" from being an "invention"; the provision "aims to prevent the patenting of abstract ideas, algorithms, and business methods without technical application" — [Section 3(m)/Section 3 discussion, search summary of indiankanoon Patents Act text](https://indiankanoon.org/doc/874310/) (text of the Act; page itself not fetchable from this machine).
- ***Ferid Allani v. Union of India***, Delhi HC, **12 December 2019** (Justice Prathiba M. Singh), W.P.(C) 7/2014: "reshaped the understanding of Section 3(k) … The case clarified that software by itself could be patented, provided that it had some 'technical effect'." — [Metayage, Decoding the Ferid Allani case](https://www.metayage.com/blogs/decoding-the-ferid-allani-case); [Invest India](https://www.investindia.gov.in/team-india-blogs/evolution-patentability-computer-program-based-innovations-india-through-ferid). *Close paraphrase of the ratio (NOT verified verbatim): the bar is on computer programmes "per se", not on all inventions based on computer programmes; in a digital age where most inventions are computer-implemented, a blanket bar would be retrograde; the test is whether the invention demonstrates a "technical effect" or "technical contribution."*
- ***Microsoft Technology Licensing LLC v. Assistant Controller of Patents and Designs***, Delhi HC 2023: Microsoft argued the invention "relates to a technical process and solves a technical problem of securing data accessed on a network, and the court reaffirmed the importance of properly understanding and applying technical advancement and technical effect in determining patentability of CRIs." — [SpicyIP, Microsoft v. Asst. Controller](https://spicyip.com/2023/03/microsoft-v-asst-controller-of-patents-and-designs-revisting-the-cri-guidelines-and-ferid-allani.html) (not fetchable; title/summary only). A second Microsoft appeal in the same period concerned "Reversible 2-Dimensional Pre-/Post-Filtering For Lapped Biorthogonal Transform."
- ***OpenTV Inc. v. The Controller of Patents and Designs***, Delhi HC, **11 May 2023**: "Business method claims are barred absolutely, with no technical effect analysis. The Delhi High Court held that the bar in India over business methods is absolute and not qualified." — [Asia IP, The Delhi High Court's Decision in OpenTV](https://asiaiplaw.com/article/india-the-delhi-high-courts-decision-in-opentv); [Kan & Krishme analysis of CRI 2025 key judgements](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/).
- ***Raytheon Company v. Controller General of Patents and Designs***, Delhi HC, **15 September 2023**: "Novel hardware is not required for patent protection. Cases like Raytheon and Microsoft further confirm that no new hardware is required." — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/). *(Date per that source; I could not confirm the neutral citation.)*
- ***Ab Initio Technology LLC v. Assistant Controller of Patents and Designs***, Delhi HC, **30 July 2024**: "upheld a patent for software that boosted processor efficiency, ruling it delivered a technical effect." — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/).
- ***Blackberry Limited v. Assistant Controller of Patents and Designs***, Delhi HC, **30 August 2024**: "For algorithms, the inventive feature must be the implementation." Judgments "reinforce that algorithms and software may qualify, but only when they go beyond abstract ideas and deliver real world technical advancements." — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/); case listing at [indiankanoon 50904559](https://indiankanoon.org/doc/50904559/) (blocked).
- ***Lava International Ltd. v. Telefonaktiebolaget LM Ericsson***, Delhi HC 2024: "Lava challenged that Ericsson's inventions fell under Section 3(k), with the court citing relevant portions from Microsoft, Ferid Allani, and other recent orders along with the revised CRI guidelines, 2017." The court set out a consolidated set of Section 3(k) principles. — [BananaIP, Section 3(k) principles – Ericsson vs. Lava Part 2](https://www.bananaip.com/intellepedia/section-3k-principles-ericsson-vs-lava-part-2/) (blocked; title + search summary only).
- ***Robert Bosch Limited v. Deputy Controller of Patents and Designs***, **Madras High Court, CMA(PT)/1/2024, Justice Senthilkumar Ramamoorthy, 25 March 2025** — see Q5; directly analogous closed-loop control method. — [De Penning & De Penning](https://depenning.com/blog/robert-bosch-limited-v-deputy-controller-of-patents-and-designs-interpretation-of-sec-3m/); [Anand & Anand, Patents Rewind](https://patentsrewind.wordpress.com/2025/05/06/madras-high-court-clarifies-the-scope-of-section-3m/); [Selvam & Selvam](https://selvams.com/insights/madras-high-court-holds-that-not-all-inventions-must-yield-physical-products-to-be-patentable/).

### Inferences
- The operative question an Indian examiner/Controller now asks is, in substance, a two-part one: (i) **strip the claim to what is actually new over the prior art** — if the novelty resides only in a calculation, a rule, or a set of instructions, 3(k) bites; (ii) if the new matter causes an effect in the physical world or in the functioning of a machine, 3(k) does not bite. This is functionally close to the EPO's "technical contribution / Comvik" approach, but Indian courts have not formally adopted Comvik and it is unsafe to cite EPO doctrine as if binding.
- *Blackberry* is the case the applicant here should fear most: it is authority for refusing claims where the "invention" reduces to steps of processing data, even when nominally recited as performed by a device.
- *OpenTV*'s absolute business-method bar matters if the drafter is tempted to add claims about energy-billing, subscription tiers, or building-management service delivery. **Do not.** Those claims are unqualifiedly dead and can taint the file.

### Gaps
- I could not obtain the numbered paragraphs of *Ferid Allani*, *Microsoft*, *Raytheon*, *OpenTV*, *Blackberry*, *Ab Initio* or *Lava*. A drafting opinion for filing should quote *Lava* paras on the consolidated 3(k) principles and *Ferid Allani* paras 10–12 verbatim; those need to be pulled from indiankanoon or the Delhi HC site on an unrestricted connection.
- Neutral citations (e.g. `2023:DHC:____`) could not be confirmed for any of these; do not reproduce a citation number without checking.
- Whether the Supreme Court has said anything on 3(k) (I found nothing suggesting it has; treat Delhi HC as the controlling authority in practice, with Madras HC persuasive).

---

## Q2. Status and legal weight of the CRI Guidelines (2017 → 2025)

### Takeaway
The 2017 CRI Guidelines have been superseded. A **draft CRI Guidelines 2025 issued 25 March 2025**, a **Version 2.0 draft in June 2025**, and a **revised/final version released by CGPDTM in 2025 (reported July 2025)**. The 2025 Guidelines expressly **reject the "novel hardware" requirement as "a higher standard which lacks any basis in law"**, add a jurisprudence chapter, and set out a **step-wise Section 3(k) assessment** with a large annexure of worked examples. Guidelines are **administrative instructions binding on examiners but not on courts** — they cannot add to or subtract from Section 3(k), and courts have struck down guideline-derived tests before. **Flag to the client: this area moved in 2025 and the exact final-version date/text should be re-verified.**

### Cited Findings
- "The Office of the Controller General of Patents, Designs & Trade Marks (CGPDTM) has released the Revised Guidelines for Examination of Computer Related Inventions (CRIs), 2025 … aim to enhance clarity, consistency, and predictability … while aligning India's patenting practices with global standards." — [PIB press release PRID 2149719](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2149719) (blocked; search summary).
- Timeline: "The Indian Patent Office released the Draft Guidelines … in March 2025, followed by a revised draft in June and a final version in July 2025." — [PIB summary](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2149719); draft date of **25 March 2025** — [AIPPI, Decoding CRI Guidelines 2025](https://www.aippi.org/news/decoding-cri-guidelines-2025/).
- **Novel hardware expressly rejected:** "The new guidelines explicitly state that novel hardware is not required for patentability and reject this as 'a higher standard which lacks any basis in law'." — [SFLC.in, Say No to Software Patents – I: The 2025 CRI Guidelines](https://sflc.in/say-no-to-software-patents-i-the-2025-cri-guidelines/); [Intepat, CRI Guidelines 2025 India](https://www.intepat.com/blog/cri-guidelines-2025-patent-india-3k); [BRB Legal](https://www.brb-legal.com/post/2025-cri-guidelines).
- **Step-wise test** as reported: "Is it a business method? If yes → automatic rejection under Section 3(k). Is it only an algorithm or program? If novelty lies only in abstract steps or code, objection under 3(k). Is there a technical effect? If the invention shows a measurable system-level impact (e.g., reduced latency, improved throughput, better memory utilization), it may pass." — [Intepat](https://www.intepat.com/blog/cri-guidelines-2025-patent-india-3k); [De Penning, Draft CRI Guidelines](https://depenning.com/blog/draft-cri-guidelines/).
- Contents: "Inclusion of a detailed chapter on jurisprudence elaborating the nuances of CRIs; Step-wise assessment methodology for Section 3(k) … supported by multiple examples." Covers AI, ML, deep learning, cloud, quantum and blockchain. — [PIB summary](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2149719); [K&S Partners](https://kandspartners.com/indian-patent-office-publishes-guidelines-for-examination-of-computer-related-inventions/).
- Size/structure: "Version 2.0 extends to 62 pages, with an Annexure I of 73 pages offering detailed, non-exhaustive examples that illustrate what is and isn't patentable under Section 3(k) exclusions." — [BananaIP, Draft CRI Guidelines 2025 Version 2.0](https://www.bananaip.com/intellepedia/cri-guidelines-2025-version-2/) (blocked; search summary).
- Mathematical-method treatment: "the mere expression of an intellectual exercise, such as a method of calculation, the formulation of equations and the like … Brent's method in numerical analysis to find the root or the Adams' method of solving differential equations would be excluded." But "mathematical methods per se remain excluded, [while] their application in technical systems may be patentable," and the exclusion "may not apply to inventions that recite mathematical formulae in systems for encoding, reducing noise in communications/electrical/electronic systems or encrypting/decrypting electronic communications." — [Lexology, Analyzing the Draft CRI Guidelines 2025 – Part 5](https://www.lexology.com/library/detail.aspx?g=b35781d8-4ffe-4a05-9257-ff752fc40cdb); [LKS, Decoding the 'Algorithm' exclusion](https://www.lkslaw.com/insights/articles/decoding-the-algorithm-exclusion-a-closer-look-at-draft-cri-guidelines-2025).
- Patentability-conferring categories named in the 2025 Guidelines: "boosting internal system efficiency or functionality, **governing external devices or physical processes**, and concrete technical implementations can lead CRIs towards patentability." — [Lexology Part 5](https://www.lexology.com/library/detail.aspx?g=b35781d8-4ffe-4a05-9257-ff752fc40cdb); [Mondaq, A Detailed Analysis Of India's New CRI Guidelines, 2025](https://www.mondaq.com/india/patent/1663246/a-detailed-analysis-of-indias-new-cri-guidelines-2025).
- Historical note on the hardware requirement: "a significant shift from the 2016 CRI Guidelines, which had required novel hardware, to the current approach that emphasizes technical contribution and technical effect instead." — [Intepat](https://www.intepat.com/blog/cri-guidelines-2025-patent-india-3k).

### Inferences
- **"Governing external devices or physical processes" is, almost word for word, what this invention does.** That phrase in the 2025 Guidelines is the single most useful sentence in the Indian examination materials for this applicant, and should be quoted back at the examiner in any FER response.
- Guidelines have no statutory force. The 2016 Guidelines' three-step "novel hardware" test was abandoned in 2017 precisely because it had no basis in the Act, and the courts (Raytheon, Microsoft) then had to repeat that point because examiners kept applying it anyway. Expect first-instance examiners to lag the 2025 text — an FER demanding novel hardware is still a realistic outcome and is answerable by citing the 2025 Guidelines plus *Raytheon*.
- SFLC.in — a digital-rights organisation critical of software patents — characterises the 2025 Guidelines as opening the door wider. Its framing ("Say No to Software Patents") is advocacy, but its factual reporting of the novel-hardware rejection matches the law-firm sources, so that specific fact is well-corroborated.

### Gaps
- **Exact date and final status of the 2025 CRI Guidelines is not nailed down.** Sources say draft 25 March 2025, v2.0 June 2025, final July 2025; the PIB release exists but I could not read it. One source ([Mondaq](https://www.mondaq.com/india/patent/1663246/a-detailed-analysis-of-indias-new-cri-guidelines-2025)) calls them "India's New CRI Guidelines, 2025" as if final. **Verify before advising.** There is also a possibility of further revision after September 2025 that my sources do not cover.
- I could not read the Annexure I examples. Whether any worked example concerns a sensor-driven actuator/control loop is unknown and is the most valuable thing to check — if one exists, it is close to dispositive for drafting.
- The precise wording of the step-wise test is second-hand from commentary, not from the Guidelines themselves.

---

## Q3. How claims are actually drafted to survive 3(k) for a sensing-and-actuating control system

### Takeaway
The winning architecture is a **system/apparatus claim whose independent claim recites physical structure (sensor, luminaire drivers, wireless transceiver, controller) and whose functional limitations are expressed as a chain running from a measured physical quantity to a physical change in the world (light actually emitted)**, paired with a **method-of-operating claim tied to that hardware**. Kill the "computer programme product" and "computer-readable medium" claims — in India they are refused on sight. Avoid pure means-plus-function, which India treats far less generously than the US. I could not retrieve the actual claim text of granted Indian lighting/HVAC control patents (databases blocked), so the drafting technique below is derived from the authorities, not copied from a granted Indian claim — **this is an acknowledged gap**.

### Cited Findings
- 2025 Guidelines recognise "governing external devices or physical processes" as a route to patentability. — [Lexology Part 5](https://www.lexology.com/library/detail.aspx?g=b35781d8-4ffe-4a05-9257-ff752fc40cdb).
- *Blackberry* (30 Aug 2024): "For algorithms, the inventive feature must be the implementation." — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/).
- *Robert Bosch* (Madras HC, 25 Mar 2025): the method claim for preheating/controlling injected fuel temperature "detailed a series of steps that the Court found to be technical and practical, **involving physical measurements and processes** rather than abstract or mental activities"; the Court rejected the Controller's reasoning that the invention "constituted a theoretical method and did not result in a tangible product." — [De Penning](https://depenning.com/blog/robert-bosch-limited-v-deputy-controller-of-patents-and-designs-interpretation-of-sec-3m/); [Selvam & Selvam](https://selvams.com/insights/madras-high-court-holds-that-not-all-inventions-must-yield-physical-products-to-be-patentable/).
- Raytheon/Microsoft line: no new hardware required, so reciting a general-purpose processor is not itself fatal. — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/).

### Inferences — concrete drafting technique (my analysis, grounded in the above)

**Claim set to file (ordered by survivability):**

1. **Independent system claim — the primary claim.** Structure it so that every limitation is anchored in apparatus, and the mathematics appears only as a *configured-to* limitation of a named physical controller:

 > *A lighting system for a room, comprising:*
 > *a plurality of light modules, each comprising a light source and a driver responsive to a received drive command;*
 > *a sensing node positioned in the room and comprising an illuminance sensor, a colour sensor, and a spatially-resolving element arranged to produce a coarse spatial distribution of light incident on the node;*
 > *a wireless transceiver coupled to the sensing node and to the light modules;*
 > *a controller coupled to the transceiver and configured to:*
 > *(a) during a calibration mode, successively energise each light module individually while the remaining light modules are de-energised, and record from the sensing node the resulting illuminance, colour and spatial-distribution measurement attributable to that light module, so as to populate a light transport matrix for the room in which each column corresponds to the measured optical contribution of one light module at the sensing node;*
 > *(b) during an operating mode, obtain from the sensing node a current measurement of the room, determine an uncontrolled daylight component as the difference between the current measurement and the sum of contributions predicted by the light transport matrix for the present drive levels, and subtract said daylight component from a target room state;*
 > *(c) determine drive levels for the plurality of light modules by solving, subject to per-module drive-level bounds, for drive levels whose product with the light transport matrix approximates the daylight-compensated target; and*
 > *(d) transmit drive commands corresponding to the determined drive levels via the wireless transceiver, thereby causing the light modules to emit light producing the target room state.*

 Why this survives: the novelty is not asserted to lie in least-squares. It lies in (a) — a **physical measurement protocol performed on the actual room**, which is not a computation at all — and in the closed loop terminating in (d), a physical change in the world. The daylight-subtraction step in (b) is likewise a *measurement-derived* quantity, not a pure calculation.

2. **Independent method-of-operating claim**, mirroring the above, expressly recited as "A method of operating a lighting system comprising a plurality of light modules and a sensing node, the method comprising: energising each light module individually…, measuring…, constructing…, solving…, **and driving the light modules so as to change the illuminance and colour of the room**." Note the last clause: the method must *end in the world*, not in a number. *Robert Bosch* is direct authority that such a method is not a mere mental act and that the absence of a "tangible product" is not a valid objection.

3. **A calibration-method claim standing alone** — "A method of characterising a room-level lighting installation, comprising energising each of N light sources individually while the others are off, measuring at a fixed sensing node…, and storing an N-column transport matrix." This is the most 3(k)-proof claim in the set because it contains essentially no mathematics; it is a measurement procedure. It is also the narrowest commercially, but it is worth having as a fallback the examiner can be steered to.

**Language that works:**
- Recite the **physical sensing modality** concretely (photodiode array / spectral channels / angularly-resolving aperture), not "a sensor configured to sense."
- Recite **what is measured** and **what physically changes**, in the same claim.
- Use "**configured to**" on a structurally-recited controller rather than "means for."
- Recite the **wireless link and the drive command** — a transmitted command that changes a driver's output is a physical act.
- Put the technical effect in the claim as a functional result clause ("thereby maintaining the measured room illuminance within X of the target notwithstanding varying daylight") and repeat it in the specification's problem-solution statement.

**Language that fails:**
- "A computer programme product comprising instructions which, when executed…" — **delete.** CRM/CPP claims are routinely refused under 3(k) in India regardless of the underlying invention.
- "A method of determining drive levels for a plurality of light sources, comprising: receiving a target vector; solving a constrained least-squares problem against a transport matrix; and outputting drive levels." This is a mathematical method plus data I/O. It will be refused.
- Pure means-plus-function ("means for solving," "means for determining"). India has **no statutory equivalent of 35 U.S.C. §112(f)**; functional claiming without corresponding structure attracts objections under Section 10(4)/10(5) (clarity, sufficiency, support) in addition to 3(k). Use it only in dependent claims, if at all.
- Any claim mentioning energy tariffs, occupant billing, building-service subscription, or "optimising operating cost" — *OpenTV* makes the business-method bar absolute and unqualified.

**Specification technique (as important as the claims):**
- The Background must state a **technical problem**: that open-loop lighting control cannot compensate for inter-luminaire optical coupling, room surface reflectance, or time-varying daylight, so delivered illuminance/colour at the point of use deviates from target.
- The Summary must state the **technical effect in measurable, physical terms** — e.g. reduction in illuminance error (lux) and colour error (Δu′v′ or CCT) at the sensing point under varying daylight; reduction in commissioning time; reduction in electrical power drawn for a given delivered lux. The 2025 Guidelines reward "measurable system-level impact."
- Include at least one worked example with **real numbers from a real room** (matrix dimensions, measured lux before/after, convergence behaviour). Indian Controllers respond to demonstrated effect.
- Describe the hardware in enough detail to support Section 10(4) sufficiency: sensor part class, drive-level resolution, protocol.

### Gaps
- **I could not retrieve or quote the independent claims of any granted Indian patent in lighting control, HVAC control, or an analogous closed-loop sensor-actuator domain.** `patents.google.com` and `ipindia.gov.in` are both blocked from this machine. A search for Signify/Philips Indian lighting-control grants returned only US and EP documents ([search results](https://patents.google.com/patent/US9629220B2/en), [Signify IP page](https://www.signify.com/global/our-company/intellectual-property/news/blogs/new-patent-families)). **Action item: before drafting, run an InPASS / Google Patents `country:IN` search on Signify N.V., Koninklijke Philips, Lutron, Siemens, Honeywell, Johnson Controls and Robert Bosch in IPC classes H05B 47/xx (control of lighting by sensors) and F24F 11/xx (HVAC control), pull 10–15 granted IN claim sets, and mirror the claim architecture of the ones that issued without 3(k) amendment.** This is the single biggest hole in this research.
- The Indian Manual of Patent Practice and Procedure's position on functional/means-plus-function claiming could not be verified from a primary source; treat my statement on it as practitioner-level guidance to confirm.

---

## Q4. Does the calibration sweep help? Would the full method claim be a technical process or a mathematical method?

### Takeaway
**Yes — the calibration sweep is the strongest single feature in the disclosure for 3(k) purposes, and it should be made the centre of gravity of the independent claims.** A method claim of the form "energising each luminaire individually, measuring…, constructing a transport matrix, solving…, driving the luminaires to…" should be treated as a **technical process, not a mathematical method**, because it begins with physical actuation, proceeds through physical measurement of the actual installed room, and ends with physical actuation. The solver, claimed alone, is a mathematical method and would be refused.

### Cited Findings
- 2025 Guidelines: "mathematical methods per se remain excluded, but their application in technical systems may be patentable"; excluded examples are pure numerical methods — "Brent's method … or the Adams' method of solving differential equations." Conversely, formulae recited "in systems for encoding, reducing noise in communications/electrical/electronic systems" escape the exclusion. — [Lexology Part 5](https://www.lexology.com/library/detail.aspx?g=b35781d8-4ffe-4a05-9257-ff752fc40cdb); [LKS](https://www.lkslaw.com/insights/articles/decoding-the-algorithm-exclusion-a-closer-look-at-draft-cri-guidelines-2025).
- *Robert Bosch*: a control method "involving physical measurements and processes rather than abstract or mental activities" is not excluded, and the objection that it "did not result in a tangible product" was rejected. — [De Penning](https://depenning.com/blog/robert-bosch-limited-v-deputy-controller-of-patents-and-designs-interpretation-of-sec-3m/).
- *Blackberry*: "the inventive feature must be the implementation" — an algorithm claimed as such fails. — [Kan & Krishme](https://kankrishme.com/analyzing-the-draft-computer-related-inventions-cri-guidelines-2025-part-2-key-judgement/).
- 2025 Guidelines recognise "governing external devices or physical processes" as patentability-conferring. — [Mondaq](https://www.mondaq.com/india/patent/1663246/a-detailed-analysis-of-indias-new-cri-guidelines-2025).

### Inferences
- Constrained least squares is textbook numerical linear algebra. Claimed at the level of "solve `min ||Ax − b||` subject to `0 ≤ x ≤ 1`," it is indistinguishable in kind from the Adams'/Brent's examples the Guidelines give as excluded. **The solver is not where the patent is.** Do not let the drafter write the case around it.
- The transport matrix is **not a mathematical abstraction in this invention — it is a measured physical characterisation of a specific room**, obtained by a physical sweep. That is closer to a calibration/metrology step than to a computation. This is the argument to make in an FER response: the matrix is data produced by physically operating the apparatus on the environment, akin to a calibration curve, and the claim is not to the matrix but to a control process incorporating it.
- The daylight subtraction is similarly defensible: it is the determination of an **uncontrollable physical input by measurement and by comparison against the measured model**, i.e. a disturbance estimate in a physical control loop — the same shape as the fuel-temperature control loop in *Robert Bosch*.
- **Practical drafting consequence:** put the calibration sweep and the drive step in the independent claim and push the solver formulation down into dependent claims ("wherein determining the drive levels comprises minimising a weighted squared error between the product of the transport matrix and a candidate drive vector and the daylight-compensated target, subject to bounds…"). If the examiner objects under 3(k) to the dependent claim, the independent survives. If the solver is in the independent claim, an examiner can characterise the whole claim as a mathematical method with conventional data-gathering.
- **Residual risk to be honest about:** an examiner can still say the calibration sweep is trivial/conventional (it is a known technique in computer graphics and in lighting commissioning — "light transport matrix" is established terminology), that the hardware is conventional, and that therefore the only contribution is the mathematics. That is the *Blackberry* attack. The answer must be that the contribution is the **integrated closed loop with in-situ measured spatial+colour transport and measured-daylight disturbance rejection**, and the specification must carry data showing the technical effect. Whether that succeeds depends on the prior art, not on 3(k) doctrine.

### Gaps
- No Indian decision I could find addresses a calibration-then-solve control architecture directly. *Robert Bosch* is the closest and is a Madras HC decision under 3(m), not 3(k) — persuasive, not on all fours.
- Whether the 2025 Guidelines' Annexure contains a worked example on calibration or sensor-actuator loops: unknown (blocked).

---

## Q5. Section 3(m) and other exclusions that might bite

### Takeaway
**3(m) is a low risk after *Robert Bosch*.** The exclusion most likely to be raised after 3(k) is **Section 3(f)** — mere arrangement or re-arrangement of known devices each functioning independently — because the system claim is, on its face, "a known sensor + known LED luminaires + a known wireless link + a known solver." Sections 10(4)/10(5) (sufficiency, clarity, support, unity) are the other practical battlegrounds. 3(m) itself should be answerable in one paragraph.

### Cited Findings
- Section 3(m): "a mere scheme or rule or method of performing [a] mental act or method of playing [a] game" is not an invention. — [indiankanoon, Section 3(m)](https://indiankanoon.org/doc/62867576/) (blocked; text per search summary).
- *Robert Bosch Limited v. Deputy Controller of Patents and Designs*, Madras HC, **CMA(PT)/1/2024, Justice Senthilkumar Ramamoorthy, 25 March 2025**: Controller refused a "Method of Preheating and Controlling the Temperature of Fuel injected into a Combustion Engine" reasoning that it "constituted a theoretical method and did not result in a tangible product, thereby attracting the bar under Section 3(m)." The Court set the refusal aside, holding the method "involves a set of inventive steps and cannot be seen as just a mental act." — [De Penning](https://depenning.com/blog/robert-bosch-limited-v-deputy-controller-of-patents-and-designs-interpretation-of-sec-3m/); [Kan & Krishme](https://kankrishme.com/interpretation-of-method-claim-under-section-3m-by-madras-high-court-robert-bosch-limited-v-the-deputy-controller-of-patents-and-designs/); [Anand & Anand Patents Rewind](https://patentsrewind.wordpress.com/2025/05/06/madras-high-court-clarifies-the-scope-of-section-3m/).
- The Delhi High Court has also "chart[ed] a test for Section 3(m)" — [Managing IP](https://www.managingip.com/article/2gx9wxtip7yiba5i4h1xc/sponsored-content/delhi-high-court-charts-test-for-section-3m-of-the-patents-act) (sponsored content; not fetchable; treat as a pointer only).
- There is live academic disagreement about importing European reasoning into 3(m): "Playing by Different Rules: Why Equating Section 3(m) to European Patent Law Doesn't Hold Up" — [SpicyIP, August 2026](https://spicyip.com/2026/08/https-spicyip-com-2026-08-playing-by-different-rules-why-equating-section-3m-to-european-patent-law-doesnt-hold-up-html.html) (blocked; title only). **Flag: 3(m) interpretation is being actively contested as of 2026.**

### Inferences
- **Section 3(f)** is the sleeper risk. The counter is drafted, not argued: the specification must show the components **do not function independently** — the sensing node's measurement determines the drive of every luminaire, and each luminaire's output changes what the sensing node measures. That mutual dependence is the definition of a closed loop and is the textbook answer to 3(f). Say so explicitly in the specification.
- **Section 2(1)(ja) inventive step** will in practice do more work than 3(k). Prior art in daylight-harvesting, DALI/Zigbee commissioning, and closed-loop illuminance control is dense (Signify/Philips, Lutron, Siemens, Honeywell). Expect the real fight to be obviousness over a daylight-harvesting controller combined with a known light-transport calibration.
- **Section 3(m) answer, if raised:** the claimed steps physically energise luminaires and physically measure light; a human cannot perform them mentally; *Robert Bosch* squarely covers it.
- Section 3(c) (discovery of a scientific principle / abstract theory) is a possible make-weight objection against the transport-matrix concept; same answer as 3(k).
- Not applicable: 3(a), 3(b) (unless an absurd energy claim is made), 3(d), 3(e), 3(h), 3(i), 3(j), 3(p).

### Gaps
- I could not identify the Delhi HC 3(m) test referred to by Managing IP (case name unknown).
- The SpicyIP August 2026 piece indicates the 3(m)/EPO-equivalence debate is unsettled in 2026; I could not read it.

---

## Q6. What would likely be REFUSED vs what would likely be GRANTED

### Takeaway
Refusal is near-certain for anything claiming the solver, the matrix, or a CRM. Grant is realistic — subject to prior art — for a system or method claim in which an in-situ calibration sweep, a measured daylight disturbance, and physical driving of luminaires are all recited in the independent claim.

### Inferences (this section is analysis, not cited fact)

**Likely REFUSED under 3(k):**
- "A method for computing drive levels for a plurality of light sources using a light transport matrix, comprising receiving a target illuminance vector and solving a constrained least-squares problem." → mathematical method + algorithm.
- "A computer-readable medium storing instructions that when executed cause a processor to…" → computer programme per se.
- "A method of controlling lighting, comprising receiving sensor data, processing the sensor data according to a model, and outputting control data." → data in, data out; *Blackberry*.
- "A system comprising a processor configured to execute a lighting-optimisation algorithm" where the only recited hardware is a processor and memory. → contribution lies wholly in the algorithm.
- Anything framed around cost/energy-billing optimisation or facility-management service delivery → *OpenTV*, absolute business-method bar.
- A claim to the transport matrix itself, or to a data structure. → not an invention.

**Likely GRANTED (3(k)-wise) if prior art permits:**
- The system claim in Q3 above, reciting sensing node hardware, light modules with drivers, wireless transceiver, calibration mode with individual energisation, daylight determination by measurement, and transmission of drive commands causing emission.
- The corresponding method-of-operating claim ending in "driving the light modules so as to alter the measured illuminance and colour of the room."
- The standalone calibration/characterisation method claim.
- A claim to the sensing node itself, if the spatially-resolving + colour sensing arrangement is structurally novel. (This one does not touch 3(k) at all and is worth including if the hardware supports it.)

**The realistic middle case:** FER raises 3(k) on all claims plus 3(f) plus inventive step; the response amends the independent claim to pull the calibration sweep and the drive step up from dependents, adds the "thereby" result clause, deletes the CPP/CRM claims, and argues *Ferid Allani* + *Raytheon* + the 2025 Guidelines' "governing external devices or physical processes." That is a normal, winnable prosecution. Budget for it.

**Be blunt with the client:** 3(k) is survivable here. **Inventive step is the real risk**, and a thin provisional that discloses only "we build a transport matrix and solve least squares" will not support the narrow, hardware-anchored claims that ultimately have to be filed to get past both objections.

---

## Q7. Provisional vs complete specification in India

### Takeaway
A provisional secures a priority date **only for subject matter it actually discloses**. Claims in the later complete specification that are not "fairly based" on the provisional take the complete's date and are judged for novelty/inventive step at that later date. The complete must be filed within **12 months**, with **no extension and no condonation**; miss it and the application is deemed abandoned and the priority is lost. **Claims are not required in a provisional.**

### Cited Findings
- "Sub section (i) states that once a patent application accompanied by a provisional specification is filed … it is mandatory to file the complete specification within a period of 12 months from the filing date." — [LinkedIn, Demystifying Section 9](https://www.linkedin.com/pulse/demystifying-section-9-indian-patent-act-provisional-complete); [Global Patent Filing](https://www.globalpatentfiling.com/blog/Navigating-Provisional-and-Complete-Specifications-under-Section-9-of-the-Patents-Act-1970-Insights-for-Innovators-in-2025).
- "If the complete specification is not filed within this period of 12 months the original application filed will be treated as abandoned and the invention will lose priority. **No extension exists for this deadline, the general power to condone delay does not reach it, and post-dating cannot extend it.**" — [Global Patent Filing](https://www.globalpatentfiling.com/blog/Navigating-Provisional-and-Complete-Specifications-under-Section-9-of-the-Patents-Act-1970-Insights-for-Innovators-in-2025); [Intepat, Provisional Patent Application in India (2026)](https://www.intepat.com/blog/provisional-patent-application).
- Fair basis: "**Claims fairly based on the provisional keep its date; claims resting on new matter take the date of the complete specification, and must meet novelty and inventive step on that later date.** A provisional application establishes a priority date only for subject matter that is clearly disclosed in it." — [Intepat](https://www.intepat.com/blog/provisional-patent-application); [Legismith](https://legismith.com/provisional-patent-application-in-india/).
- "In India it is the document your later claims will be measured against for fair basis, so the quality of the disclosure decides whether those claims obtain its date." — [Intepat](https://www.intepat.com/blog/provisional-patent-application).
- Section 9 also bars post-dating of a provisional as a way to buy time — [Lexology / R K Dewan, Section 9 as a bar to post-dating](https://www.rkdewan.com/articles/article-section-9-of-the-indian-patents-acts-acts-as-a-bar-for-post-dating-of-a-provisional-application/).
- "For provisional specifications, the filing fee is the same as a complete specification, but the provisional approach lets you lock in the priority date while deferring the cost of professional specification drafting." — [search summary, professional-fees sources](https://www.intepat.com/blog/patent-fees-cost-india).

### Inferences — what a provisional must actually contain for this invention
Claims are optional in an Indian provisional, but the disclosure is everything. To make the later hardware-anchored claims fairly based, the provisional **must** already describe, in specific terms:
1. The sensing node's physical construction — illuminance channel, colour channels, and the mechanism by which coarse spatial distribution is obtained (aperture/lens/array geometry). "A sensor that senses spatial distribution" is not enough.
2. The calibration sweep as a concrete procedure: one source at a time, others off, settling time, what is recorded, how the column is formed, what happens with N sources, how the matrix is stored and per-room keyed.
3. The daylight estimation mechanism, explicitly, as a measured/derived disturbance.
4. The constrained formulation including the constraint set (drive bounds, non-negativity, any smoothness/flicker constraints) and at least one named solution approach.
5. The wireless command path and the driver interface.
6. **Numbers.** Room dimensions, number of sources, measured lux/colour error before and after, timings.
7. Every variant you may want to claim later: different sensing modalities, multiple sensing nodes, re-calibration triggers, partial re-calibration, occupancy interaction. **Anything not in the provisional gets the later date.**

**Consequences of a thin provisional, stated bluntly:** the applicant does not lose the right to file a complete, but the narrowing amendments that 3(k) and inventive-step objections *will* force during prosecution are exactly the specific hardware and procedural details a thin provisional omits — so the claims that eventually get granted will carry the complete's date, not the provisional's. Twelve months of intervening publication, public demonstration, or the company's own sales then become prior art against those claims. A thin provisional in a fast-moving hardware field is often worse than no provisional, because it creates a false sense of protection.

### Gaps
- I could not retrieve the text of Section 9 itself or an Indian judgment applying "fair basis" to a provisional. The doctrine as stated is consistent across commentary but should be checked against Section 9(1)–(4) and Section 11(2)/(3).
- The precise Indian formulation of "fair basis" (a legacy of the UK 1949 Act) and whether Indian courts still use that label rather than "support" was not verifiable.

---

## Q8. Costs in India (2026)

### Takeaway
Official fees are trivially small — a full provisional-to-grant run costs a few tens of thousands of rupees in government fees at the reduced rate. **Professional drafting fees dominate, and the cheap end of the market (₹6,000–₹12,000 for a provisional) will produce exactly the thin provisional described above.** For an electronics/software-hardware case of this complexity, budget ₹40,000–₹80,000+ for a properly drafted complete specification. **Critical entity point: a private limited company is NOT a "natural person." It gets the reduced slab only if it is a DPIIT-recognised Startup or a registered MSME/small entity, and must file Form 28 with evidence.**

### Cited Findings (all e-filing; verify against the First Schedule)
| Item | Natural person / startup / small entity / educational institution | Other (large entity) | Source |
|---|---|---|---|
| Form 1 filing, with provisional or complete (≤30 pp, ≤10 claims) | **₹1,600** | **₹8,000** | [Intepat, Patent Cost in India 2026](https://www.intepat.com/blog/patent-fees-cost-india); [IncorpX](https://www.incorpx.io/blog/patent-filing-fees-india-2026-startup-vs-company) |
| Request for Examination (Form 18) | **₹4,000** | **₹20,000** | [Intepat](https://www.intepat.com/blog/patent-fees-cost-india) |
| Expedited Examination (Form 18A) | **₹8,000** | **₹60,000** | [S.S. Rana, Express Patent Examination in India](https://ssrana.in/articles/express-patent-examination-in-india/); [Lexgin](https://www.lexgin.com/early-publication-form-9-and-expedited-examination-form-18-when-is-it-worth-it/) |
| Early Publication (Form 9) | **₹2,500** | **₹12,500** | [Lexgin](https://www.lexgin.com/early-publication-form-9-and-expedited-examination-form-18-when-is-it-worth-it/); [Patent in India](https://patentinindia.com/form-9-request-for-early-publication/) |
| Extension of RFE-type deadlines under the 2024 Rules | — | **₹50,000 per month** | [Intepat, Patent Amendment Rules 2024](https://www.intepat.com/blog/patent-amendment-rules-2024-a-comprehensive-overview) |
| PCT search fee, **IPO as ISA** | **₹2,500** | **₹10,000** | [Intepat, PCT Filing from India 2026](https://www.intepat.com/blog/pct-filing-india) |
| PCT preliminary examination fee (ISR by IPO) | ₹2,500 | ₹10,000 | [Intepat](https://www.intepat.com/blog/pct-filing-india) |
| PCT preliminary examination fee (ISR not by IPO) | ₹3,000 | ₹12,000 | [Intepat](https://www.intepat.com/blog/pct-filing-india) |

**⚠ CONFLICT IN SOURCES ON THE "SMALL ENTITY" SLAB.** One source states filing is "₹1,600 for natural persons and startups, **₹4,000 for small entities**, and ₹8,000 for large entities" ([IncorpX](https://www.incorpx.io/blog/patent-filing-fees-india-2026-startup-vs-company)), and the Form 9 figures are given as "₹2,500 natural persons/startups, **₹6,250 small entities**, ₹12,500 large" ([Lexgin](https://www.lexgin.com/early-publication-form-9-and-expedited-examination-form-18-when-is-it-worth-it/)). Other sources put small entities in the ₹1,600 / ₹2,500 slab ([Intepat](https://www.intepat.com/blog/patent-fees-cost-india)). The three-tier ₹1,600 / ₹4,000 / ₹8,000 structure is the **pre-2019** schedule; the Patents (Amendment) Rules 2019 merged startups and small entities into the lowest slab. Many fee blogs still reprint the old table. **Do not quote a small-entity figure to the client without checking the current First Schedule on ipindia.gov.in.** For this company the practical answer is the same either way: get DPIIT Startup recognition and file Form 28 to land in the ₹1,600 slab.

**Professional fees:**
- Provisional drafting + filing: **₹6,000–₹12,000** (commodity end) — [Razorpay](https://razorpay.com/learn/patent-cost-in-india/); [Intepat](https://www.intepat.com/blog/patent-fees-cost-india).
- Complete specification drafting + filing where no provisional was filed: **₹10,000–₹27,000** (commodity end) — [Razorpay](https://razorpay.com/learn/patent-cost-in-india/).
- "For more complex applications, professional drafting costs range from **₹15,000–₹60,000** depending on complexity, and professional complete specification drafting and filing can range from **₹40,000 to ₹80,000**." — [Abhijit Bhand, cost of complete patent application](https://abhijitbhand.com/blog/how-much-patent-agent-charge-for-a-complete-patent-application-how-much-are-government-fees-a-complete-guide-on-cost-of-complete-patent-application-in-india); [Indium Law](https://www.indiumlaw.com/patent-cost-in-india/).
- "For most applicants, the total patent cost in India ranges from **₹45,000 to ₹1,15,000**, depending on the type of applicant, complexity of the invention, and procedural steps involved." — [Ezylegal](https://www.ezylegal.in/blogs/cost-of-patenting-understanding-fees-and-expenses); [Lattice Law, Patent costs in India, September 2026](https://www.latticelaw.com/cost-patent-registration-india/).
- Startups pay the same fees as natural persons at the IPO across filings, subject to Rule 2(fb) — [S.S. Rana](https://ssrana.in/articles/express-patent-examination-in-india/).
- Form 28 with supporting documents must be filed to claim startup/MSME benefit — [Intepat](https://www.intepat.com/blog/patent-fees-cost-india).

### Inferences
- **Realistic all-in Indian budget for this case (reduced slab), my estimate:** provisional ₹1,600 official + ₹25,000–₹60,000 professional (a properly detailed provisional for this invention is *not* a ₹8,000 job); complete ₹1,600 + ₹60,000–₹1,20,000 professional including drawings; RFE ₹4,000 (or ₹8,000 expedited); early publication ₹2,500; FER response ₹25,000–₹60,000 professional. **Total to grant, roughly ₹1.2L–₹2.5L**, dominated by professional fees, excluding renewals. The ₹45,000–₹1,15,000 figure quoted by aggregators corresponds to a simpler case with a commodity-priced agent.
- The market's low-end drafting prices exist because the drafting is thin. For a 3(k)-exposed case, paying the low end is the expensive option.

### Gaps
- Excess-page and excess-claim fees (commonly cited as ₹160/page and ₹320/claim for the reduced slab, 5× for large entities) could not be verified from a primary source. **Verify.** They matter here: a well-drafted spec with matrices, drawings and a worked example will exceed 30 pages.
- Renewal fees from the 3rd year, and the 2024 Rules' reported discount for advance payment of 4+ years' renewals electronically, were not verified.
- Form 25 (FFL) official fee not verified from a primary source.

---

## Q9. Timelines

### Takeaway
Complete within **12 months** of provisional (hard). Publication at **18 months** from priority, or ~1 month after a Form 9 request. **RFE within 31 months** of earliest priority for applications filed on or after **15 March 2024** — the Patents (Amendment) Rules 2024 change from 48 months is confirmed and in force. FER typically **12–24 months** after RFE on the ordinary route; **1–3 months** on expedited. Grant typically **3–5 years** ordinary; **1–2 years** with expedited examination and early publication.

### Cited Findings
- "The Patent (Amendment) Rules 2024 reduced the timeline for filing request for examination … from 48 months to **31 months from the date of earliest priority**." Applications filed **before 15 March 2024 remain at 48 months**; applications filed **on or after 15 March 2024 are at 31 months**. — [Intepat, Patent Amendment Rules 2024](https://www.intepat.com/blog/patent-amendment-rules-2024-a-comprehensive-overview); [Cyril Amarchand client alert, 18 March 2024](https://www.cyrilshroff.com/wp-content/uploads/2024/03/Client-Alert-Patent-Amendment-Rules-2024.pdf); [De Penning](https://depenning.com/news-and-insights/key-highlights-the-patent-amendment-rules-2024/).
- "For applications entered in India on or after March 15, 2024, the national phase entry and the request for examination deadline both expire at the same 31-month mark. The 2024 amendment eliminates the buffer … practitioners should now docket national phase entry and Form 18 filing as a single coordinated deadline." — [Intepat, Filing the Request for Examination in India](https://www.intepat.com/blog/patent-request-for-examination).
- "On the ordinary route, the gap between the request for examination and the first report runs to **twelve to twenty-four months**, while expedited examination takes **one to three months**." — [Intepat, Patent Examination India](https://www.intepat.com/blog/patent-examination-procedure-india); [Kayser Legal](https://kayserlegal.com/blog/patent-examination-process-in-india-timelines-and-requirements/).
- "You must respond to the FER within **6 months (extendable by 3 months)**." — [Intepat](https://www.intepat.com/blog/patent-examination-procedure-india).
- "While it usually takes **3–5 years** … Expedited examination can cut the timeline drastically—sometimes to just **1–2 years**." — [Dr. Rahul Dev, How to Get Your Patent Granted in India in 2026](https://patentbusinesslawyer.com/how-to-get-your-patent-granted-in-india-in-2026/); [Intepat, patent grant within 1 year](https://www.intepat.com/blog/patent-grant-india-1-year).
- Early publication: "If a request for early publication is filed under Rule 24A and on Form 9 then the application is published **within one month** of making such request. Without this request, the patent application is published automatically **18 months** after the filing or priority date." — [Lexgin](https://www.lexgin.com/early-publication-form-9-and-expedited-examination-form-18-when-is-it-worth-it/); [Patentmyidea](https://patentmyidea.in/early-publication-of-patents-in-india-how-startups-can-get-their-patent-application-published-faster).

### Inferences
- **Concrete docket for this client if the provisional is filed on, say, 1 October 2026:** complete by 1 October 2027 (absolute); Paris/PCT by 1 October 2027 (absolute); publication ~1 April 2028 unless Form 9 is filed; **RFE by 1 May 2029 (31 months from 1 Oct 2026)**; FER realistically 2029–2031 ordinary route, or within months of RFE if Form 18A expedited is used (available to DPIIT startups).
- **Recommendation:** because the company qualifies (if DPIIT-recognised) for expedited examination at ₹8,000, and because a granted patent is worth far more than a pending one for fundraising and for deterring copyists in a fast-moving lighting market, file Form 9 + Form 18A early. The cost delta is ~₹6,500 in official fees.
- The 31-month RFE and 31-month national-phase deadlines now coincide. Docket them as one date.

### Gaps
- No art-unit-specific pendency statistics for electronics/lighting control were found. The 3–5 year figure is a general average; CRI cases historically run longer because of 3(k) objection cycles.

---

## Q10. PCT, foreign filing, and Section 39

### Takeaway
Paris Convention deadline is **12 months** from the provisional; PCT national phase in India is **31 months**. **Section 39 requires an Indian resident to either file in India first and wait 6 weeks, or obtain a foreign filing licence on Form 25, before filing abroad. Breach carries imprisonment up to 2 years, or a fine, or both, under Section 118, plus the application is deemed abandoned under Section 40 and any granted patent is vulnerable to revocation under Section 64.** The IPO as ISA is dramatically cheaper than the EPO, but an EPO search report carries far more weight in Europe and the US.

### Cited Findings
- **Section 39:** "If you are resident in India and want to file a patent application outside India, you must satisfy Section 39 … before that foreign filing is made. For most applicants, the requirement is met simply by **filing in India first and waiting 6 weeks**, provided no secrecy direction is issued under Section 35 during that period." — [Intepat, Foreign Filing License in India: Section 39 & Form 25](https://www.intepat.com/blog/foreign-filing-license-permission); [S.S. Rana](https://ssrana.in/ip-laws/patents/ffl-foreign-filing-license-patent-india/).
- **Section 118 penalty:** "if any person fails to comply with any direction given under section 35 or makes or causes to be made an application for the grant of a patent in contravention of section 39 he shall be punishable with **imprisonment for a term which may extend to two years, or with fine, or with both**." — [Intepat](https://www.intepat.com/blog/patent-foreign-filing-license-permission); [Mondaq, Section 39 Of The Patents Act, 1970](https://www.mondaq.com/india/patent/1066932/section-39-of-the-patents-act-1970).
- Civil consequences: "Section 40 states that an application made in contravention of Section 39 **shall be deemed to be abandoned**. If a patent has already been granted, it may subsequently become **vulnerable to revocation under Section 64**. In a company context, **liability may extend beyond the named inventor to persons who were responsible for, or consented to, the foreign filing**." — [Intepat](https://www.intepat.com/blog/patent-foreign-filing-license-permission); [The IP Press, Failure to obtain foreign filing permit in India](https://www.theippress.com/2020/07/10/failure-to-obtain-foreign-filing-permit-in-india-illegality-or-irregularity/).
- **PCT international filing fee:** "For Indian applicants, the international filing fee is **1471 USD**, with an additional fee of **17 USD per sheet over 30**, and a reduction of **11 USD for PCT easy filing**." — [Intepat, PCT Fees in India 2026](https://www.intepat.com/blog/pct-entry-fee-india). **Conflicting figure** of "base fee of **USD 1,667**" appears in [Intepat, PCT Filing from India 2026](https://www.intepat.com/blog/pct-filing-india). Authoritative source is the [WIPO PCT Fee Tables (amounts on 1 August 2026)](https://www.wipo.int/pct/en/docs/fees.pdf) — **blocked from this machine; check it.** The fee is set in CHF, so the USD equivalent moves.
- **90% reduction:** "The WIPO 90% reduction on the international filing fee applies **only to natural persons (individuals) who are nationals of and reside in India. India is on the qualifying list. Startups, companies, MSMEs, and educational institutions do NOT qualify.**" "Where there are multiple applicants, every applicant must independently satisfy the natural-person and residency criteria." The reduction "brings the base fee … down to approximately USD 167 for qualifying individuals." — [Intepat, PCT Filing from India 2026](https://www.intepat.com/blog/pct-filing-india); underlying instrument: [WIPO, Applicability of 90% Reduction in Certain PCT Fees](https://www.wipo.int/documents/d/pct-system/docs-en-fee-reduction-january.pdf) (blocked).
- **ISA options:** "Indian applicants can choose from **8 International Searching Authorities** including the European Patent Office (EPO). The Indian Patent Office as ISA is the lowest-cost option (**INR 10,000 for others; INR 2,500 for qualifying applicants**)." — [Intepat, PCT Filing from India 2026](https://www.intepat.com/blog/pct-filing-india).
- **India national phase deadline: 31 months.** — [Intepat, PCT National Phase India Calculator](https://www.intepat.com/pct-national-phase-calculator); [BananaIP national phase](https://www.bananaip.com/services/patents/national-phase).

### Inferences — the Section 39 trap this client must not fall into
- The invention is being made in India by Indian residents. If the company (or a US-based co-founder, or an investor's counsel) files a US provisional **first** without an FFL and without having filed in India six weeks earlier, that is a criminal offence under Section 118, the Indian application is deemed abandoned under Section 40, and the Indian patent (if granted) is revocable. This is the most common serious mistake Indian hardware startups make.
- **Safe sequence:** (1) file the Indian provisional; (2) either wait 6 weeks with no Section 35 secrecy direction, or file Form 25 for an FFL (typically issued in ~3 weeks) if you need to file abroad sooner; (3) file the PCT (or direct foreign applications) by the 12-month anniversary.
- **ISA choice — the real trade-off.** IPO as ISA costs ₹2,500/₹10,000. EPO as ISA costs of the order of a thousand-plus euros (I could not verify the current figure — see Gaps). The IPO's search quality in CRI/control-systems art is generally regarded as weaker and its written opinion carries little persuasive weight at the EPO or USPTO. For a case where the fight is inventive step over dense Signify/Lutron/Honeywell prior art, **an EPO search is worth paying for** — it tells you early, and cheaply relative to national-phase costs, whether the invention is actually novel, and a positive EPO ISR/IPRP materially smooths EP national phase (and supports PPH elsewhere). If the budget is genuinely tight and the PCT is being filed only to keep options open, IPO as ISA is defensible.
- **Do not rely on the 90% PCT reduction.** A private limited company is disqualified. If the founders hold the invention personally and file the PCT as natural persons resident in India, the international filing fee drops from ~USD 1,471–1,667 to ~USD 167 — a saving of well over ₹1 lakh. That is a real, legitimate structuring decision, but it has ownership consequences (assignment to the company later, investor diligence, Section 6 applicant entitlement) and should be taken deliberately with counsel, not by accident.

### Gaps
- **EPO ISA search fee for PCT applications as of 2026: not verified.** I will not invent a number. Pull it from the [WIPO PCT Fee Tables](https://www.wipo.int/pct/en/docs/fees.pdf) (Annex D, EPO) or epo.org.
- The IPO transmittal fee for acting as Receiving Office (commonly cited around ₹3,200 / ₹16,000) was not verified.
- Whether India appears on the current WIPO 90%-reduction list was asserted by a single commercial source ([Intepat](https://www.intepat.com/blog/pct-filing-india)) and I could not confirm it against the WIPO instrument. **This is a material figure — verify it directly before budgeting.**
- Form 25 FFL official fee and current issuance turnaround not verified from a primary source.

---

## Cross-cutting: what to tell the client, unvarnished

1. **Section 3(k) is survivable but it is not free.** Expect at least one FER raising 3(k). The 2025 CRI Guidelines and *Ferid Allani*/*Raytheon*/*Ab Initio* give you good answers; *Blackberry* and *OpenTV* give the Controller good ammunition if the claims are drafted lazily.
2. **Do not claim the solver.** The calibration sweep and the physical drive step are the patent. Least-squares is not.
3. **Delete every CPP/CRM claim before filing.** They are free refusals.
4. **The bigger risk is inventive step, not eligibility.** Daylight harvesting with closed-loop illuminance control is a crowded field. Commission a professional novelty search (or buy an EPO ISA search via the PCT) before spending on a complete specification.
5. **Section 3(f)** — draft the specification to show the components are functionally interdependent, not merely assembled.
6. **A thin provisional is a trap.** Everything you might need to claim must be disclosed now, with numbers.
7. **Never file abroad first.** Section 39 breach is a criminal offence and kills the Indian right.
8. **Verify the fee slab and the PCT reduction** before budgeting; the secondary sources conflict and several reprint pre-2019 tables.
9. **Two things are genuinely unsettled as of September 2026:** the exact final form/date of the 2025 CRI Guidelines, and the scope of Section 3(m) (a contested question as of an August 2026 SpicyIP piece I could not read).
