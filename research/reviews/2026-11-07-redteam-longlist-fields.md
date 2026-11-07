# Red team: research/longlist-scoring-fields.md (A18) with research/longlist.md
Date: 2026-11-07 | Mode: RED TEAM (reasoning, not sources) | Verdict: **needs work before B1.** A18 does what was asked: every row has a signer, wedge, route and buyer count, and it is honest about gaps ("None of these vendors is open to this founder"). But B1 will misuse it in three ways. (1) The K1/K2 evidence often belongs to a different product than the wedge being scored. (2) Several "Job" budget labels are generic opex, not spend on the job. (3) No row is accessible to this founder *and* large enough to fund. Fact-checking is out of scope. Facts are taken as stated in A18. Vendor and legal facts added here are from searches in this session and are marked by type.

Scope: what A18 adds (signer, budget line, wedge, status quo, trigger, first-sale route, K2 example, buyer count) and how B1 will read it under `research/scoring.md` v3. Not repeated: F1–F4 and the per-row table in `2026-11-07-redteam-longlist.md`, and S1–S6 in `2026-11-07-redteam-scoring-v3.md`.

## Fatal or near-fatal objections

**G1. The K1/K2 evidence often does not match the wedge it is meant to support. Fix 3 says the unit of scoring is the wedge (signer + product).** B1 will copy the row's evidence and pass wedges that have none.

