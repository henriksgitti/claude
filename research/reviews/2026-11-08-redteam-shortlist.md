# Red team: research/shortlist.md (B1, as corrected by B4)
Date: 2026-11-08 | Verdict: **needs work (as caveats; no new fix tasks, rule 14)** | Task: B2 (red-team part) | Mode: RED TEAM (Opus)

Scope: the reasoning behind the top 5 (L01, L07, L06, L03, L13) and runner-up L29, plus the CEO's pending choice B3. The facts are taken as given; the fact-check (`2026-11-08-shortlist.md`) is not repeated. Earlier red-team points G1–G5 and S1–S8 (`2026-11-07-redteam-longlist-fields.md`, `2026-11-07-redteam-scoring-v3.md`) are not repeated either, only built on. I ran a few new desk checks, marked **NEW** below. Their sources are listed at the end, all opened.

**Bottom line.** L01 is the right first deep dive, but **not for the reason the shortlist gives.** New TED evidence shows that employers *do* buy eldercare counselling, in dated, named and priced contracts, so the B4 "strict K1" fallback no longer forces L01 out. The same evidence shows who wins those contracts: bundled family-service providers (pme four times, awo lifebalance once). Eldercare is a module inside a childcare-led framework, not something bought on its own. The L01 sketch ("depth on statutory benefits vs pme's broad EAP") attacks the wrong layer, and two Munich incumbents (pme, famPlus) already hold the Munich beachhead. L07 is the strongest budget, but nothing in it is specific to this founder. L06, L13 and L29 should not get a brief. L03 should not be a co-payer in the L01 brief.

## Fatal or near-fatal objections

**R1. L01: incumbents own the buying unit, and it is a bundle (NEW evidence; near-fatal for the wedge as sketched, not for the row).**
- Dated, named, priced employer purchases that include eldercare counselling, from TED [A] (fields opened via the TED API):
  - **Max-Planck-Gesellschaft (Munich), "RV Familienservice", award 763108-2025.** Winner: pme Familienservice GmbH, €1.2m. Scope: "Sorgeberechtigte von Kindern … oder pflegebedürftiger Angehöriger". The family service supports employees "in erster Linie durch Beratung und Vermittlung".
  - **Federal government (BMI procurement office), framework for federal agencies, award 397127-2025.** Winner of both lots: awo lifebalance (€949,639 + €443,143). Lot 1 includes "Modul 5 – Allgemeine Beratung zur Betreuung von pflege- und unterstützungsbedürftigen Angehörigen".
  - **TenneT TSO, EAP, award 159617-2026.** Winner: pme, result value €1.1m. The focus is mental health, but the service covers employees and their relatives.
  - **Kliniken des Bezirks Oberbayern, "Betriebliche Sozialberatung", award 321969-2025.** Winner: pme. Includes a "Lotsendienst – Recherche, Information, und aktive Vermittlung … an externe Fachstellen".
  - **Charité, "Elder Care", award 565616-2022.** €372k. Winner not shown in the API fields. The notice is from 2022, so >3 years old.