| Row | A18 wedge | Evidence A18 gives | Why it does not transfer |
|---|---|---|---|
| L05 | TI/KIM/ePA onboarding *as a service* for care homes | K2: voize (voice documentation). Budget: § 8 Abs. 8 grant, RLP § 19a 0.5-FTE credit for *speech documentation* | Different job. The TI job has its own money: a monthly TI-Pauschale from the care-insurance fund under § 106b SGB XI. TI connection has been mandatory for all care facilities since 1 Jul 2025 (search summary of [gesetze-im-internet.de § 106b](https://www.gesetze-im-internet.de/sgb_11/__106b.html), [euregon TI FAQ](https://euregon.de/wp-content/uploads/2025/07/euregon-TI-FAQ.pdf); snippet only, not opened). So K1 may pass on the right budget. But that money goes to the facility and buys connectors and services from care-software houses, which already advertise the reimbursement process (CGM page in the same search, not opened). Inference: K2 has no example for this job, and the incumbents are the suite vendors, not voize |
| L08 | "Transition medication list" niche | K2: Recare (discharge platform, leader) | Different product. The ePA electronic medication list (eML) has been available since "ePA für alle" (15 Jan 2025), and ePA use is mandatory for hospitals since Oct 2025 (search summary, [PZ](https://www.pharmazeutische-zeitung.de/bald-kann-die-epa-mehr-168856/), [DKG notes](https://www.dkgev.de/fileadmin/default/Mediapool/2_Themen/2.1_Digitalisierung_Daten/2.1.5._Telematik-Infrastruktur/2.1.5.4_Elektronische_Patientenakte__ePA_/DKG-Umsetzungshinweise_prozessual-technischer_Teil_2025-03-14.pdf); snippet only). A free state-run substitute is missing from "Status quo". Medication-related decision support also carries MDR risk |
| L21 | Classification module sold **to a BPO** | K1: § 302 processing awards (the **Kasse** buys a service) | Wrong signer. No source shows a BPO paying a third party for document classification. Established input-management vendors already sell AI classification to private insurers. Insiders Technologies: Debeka, Signal Iduna, Ideal, BGV (search summaries of [cio.de](https://www.cio.de/article/3696206/debeka-nutzt-ki-fuer-dokumentenerkennung.html), [pressebox](https://www.pressebox.de/pressemitteilung/insiders-technologies-gmbh/insiders-technologies-steigert-vollautomatisierung-beim-bgv-um-rund-10-prozentpunkte/boxid/1306308); not opened). Neither vendor is in A18's status quo |
| L06 | LLM discharge-letter drafting | Budget labelled ***Adjacent*** by A18 itself | Under fix 4, "adjacent" means **K1 fails**. The `scoring.md` calibration still shows L06 "K1 Pass". B1 must follow A18's label, not the calibration |
| L26 | DE recruitment/feasibility service + software → "DE affiliate" head of clinical ops | Sponsor recruitment budgets | Wrong signer (already noted in F2/per-row: country allocation is decided by global study teams and CROs). A18 kept the DE-affiliate signer. The wedge is a CRO service that needs site relationships, not a product |

**Required B1 rule (one line):** K1 and K2 evidence must name the same signer *and* the same product as the wedge. Otherwise the cell is "K1 not shown" or "K2 unproven", and the row's evidence is not carried over.

**G2. A "Job" budget line that says "opex" and "no observed purchase" fails K1 by the letter.** Fix 4 requires that "the wedge's signer type pays today for the same job, sourced [A]/[B]".
- L12: "*Job:* practice opex. No observed purchase for form automation" → **K1 fail**.
- L20: "*Job:* pharmacy opex. No purchase of a shortage tool observed" → **K1 fail**, unless Apo-Mall "Bestell-Engel" turns out to be paid (fee not stated). The data owner's own platform (pharmazie.com, Avoxa/ABDA) advertises "Lieferengpass-Alternativen" (search summary, [go.pharmazie.com](https://go.pharmazie.com/blog/abda-artikelstamm), not opened). Inference: the wedge needs the ABDA article master licence, which is held by the incumbents.
- L24: "*Job:* PKV claims processing (>70m invoices/yr)" is the insurer's own cost, not an observed purchase of a GOÄ-check module. Pass only on a sourced vendor contract.
- L09: "rostering software" is close but is not the job. An internal shift-cover pool is not rostering.

If B1 passes these on "opex", K1 means nothing.

**G3. The rows a part-time, non-technical founder can reach are too small to fund, and the rows large enough to fund are closed to him.** Ceiling = A18 buyer count × A18 ACV guess, at 100 % share (my arithmetic on A18's inference prices, so all tagged L):

| Row | Route open to a new company? | Ceiling at 100 % share | Comment |
|---|---|---|---|
| L01 employer benefit | Yes (private) | 18,632 × €5–20k ≈ **€93–373m/yr** | Only accessible row with a seed-scale ceiling |
| L13 phone AI | Yes | ~103k × €1.2–2.4k ≈ €124–247m | Commodity (10 vendors incl. Doctolib) |
| L12 forms | Self-serve, but PVS-blocked | ~103k × €0.4–1k ≈ €37–99m | K1 fail (G2) |
| L05 TI onboarding | Yes (private) | ~32k × €0.6–1.8k/yr + one-off ≈ €19–58m | Service margin; the TI-Pauschale caps what operators will pay |
| L20 pharmacies | Yes | 16,601 × €0.6–1.8k ≈ €10–30m, shrinking | Data licence held by incumbents |
| L09 shift pool | Yes | operators with 3–10 homes (count not given) × €3–10k | Count missing |
| L03 Pflegekasse course | ≤€50k direct award, then "soll wechseln" | 92 × €50k ≈ **€4.6m** pilot ceiling | Recurring revenue needs a tender |
| L23 MD drafting | ≤€50k pilot | 15 × €50k ≈ **€0.75m** | Only 15 buyers |
| L24 PKV | Private, but DORA | 39 × €100–300k ≈ €4–12m | See below |
| L07 MD-audit defence | Private hospitals only | 1,807 × €20–40k ≈ €36–72m | Not shippable without a coding expert |
| L06 LLM letters | No (K1 fail, G1) | 1,807 × €30–100k ≈ €54–180m | Tenders, KIS gate |
| L29 PMS for SMEs | Yes (private) | 1,480 × €10–30k ≈ €15–44m | Flinn is the leader ($20m) and the founder has no RA background |

A Munich seed investor will ask for a €100m+ revenue pool in the beachhead. Only L01 (and the commodity L13) has one. This is the "think big but achievable" tension, now in numbers. B1 cannot fix it, but the shortlist must state it rather than hide it in criterion 2.

**G4. The timing works against the founder in both directions.** A18 shows it but does not draw the conclusion:
- Triggers already in force (audit quotas 1 Jan 2027, lung LDCT Apr 2026, Pflegebudget 2027, TI obligation) pass K1. They are captured by incumbents before the founder goes full-time in Sep 2027.
- Triggers that suit his timing (GOÄ 2028, § 113e 2028, short-stay flat rates 2028, PNOG fund) are bills or plans, so they **fail K1** ("a budget line counts only if it is in force today").

Inference: under v3 as written, no row has both a valid K1 and an entry window the founder can use. The CEO question on the 12-month clock (S6, still open) decides whether "in force by Sep 2027/2028" can count. Until then B1 should flag any row whose only K1 basis is a 2026–Jan 2027 trigger with "incumbent window closes before founder full-time".

**G5. L24 is understated.** The note "outsourcing/DORA rules `[UNVERIFIED]`" hides a real barrier. DORA has applied to insurers since 17 Jan 2025 and covers their ICT third-party providers (search summary of [Bundesbank](https://www.bundesbank.de/de/service/meldewesen/finanzaufsicht/europaeisches-meldewesen/digital-operational-resilience-act-dora--951046), [Noerr](https://www.noerr.com/de/insights/digital-operational-resilience-act-dora-bedeutung-fuer-den-finanzsektor); not opened). Inference: a 1–2-person vendor of a claims module must survive the PKV's DORA third-party onboarding. The GOÄ trigger is also only "planned".
- Correct reading: K1 not shown (G2), K2 unproven, criterion 5 = 1–2 L.

## Per item: wedge shippable? signer right? route real? K2 comparable? B1 risk
"Ship by Sep 2027" means: a part-time, non-technical founder with €10k and no CTO gets a working pilot to one paying customer.

| # | Shippable by Sep 2027? | Signer right? | First-sale route realistic? | K2 example comparable? | B1 will… |
|---|---|---|---|---|---|
| L01 | **Yes** as a service + content (navigator, hotline, guides). No integration needed | Mostly. Benefits are often bought through an EAP/family-service framework, not one lead per firm | Yes. Private, but long HR cycles (budget years) | **heycare: same signer, adjacent job** (childcare-led "Rundum-Care"). The closer comparable is **pme Familienservice**, an established eldercare provider that employers pay and that is missing from status quo (search summary, [UK Essen flyer](https://www.uk-essen.de/wp-content/uploads/2022/04/Flyer_PME_Wochenend_und_Notfallbetreuung.pdf): employer pays for counselling and placement; not opened) | Pass K1/K2 correctly. **Risk:** criterion 8 too high, because heycare (Munich, profitable) and pme are both incumbents → criterion 8 ≤ 2 |
| L02 | — | — | — | — | Out (agreed) |
| L03 | Yes, with a nurse/educator partner for content | Yes for the job; the contract is signed by the Kasse board/purchasing | Pilot yes (≤€50k). Recurring revenue no ("soll wechseln") | PflegeBetreuer: same signer, same job. Fee and age unknown | Pass K1 on § 45. K2 unproven. Score market at 1–2 (G3). Do not score pain from "45 % cut hours" (earlier review) |
| L04 | — | — | — | — | Out (agreed) |
| L05 | Yes as a service, but not a venture product | **No.** The Pflegedienstleitung does not sign IT purchases. The operator's managing director does, or central IT in chains | Yes (private) | **Stretched:** voize ≠ TI onboarding (G1) | **Wrongly pass K2** via voize. K1 should be re-based on § 106b. Criterion 8: the suite vendors |
| L06 | No (KIS integration, security, MDR/AI Act checks) | Medical director is the user champion. CIO + managing director sign | No | None | **Wrongly pass K1** if B1 follows the calibration (G1) |
| L07 | Borderline: only as a service-led tool with a coding-expert co-founder and one hospital's data | Yes (commercial director). Private chains buy centrally, and a "small private <300 beds" hospital is often a chain member | Private independents only | None (calliora unnamed) | K2 unproven, correctly. Trigger Jan 2027 → incumbent window (G4) |
| L08 | No | Yes | No (KHZG over) | **Stretched** (G1) | Wrongly pass K2 via Recare. Status quo misses the ePA eML |
| L09 | MVP yes (app). Cross-entity pooling in a group may raise temporary-agency-work (AÜG) questions `[UNVERIFIED]`, inference | Yes for a 3–10-home operator (managing director) | Yes | CrewLinQ: same signer, same job, but no named customer | K1 borderline (G2), K2 unproven. Operator count missing |
| L10 | — | — | — | — | Merge (agreed) |
| L11 | Yes as a placement/case-management service | Yes (HR) | Yes (private) | Not searched | **May wrongly fail K1.** A18 calls recruiting budgets "adjacent" with fees `[UNVERIFIED]`. But employers pay per-hire fees for international nurse recruitment, which is the same job if the wedge includes recognition. Not searched, not disproven |
| L12 | No (PVS interface) | Yes | Blocked | None | **Wrongly pass K1** (G2) |
| L13 | Yes | Yes | Yes | None named; Doctolib bought aaron.ai | Passes everything. Criterion 8 = 1 (earlier review) |
| L16 | No | PKV benefits, yes | Unknown | Fails age test | Out on K1 "adjacent", correctly |
| L17 | Yes (simple tool) | **Unclear who pays.** A €50/month tool for a rare eligibility check is not a GP purchase pattern (inference) | Unproven | None | Out on K1 "adjacent", correctly. Was "watch". Keep it out unless a paid EBM consult creates a practice-side job |
| L20 | Yes, if the drug data can be licensed | Yes | Yes | None (Bestell-Engel built by wholesaler-pharmacists) | **Wrongly pass K1** (G2) |
| L21 | No (ISO 27001, § 302 references) | **Wrong signer for the K1 evidence** (G1) | Channel closed (TechBoost needs completed B2B projects) | None | Wrongly pass K1 |
| L22 | No (physician review firm with turnover + references) | Yes | No | None | Out on K2. Conflicts with L07 |
| L23 | Prototype yes. A real pilot needs MD data access and security approval | Yes | €50k pilot is legal. No open call. MD Nordrhein needs €600k turnover | None | K2 unproven. Market ceiling €0.75m (G3) |
| L24 | No (DORA onboarding, G5) | Yes | Private, but heavy third-party due diligence | None (incumbents: Insiders Technologies classification, adesso/Verisk snippets) | Wrongly pass K1 (G2) |
| L26 | No (a CRO-type service) | **Wrong** (global, not DE affiliate) | Vendor qualification | None | Pain mis-scored if site pain is used (earlier) |
| L27 | Partly (templates) | CRO start-up lead | Private | None | K1 "adjacent" → out, correctly |
| L28 | No (HTA co-founder needed) | Yes | Vendor qualification | None | Out on founder fit/achievability |
| L29 | No without RA expertise | Yes | Yes (private) | **Flinn: same signer, same job.** It is the leader, so criterion 8 ≤ 2 (S2) | **Wrongly ranks mid-table:** it passes K1/K2 cleanly, but the founder has no RA edge (criterion 4 should be 2) and a $20m leader holds the wedge |
| L14, L15, L18, L19, L25, L30 | — | — | — | — | Out/merge (agreed) |

**Summary for B1:**
- **Wrongly pass K1:** L06, L12, L20, L21, L24.
- **Wrongly pass K2 via a stretched example:** L05, L08.
- **May wrongly fail K1:** L11 (not searched).
- **Pass cleanly but should not rank high:** L13 (commodity), L29 (leader, no founder fit), L01 (incumbents missing from status quo).

## Tier B candidates ("unproven but worth a cheap test")
These five rows pass or nearly pass K1, have a route a new company can use, and could be shipped by Sep 2027. Each has one cheap desk-only test that settles it.

| Row (wedge) | Why worth a test | Single cheapest desk test | Kills it if |
|---|---|---|---|
| **L01** employer eldercare benefit | Only accessible row with a seed-scale ceiling (G3). Private buyer | Find one dated, named employer contract (or a public-employer award notice on TED/Bayern) for **eldercare** counselling with a price, from pme Familienservice, heycare or another provider. Also: is heycare's eldercare module live? | Employers buy eldercare only inside bundled EAP frameworks at a few €/employee, so there is no room for a stand-alone wedge |
| **L03** § 45 online carer course | Budget in force. Kassen already commission online courses | Search Kassen press releases and TED for "Pflegekurs" + "§ 45 SGB XI" awards with a value, or a GKV-SV framework that fixes the fee per participant | Courses are paid per participant at a level where 92 Kassen × ≤€50k cannot fund a team, or Kassen run them only in-house |
| **L11** recognition case management for employers of foreign-trained nurses | The only row with a founder-specific angle (German + Portuguese, Lisbon network). Private buyer. K1 never tested | Find a published per-hire fee for international nurse recruitment in DE, and one ≤5-year-old agency with a named hospital or care employer. Destatis recognitions by country (Brazil/Portugal share) is test 10 from the earlier review | Fees are bundled into large recruiters' placement packages, and the bottleneck is the recognition authorities, so a new entrant adds nothing |
| **L20** pharmacy shortage assistant | Many small private buyers, high documented time cost | Two facts: is "Bestell-Engel" (or any shortage tool) **paid**, and does a usable drug-data feed exist for a third party (ABDA article master licence terms / pharmazie.com API price)? | No paid tool exists, or the data owner bundles shortage alternatives itself |
| **L07** MD-audit case defence, private independent hospitals | Largest proven job budget (DKI €40k median) a private buyer can award directly | Count independent (non-chain) private hospitals with ≥1 MD audit/quarter in the GKV-SV statistics, and find one named customer of any ≤5-year-old vendor (= A24 test 2, calliora) | Independents are too few, or all MD-audit work is outsourced to coding consultancies on success fees |

Reserve: **L23** (test: the TED award notice of the MD RLP AI PoC: winner, founding year, value). Excluded from tier B because 15 buyers × ≤€50k cannot fund a company in DACH.

## Cheapest tests
1. **B1 rule check (no research):** apply G1 and G2 when filling K1/K2. Expected effect: L06, L12, L21 and L24 drop to "K1 not shown", and L05 and L08 drop to "K2 unproven". If B1 does not apply them, the top 5 will be built on evidence about other products.
2. The five tier-B desk tests above, in order **L01, L20, L03, L11, L07**. Each takes one researcher pass with no outreach.
3. **CEO, 10 minutes (still open from the earlier review):** does he know one HR/benefits lead at a ≥250-employee firm, or one care-home operator? This decides criterion 4 for L01 and L05, the two rows with the most open routes.

## Sources opened or seen in this review
All were search summaries (snippets). No page was opened, so they are used only as pointers for B1/A24 and not as facts:
- § 106b SGB XI TI-Pauschale; TI mandatory for care facilities since 1 Jul 2025: https://www.gesetze-im-internet.de/sgb_11/__106b.html, https://euregon.de/wp-content/uploads/2025/07/euregon-TI-FAQ.pdf
- ePA eML available since Jan 2025; ePA mandatory for hospitals since Oct 2025: https://www.pharmazeutische-zeitung.de/bald-kann-die-epa-mehr-168856/
- Insiders Technologies AI classification at private insurers (Debeka, BGV): https://www.cio.de/article/3696206/debeka-nutzt-ki-fuer-dokumentenerkennung.html, https://www.pressebox.de/pressemitteilung/insiders-technologies-gmbh/insiders-technologies-steigert-vollautomatisierung-beim-bgv-um-rund-10-prozentpunkte/boxid/1306308
- pme Familienservice eldercare, paid by the employer: https://www.uk-essen.de/wp-content/uploads/2022/04/Flyer_PME_Wochenend_und_Notfallbetreuung.pdf, https://www.ruv.de/dam/jcr:212a92df-1a4c-45f0-a7be-f60a5184a8b6/Kombifaltblatt+KB-EC-BU+6504.pdf
- DORA applies to insurers from 17 Jan 2025: https://www.bundesbank.de/de/service/meldewesen/finanzaufsicht/europaeisches-meldewesen/digital-operational-resilience-act-dora--951046
- ABDA article master / pharmazie.com "Lieferengpass-Alternativen": https://go.pharmazie.com/blog/abda-artikelstamm