- **What this changes:**
  - **K1 passes on the strict reading** if the job is defined as "family-service / eldercare counselling for employees". It fails only if the job is "eldercare alone". B4's either/or (weak pass vs out) is a false choice.
  - **The ACV logic breaks.** Buyers procure **multi-module frameworks** (hotline, online portal, childcare placement and emergency care, eldercare counselling) worth €0.4–1.4m, and the incumbents win them. A 1–2-person eldercare-only startup cannot bid on these: it has no childcare network, no references and no turnover. The shortlist's €5–20k per-employer eldercare ACV is not how this market buys. *Inference.*
  - **The Munich beachhead is occupied.** famPlus (Munich phone numbers, 089; "integrierte Corporate-Care-Lösung", with eldercare counselling and an "Angebotssuche" covering care homes, prices and reviews, "nach DIN 77009-1 auditiert") is not in the shortlist [B] ([famplus.de](https://www.famplus.de)). It is the same product as the L01 sketch. The Bavarian Familienpakt lists famPlus and **pme Familienservice München** as providers of "Betriebliche Pflegelotsen" training for companies in 2026, alongside public bodies (Landratsamt Coburg, Wirtschaftsförderung Bayreuth) [B] ([Familienpakt Bayern PDF](https://www.familienpakt-bayern.de/images/2026/Pflegelotsentermine%202026%20final1.pdf)). This adds to the free AOK PLUS substitute already in the shortlist.
- **Buyer's view (HR lead, ≥250 staff, Munich):** "We already have pme or famPlus under a framework, or we train two Pflegelotsen through the Familienpakt. Why add a second vendor for one module, plus works-council and data-protection review?"
- **Investor's view:** "heycare raised €4m, pme has existed for decades. This is a services category with framework procurement. Where is the software margin?"
- **What survives.** The pain (3 % use of statutory counselling; 46.9 % of employed carers "hoch belastet") and the proof that employers pay. The viable wedges are different from the sketch:
  - **(i)** An AI case-handling layer sold *to* the bundlers (pme, famPlus, awo lifebalance, heycare) to cut their cost per eldercare case. That is B2B software with 5–10 buyers. *Inference*, untested.
  - **(ii)** Mid-size private employers (250–2,000 staff) that have *no* family-service contract, sold a self-serve eldercare module at a lower price. *Inference*; the size of this "no contract yet" segment is unknown.
  - The C1 brief must choose between (i) and (ii) and drop "beats pme on depth".

**R2. No top-5 idea uses anything specific to this founder (near-fatal for the investor pitch, all rows).**
- `founder-brief.md` lists three things specific to this founder:
  - Interest in drug development and clinical research. Rows L18, L26, L27 and L28 are all knocked out.
  - The Lisbon network and Portuguese. Only L11 used these, and it was knocked out unsearched (A26 deferred).
  - Hands-on AI-agent implementation. It is used only by L13, a commodity.
- On every top-5 row, the answer to "why this founder?" is "German-speaking, health-innovation master's". That is true of thousands of people. Criterion 4 is M everywhere (shortlist "Founder access … separates little"), so the method cannot show this.
- **Logistics:** the founder works full-time in Lisbon until Sep 2027. L01 (Munich HR, works council) and L07 (hospital commercial directors) are both in-person, relationship sales. Part-time sales from Lisbon in 2027 make the "first pilot in 12 months" assumption weaker than the scores imply. *Inference.*

**R3. Data-protection gates are missing from the reasoning for L03, L06, L07 and L13 (material, not fatal).**
- **§ 393 SGB V [A]** ([gesetze-im-internet.de](https://www.gesetze-im-internet.de/sgb_5/__393.html)): providers (Leistungserbringer) and Kranken-/Pflegekassen, "sowie ihre jeweiligen Auftragsdatenverarbeiter", may process health data in the cloud only with:
  - a domestic establishment ("Niederlassung im Inland"), and
  - a current C5 attestation: Typ 1 for the first 18 months after a system is first put on the market (after 30 Jun 2025), then Typ 2.
- So every cloud/LLM vendor in the chain must sit on C5-attested infrastructure. This applies to:
  - hospitals (L06, L07),
  - practices (L13: real-time voice LLMs on C5 infrastructure narrows the stack),
  - Pflegekassen (L03).
- It is manageable with C5-attested hyperscalers, but it adds cost and is the first question a hospital DPO will ask. *Inference* on the application.
- **L01:** relatives' care data falls under Art. 9 GDPR. If anonymised usage reports go to HR, the works council will at least review the tool. § 87 (1) no. 6 BetrVG [A] ([gesetze-im-internet.de](https://www.gesetze-im-internet.de/betrvg/__87.html)) gives co-determination over "technische Einrichtungen, die dazu bestimmt sind, das Verhalten oder die Leistung der Arbeitnehmer zu überwachen". Whether a usage dashboard qualifies is a legal question `[UNVERIFIED]`. The sketch's "first pilot at a Munich employer with a works council" adds months. *Inference.*

**R4. Bundling L03 into L01 makes the brief worse (near-fatal for option (a) as written).**
- **Two signers, two sales motions:** HR at private employers, and the Kasse board or purchasing via ≤€50k direct award, then tender ("soll … wechseln"). That doubles the sales load for a part-time founder.
- **L03 creates a substitute for L01.** If the Kasse pays for a personalised online carer course, the employee gets it free. An HR lead then has one more reason not to pay for L01. The AOK PLUS Pflegelotsen and the Familienpakt trainings already show this pattern.
- L03's ceiling is €4.6m (direct-award cap, not an observed price).
- **Keep L03 as one line in the L01 brief ("possible later channel"), not as a co-payer.**

## Per item: payer / founder fit / incumbents / verdict
Buyer = the person who signs. "Sellable" = can a 1–2-person, part-time founder with €10k close the first paid contract by ~Sep 2028?

| # | Who really pays (signer, budget line) | Sellable by this founder? | Why this founder? | Incumbents / status quo the shortlist under-weights | Single most likely reason it fails | Verdict |
|---|---|---|---|---|---|---|
| **L01** | HR/benefits lead with works-council sign-off. Budget line: family-service/EAP framework (TED: €0.4–1.4m multi-year at large employers) | Not into frameworks (references, childcare network). Possibly mid-size firms without a contract, or B2B to the bundlers | Weak: German and non-clinical fit the buyer, but no network or edge shown (founder-access check still unanswered) | pme (4 TED wins incl. MPG Munich, TenneT, kbo), awo lifebalance (federal framework), **famPlus (Munich, same product)**, heycare (Munich), Familienpakt Bayern Pflegelotsen, AOK PLUS, statutory § 7a counselling (free) | HR already has eldercare inside a pme/famPlus/awo bundle and will not add a vendor for one module | **Deep-dive, re-wedged** (R1) |
| **L07** | Commercial director (kaufm. Direktor) of an independent private hospital. Budget: medical-controlling staff plus success-fee consultancies; DKI median €40k is one-off + running cost | Hard. Hospital sales need a coding/medical-controlling co-founder, one hospital's data, § 393 C5 and references. Chain members buy centrally | None. The core is coding and medical-necessity know-how the founder lacks | Tiplu (~30 hospitals), calliora (Munich, €5.3m), ID Berlin, Dedalus, coding consultancies on success fee, in-house medical controlling. Structural: the Vorhaltebudget is exempt from single-case audits (KHVVG; `hospital-billing-audits.md`), so audited euros per case fall as it phases in; effect unquantified there | Incumbents capture the Jan 2027 quota wave 9 months before the founder starts, and an independent private hospital will not trust a tool without a known medical-controlling name behind it | **Deep-dive only if a medical-controlling co-founder candidate is named first**; otherwise do not brief |
| **L06** | Hospital CIO + managing director; medical director is the champion. Budget: KIS/IT capex; the KHZG one-off is over | No: KIS integration, security, MDR question, tenders with full-implementation references | None (needs clinical + KIS engineering) | Tandem (Telekom-backed, >10k facilities), Microsoft/Nuance, KIS vendors bundling, university hospitals building in-house | The KIS vendor ships the feature in its own suite | **Do not brief** |
| **L03** | Pflegekasse purchasing/board, § 45 SGB XI budget; ≤€50k direct award, then tender | Pilot yes; recurring revenue needs a tender with references | Weak (content needs a nurse educator) | Gesundheit von Morgen/PflegeBetreuer (Mobil, ZF BKK), curendo, in-house Kasse courses, TK training awards | €4.6m cap: a few pilots, then lost at tender to an established course provider | **Footnote in L01 brief, not a co-payer** (R4) |
| **L13** | Practice owner (self-pay opex, €9–229/month) | Yes. Self-serve, fast, the founder can build it | **Strongest fit** of the six (AI agents are his job) | Doctolib (owns aaron.ai and the booking channel), ~10 vendors, PVS vendors adding voice; one practice cancelled after 2 of 10 calls handled | No moat: price floor €9/month, churn, and Doctolib bundles it with booking. Investors see a feature, not a company | **No brief.** At most a 2-week build to test the founder's own skills, outside the venture pipeline |
| **L29** | RA/QA head at a device SME (20–250 staff) | Only with an RA co-founder; Flinn's named customers are large firms | None | Flinn ($20m; Zeiss, Philips, Hartmann), RA consultancies, Notified Body backlog work. A planned MDR simplification could shrink the PMS burden (shortlist criterion 9 = 3) | The founder has no RA edge against a funded leader moving down-market | **Do not brief** |

Method notes (the method itself is not re-litigated; S1–S8 stand):
- **Additive scores let L01 lead on things that do not apply to it.** Its 66 includes Reg 5, Fund 4 and Future 5. None addresses the binding constraint (incumbents hold the buying unit). Its competition score (2 H) was set without famPlus or the TED framework winners. On the evidence above, L01 competition is 1, which gives 64/60. It still ranks 1st, so the rank holds, but the margin is thinner than it looks. *My arithmetic: −1 × 2.*
- **L13 shows the opposite failure.** The only row with real founder fit is held down by competition 1 H. That is correct, and it is why L13 should not be a brief.
- **The ranking cannot see the gap between "pays today" and "pays a new 1–2-person company".** K2 "unproven" covers every row. Every brief must answer this question first.

## Pre-mortem and kill criteria
Not applicable to the shortlist (briefs only). The single most likely failure per row is in the table above. Kill criteria for the C1 briefs belong to the brief review.

## Cheapest tests (before or at the start of C1)
| Row | Cheapest test | Type | Confirms if | Kills if |
|---|---|---|---|---|
| **L01** | Pull the ~19 TED "Familienservice"/EAP notices since 2022 (DE): winner, value, duration, eldercare share or module price, subcontracting/consortium clauses. Add the partner/white-label pages of pme, famPlus, awo lifebalance and heycare. The query recipe is under Sources | Desk, researcher, ~1 run | Some frameworks price eldercare as a separate module or lot, or allow subcontractors; or a bundler buys tech from third parties | Eldercare is always unpriced inside full bundles, and the bundlers build their own tools |
| **L01** | 3 conversations with HR/benefits leads at Munich firms of 250–2,000 staff: "Do you have a family-service contract? Does it cover eldercare? What is usage? What would make you pay for a separate eldercare module?" | **Outreach: needs CEO approval** (rule 5). Could double as the founder-access check | ≥1 of 3 has no contract and names a budget | 3 of 3 are covered by pme/famPlus/awo or by Familienpakt Pflegelotsen |
| **L07** | CEO, 10 min: name one medical controller or coding expert who might co-found. Desk: the A26 count of independent private hospitals with ≥1 MD audit per quarter | CEO check + desk | A named candidate exists, and independents number ≥150 (*my threshold*, inference) | No candidate. Then no brief: the founder cannot sell or build it alone |
| **L06** | None worth running for this founder. If the CEO insists: Harzklinikum award winner and age | Desk | — | (default: drop) |
| **L03** | TED/Kassen press search for awarded "Pflegekurs § 45" online courses with a value | Desk | Price per participant supports >€50k per Kasse per year | Courses run in-house or at a few €k per Kasse |
| **L13** | Is Doctolib's phone assistant included in its subscription, and at what extra price? Do the top 3 PVS vendors offer their own voice agent? | Desk | A specialty niche the bundlers do not cover | Doctolib/PVS bundle it at ~0 extra cost |
| **L29** | Flinn pricing page / any SME (<250 staff) customer; status of the MDR targeted revision on PMS duties | Desk | Flinn is enterprise-only and SMEs are priced out | Flinn has SME tiers |

## View on B3 (the CEO's pending choice)
**Recommendation: option (a), changed. Deep-dive L01 as one brief, re-wedged per R1, with L03 as a footnote. Add L07 as the second brief only if the CEO can name a medical-controlling or coding co-founder candidate in the 10-minute check. Do not deep-dive L13 or L06.**

Why:
- **L01 vs the strict fallback.** The B4 fallback assumed L01 fails strict K1. The TED awards show employers pay for eldercare counselling (MPG Munich, federal agencies, TenneT, kbo, Charité). So the strict reading keeps L01 in, as long as the job is "family-service / eldercare counselling" rather than "eldercare alone".
- **The fallback (L07 + L13) gives two briefs where "why this founder?" has no answer.** L07 has no founder edge and L13 has no venture case. Two briefs that will fail a seed investor's first question are busywork for a part-time CEO.
- **L01 is the only row where:**
  - the buyer is non-clinical and German-speaking (founder fit at the signer level),
  - the product can start as a service plus AI with €10k,
  - a priced purchase pattern is now shown.
  Its risk is incumbents, and one desk run plus three HR conversations can test that cheaply.
- **L07 has the strongest budget**, but without a co-founder the brief would describe a company someone else should found.

What would change my mind:
- **Against L01:** the TED pull shows eldercare is never priced separately and frameworks forbid subcontractors, *and* 3 of 3 HR leads are already covered. Then drop L01 and go to the next point.
- **For a different second idea:** run the deferred A26 L11 test (per-hire fees for international nurse recruitment; one young agency with a named employer). L11 is the only long-list row with a founder-specific angle (German + Portuguese, Lisbon network). If it passes K1, it beats L07 as the second brief for this founder. This is a CEO call (it reopens a knocked-out row), so it is listed as an open question, not a task.
- **For L07:** a co-founder candidate is named, or MIA is confirmed as a ≤5-year-old winner (C1).

No new tasks added (rule 14: the shortlist has had its B4 fix round). No issue changes the B3 pick outright: B3 already offers L01 + L07. The changes above are for the CEO to weigh in B3 and for the C1 brief.

## Sources opened in this review (accessed 2026-11-08)
- TED API (https://api.ted.europa.eu/v3/notices/search), [A]:
  - query `FT~"Familienservice" AND buyer-country=DEU AND publication-date>=20220101`: 19 notices
  - same with `FT~"Eldercare"`: 4
  - same with `FT~"Elder Care"`: 4
  - same with `FT~"Pflegeberatung" AND FT~"Beschäftigte"`: 4
  - Fields read: publication-number, buyer-name, winner-name, result-value-lot, total-value, title-lot, description-lot, description-proc
  - Notices: 763108-2025 / 329012-2025 (MPG, pme, €1.2m), 397127-2025 (BMI, awo lifebalance, €949,639 + €443,143), 159617-2026 (TenneT, pme, €1.1m result / €880k total), 321969-2025 (kbo, pme), 565616-2022 (Charité, €372k)
- https://www.famplus.de: famPlus corporate care, eldercare counselling, Munich phone numbers (089), "nach DIN 77009-1 auditiert" [B]
- https://www.famplus.de/gast/angebot/pflegeberatung: eldercare counselling for employees; "Angebotssuche" covering care homes, prices and reviews [B]
- https://www.familienpakt-bayern.de/images/2026/Pflegelotsentermine%202026%20final1.pdf: "Ausbildungsangebote ‚Betriebliche Pflegelotsen'", Bavaria, as of Feb 2026; providers: famPlus, pme Familienservice München, Landratsamt Coburg, Wirtschaftsförderung Bayreuth [B]
- https://www.gesetze-im-internet.de/sgb_5/__393.html: § 393 SGB V cloud use, C5 attestation [A]
- https://www.gesetze-im-internet.de/betrvg/__87.html: § 87 BetrVG co-determination [A]
- WebSearch snippets only (not used as fact): voiio employer care benefit survey (personalwirtschaft); GKV-SV/TK/vdek positions on sample audits (already resolved in `hospital-billing-audits.md`).
