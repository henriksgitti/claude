# Red team: research/longlist.md (A7/A21, before A18 and B1)
Date: 2026-11-07 | Mode: RED TEAM (reasoning, not sources) | Verdict: **needs work.** The list meets the Stage A bar. But as a basis for B1 it overstates who pays, counts about 10 buyer clusters as 30 problems, and has no row where *this* founder has an edge in reaching the buyer. Method points on `research/scoring.md` v3 and the two open CEO questions are in `research/reviews/2026-11-07-redteam-scoring-v3.md`.

Scope: all 30 rows, Findings, Excluded table. Facts are assumed correct (they were fact-checked in `2026-11-07-longlist.md` and the A21 re-check). Rejected scoring options (new criteria/weights, K3–K6, minimum bars, fixes 7–10) are not re-argued. A18 fields (signer, budget line, wedge, route, buyer count, young-vendor example) are not filled in yet. Where this review names a signer or wedge, it is my inference for A18/B1 to test. Vendor names marked `[UNVERIFIED]` were not opened in this review.

## Fatal or near-fatal objections

**F1. No row answers "why this founder", and the €10k / part-time constraint is not applied anywhere.** (near-fatal for the "ready to start" goal, not for Stage A)
- `founder-brief.md` gives the founder German, AI-agent implementation (1.5 years, asset management, Lisbon), a health-innovation Master's and €10k of own money. It names no buyer network in German hospitals, insurers, care operators or pharma.
- The Findings call L07/L22, L26 and L05 "the strongest rows", combining "a dated rule change, a budget and founder fit". Founder fit is asserted there, not shown. The fit in those rows is a topic match ("AI/automation for workflow"). The same is true of almost every admin row. An investor will read this as "anyone with an LLM and a CTO could do this".
- The constraint bites hardest on the institutional rows:
  - Every insurer tender in `pain-industry.md` asks for ISO 27001 (BIG, BAHN-BKK, AOK Rheinland/Hamburg, hkk).
  - calliora already lists ISO 27001 for hospital sales (`hospital-billing-audits.md`).
  - Commissioning a processor of social data requires prior notice to the insurer's supervisory authority: "nur zulässig, wenn der Verantwortliche seiner Rechts- oder Fachaufsichtsbehörde rechtzeitig vor der Auftragserteilung den Auftragsverarbeiter … anzeigt" [A] ([§ 80 Abs. 1 SGB X](https://www.gesetze-im-internet.de/sgb_10/__80.html), opened 2026-11-07). Abs. 3 adds that commissioning a non-public processor is allowed only if operations would otherwise be disrupted or the work is "erheblich kostengünstiger" (my reading of who Abs. 3 covers is inference).
  - None of these is fundable from €10k. EXIST is closed while the founder is employed (`munich-ecosystem.md`).
- The only rows where the brief gives any edge:
  - **L11:** Portuguese, Lisbon network. Brazil as a source country for nurses is my hypothesis, `[UNVERIFIED]`.
  - **L26:** interest in clinical research, but no experience in it.
- **Consequence for B1:** criterion 4 will be "4 M" on nearly every row and will not separate them. The 10-minute founder-access check proposed in both earlier scoring red teams is still unanswered. It is the cheapest test in the whole pipeline.

**F2. "Who pays (status)" often labels spend *around* the problem as spend *on the job*. This primes B1 to pass K1.** Fix 4 defines the category as "the wedge's signer type pays today for the same job", but the long-list labels say "proven" where the money buys something else:
| Row | Label in long list | What the money actually buys | Same job as a product? |
|---|---|---|---|
| L02 | "*proven* self-pay €3,364/month in care homes" | Care itself | No. And 91 % of services turn clients away, so supply is the constraint. Providers who are full do not pay for more demand (inference) |
| L04 | "*proven* self-pay €2,800–3,500/month + agency fees" | Labour (carers) via agencies | Only if the wedge *is* an agency (a people business with labour-law exposure, Verbraucherzentrale: 24-h care by one person "legal nicht möglich") |
| L05 | "§ 8 Abs. 8 grant €143.3m paid 2019–24" | A 40 % co-funded grant, max €12k/facility | Partly. **Read the other way:** only ~37 % of a free pool was drawn in six years and payouts are flat at €24–32m/yr (`reimbursement-routes.md`). Even subsidised demand is weak. From 2027 the old grant drops staff-workflow purposes (PNOG) |
| L06 | "*proven*: 8 speech-recognition buyers" | Dictation software (mostly tenders closed to startups) | Not the same job as LLM letter drafting. UKE and Leipzig build in-house (`scoring.md` calibration) |
| L14 | "*budget*: €2.9bn TSVG fees" | Extra fees paid **to physicians** for appointments | No. Not a software budget at all |
| L26 | "*proven*: sites are paid for patient identification; MPIRIQ €99–329/month" | Sponsor fees to sites; a price list with no named customer | Fix 4: a price list "counts only with a named paying customer". Site fees are not a tool purchase |
| L08 | "*proven*: Helios framework + 4 other buyers, KHZG FTB2" | Discharge platforms; KHZG was one-off money that has ended | Yes, but the money that made it "proven" is gone |
- *Effect:* "proven spend exists in 15 rows" (Findings) overstates K1 passes. Fix: A18 should record "spend on this job" separately from "adjacent spend". Task A23.

**F3. 30 rows ≈ 10 buyer clusters. Several rows are not solvable by a product.** The wedge rule (fix 3: score each wedge as its own row) can then fill the top 5 with variants of one bet, such as three hospital-admin wedges.
| Cluster (signer type) | Rows | Comment |
|---|---|---|
| Hospital revenue/coding (commercial director, medical controlling) | L07, **L10** | L10 has the same signer, the same vendors and the same software category. A18 notes say KVs give groupers away free. The churn ends when the 2028 regime settles, so a product built for 2027 has a 12–18-month window. **Merge into L07** |
| Payer/MD claims and assessment (Kasse, MD) | L21, L22, L23 | All fall under the SVHV direct award (€50k, "soll … wechseln"), § 80 SGB X notice, and ISO 27001 in tenders. **L22 is the opposite side of L07.** Selling audit AI to both hospitals and MDs is a credibility conflict: pick one side |
| Private insurers | L24 | Different regime (private company, no procurement law). Likely also EU DORA ICT third-party rules for insurers (`[UNVERIFIED]`, not checked) |
| Family carer support (Pflegekasse, employer, family) | L01, L02, L03, (L04) | L01 and L03 share the two only plausible payers: Pflegekasse via § 45 SGB XI, or the employer (A18 notes: heycare, Munich, >200 named employers). L02's hospital side is L08 |
| Hospital clinical workflow (CIO, medical director, nursing director) | L06, L08, L09 | The discharge letter sits in both L06 and L08 |
| Practice admin (practice owner) | L12, L13, (L14) | Price-sensitive, self-serve buyers; PVS lock-in |
| Patient navigation in a disease (Kasse) | L15, L16, L17, L18 | Kasse builds in-house (BARMER) or there is no third-party purchase |
| Clinical research (sponsor/CRO) | L26, L27, **L30** | The file itself calls L30 "an enabler for L26 rather than a pain". **Merge into L26** |
| Regulatory/market access (manufacturer) | L28, L29 | Both need a regulatory-affairs/HTA expert co-founder |
| Singles | L05, L11, L19, L20, L25 | |

Not product-solvable as framed (root cause outside a vendor's reach):
- **L02:** staff, not matching.
- **L04:** legal status.
- **L11:** Länder recognition authorities.
- **L15:** capacity planning.
- **L25:** the budget ends in 2026, so K1 fails by definition ("in force today").
- **L29:** notified-body capacity, and the revision may shrink the problem.
- **L19:** ePA/ident is owned by gematik/BSI and the insurers' IT providers. That is **the same reason S6 was excluded** ("infrastructure owned by gematik … a startup cannot fix it from outside"). Keep the rule consistent: exclude L19 or un-exclude S6.

After merging L10→L07 and L30→L26 and excluding L19, 27 rows remain. The Stage A bar of ≥20 still holds.

**F4. A trigger everyone can see is a race the funded incumbent wins.** The Findings sell "dated rule changes" (2027 audit quotas, the 5 % rule, the PNOG fund) as the reason to act now. The incumbents already sell into exactly these:
- Tiplu markets its MBEG-Assistent "directly at the BStabG" and is in ~30 hospitals.
- calliora raised $6m in Oct 2026.
- voize has $50m and 1,100 facilities.

The founder can only go full-time in **September 2027**. The 2027 audit wave starts on 1 Jan 2027. A seed investor in Munich will ask why a team that starts nine months into the wave beats a funded Munich team that started in 2023.

The triggers that still favour a late entrant are those whose effect starts **after** Sep 2027:
- GOÄ 2028 (L24)
- Kurzzeitfallpauschalen 2028 (L10, but see F3)
- § 113e from 2028 (L05)
- 5 % exemption applications for launches from 2027 onward (L26)

## Per row: payer / founder fit / incumbents / verdict
Abbreviations: **Fit** = founder can reach and sell to this signer part-time (H/M/L, my judgement from `founder-brief.md`). **v3 risk** = how B1 is likely to mis-place the row under scoring v3. Tests are desk-only (no outward action).

| # | Real signer and budget line (inference) | Can 1–2 part-time people sell here? | Fit | Incumbents / status quo | v3 risk | Verdict | Cheapest desk test |
|---|---|---|---|---|---|---|---|
| L01 | Pflegekasse (§ 7a counselling, run in-house or by Pflegestützpunkte) or **employer** (HR benefits). Family: WIdO says non-use is mostly "fehlender Bedarf" | Kasse: €50k direct award, then "wechseln". Employer: private, faster | M | Kassen apps, Pflegestützpunkte, pflege.de; employer side: heycare (Munich) | Low as framed (K1 fails on navigation); **under-rated as an employer wedge** | Merge with L03 into "carer support", two wedges | heycare founding year + one named paying employer with a date. If heycare ≤5 years old at that sale, the employer wedge passes K2 (and heycare is the competitor) |
| L02 | Families (pay for care, not search); hospital social services (= L08) | Family marketplace: needs provider-side fees, but providers are full | L | Recare, Pflegeplatzmanager (A18 notes), lead portals | Low | **Out / merge into L08.** Supply problem | Find one named home-care/care-home operator paying per lead. Given 91 % turn clients away, expect none → kill |
| L03 | Pflegekasse via § 45 SGB XI courses (in force); employer | Courses: Kassen already buy (Mobil × PflegeBetreuer, curendo); price unknown | M | curendo, PflegeBetreuer, Kassen's own courses | **Wrongly up** if pain is scored on "45 % cut hours" while the wedge is a course: a course does not give hours back | Keep only if the pain evidence matches the wedge (fix 3) | Find any price or contract value for a Kassen-funded online carer course (Kasse annual report, award notice) |
| L04 | Families via agencies | Only as an agency (people, posting law, liability) | L | ~266 agencies (2017, stale) | Low | **Out** for a software founder | One named agency paying a ≤5-year-old software vendor. If none, close |
| L05 | Operator management (private ~majority); 40 % grant; PNOG fund is a bill until passed | Yes for small operators (~32,000 facilities, private). Chains are slow | M | voize ($50m, 1,100); care-software suites adding AI `[UNVERIFIED]` | **Wrongly up** if voize counts as K2 evidence and criterion 8 does not fall with it (the route evidence *is* the dominant competitor) | Big pain, taken wedge. Look for a sub-wedge (TI/KIM onboarding: only 50 % had an activated TI card) | Check whether ≥2 care-software suites ship speech/AI documentation (vendor pages). If yes, kill the voice wedge |
| L06 | Hospital CIO/medical director; IT budget (KHZG money ended) | Tenders closed; in-house builds at university hospitals; B3S/ISO and MDR risk for decision-support features | L | Microsoft/Nuance, KIS vendors, UKE IDM, UKL-GPT | **Wrongly high:** pain 5, market 5, future 5 carry it into tier B by base total (calibration: 70) although no startup sale exists | Park unless a young vendor with a named hospital is found | One more search, private chains (Helios, Asklepios, Sana, Schön): did they buy LLM letters from a ≤5-year-old firm, or build/buy big? |
| L07 | Commercial director / head of medical controlling; DKI median €40k planned non-staff spend. 1,603 IKs × €40k ≈ **€64m/yr** pool (my math), shared | Private hospitals buy outside TED. Needs ISO 27001 and coding expertise | L | Tiplu/LOGEX (~400 customers, MBEG in ~30), ID Berlin (>1,400), Dedalus, calliora (Munich, $6m), Kodierbörse | **Wrongly high** on pain/market/future; "unproven" only | Real problem, late and crowded for this founder | List every vendor marketing BStabG/MD-audit AI in 2026 with funding. If ≥5 incl. 2 funded, competition = 1 |
| L08 | Hospital (discharge management, social services) | Same hospital barriers; Kassen pilots only | L | Recare (~2/3 of hospitals, vendor claim; Knappschaft via Telekom), Pflegeplatzmanager | Medium | Crowded network business | Recare named customer count (already partly in A18 notes). Settles criterion 8 |
| L09 | Nursing director/HR; operators | Hospital tenders need ≥500 FTE references. Care operators are private | L | Mature rostering suites; DBfK satisfaction "konstant recht hoch" | Low | Root cause is headcount. Only a shift-pool/marketplace wedge (CrewLinQ, A18) | CrewLinQ founding year + named paying operator |
| L10 | Medical controlling / practices | — | L | Grouper/billing vendors; KVs free | Low | **Merge into L07** (F3); time-limited | None needed |
| L11 | Employer HR (recruiting budget; fees `[UNVERIFIED]`) | As a placement business, yes; as software, the bottleneck is the authorities | **M (only row with a language edge)** | Recruiters, state programmes `[UNVERIFIED]` | Low (2 evidence items) | Watch: weak evidence, but the one row where the founder's languages could matter | Destatis recognitions by country of training: is Brazil/Portugal a material source? If <2 %, drop the edge |
| L12 | Practice owner | Self-serve, but needs PVS integration (same lock-in as excluded S6) | M | PVS vendors; policy (KBV form reform) | Low | Low | Does any major PVS offer a public third-party API/marketplace? If not, out |
| L13 | Practice owner, €9–229/month | **Yes**, self-serve, private, many buyers | M | 10 vendors incl. Doctolib | **Wrongly up on confidence:** H tags everywhere, so it may be the only tier-A row although an investor would see a commodity | Commodity. Criterion 8 must be 1 | Funding of the top 3 AI-phone vendors. If any raised >€10m, competition = 1 |
| L14 | KV/116117, Kassen; patients use free apps | No paying third-party buyer observed | L | Doctolib, 116117, GeDIG (draft) | Low (K1 fails once the "€2.9bn" is read correctly) | **Out** | None |
| L15 | GKV/self-pay; capacity planning | No | L | DiGA (treatment, a different problem) | Low | **Out**: not product-solvable | None |
| L16 | Kasse (builds in-house: BARMER); navigator review "mostly no effect" [A] | No third-party purchase observed | L (cancer interest only) | BARMER in-house; cancer apps `[UNVERIFIED]` | Low | **Out** unless a named Kasse contract with a third-party vendor exists | One search for a Kasse contract with an oncology navigation vendor |
| L17 | Kassen (invitations are statutory); radiology networks for lung LDCT (new benefit Apr 2026) | Unclear; patient-marketing limits for practices `[UNVERIFIED]` | L | Kassen mailing, GP eligibility checks | Low; **a lung-screening eligibility/referral wedge is unexamined** and is a genuine 2026 trigger | Watch | Does any radiology network or Kasse buy invitation or eligibility-check software (named)? |
| L18 | Pharma (orphan patient finding) or ZSE centres (no budget) | Pharma: vendor qualification; diagnostic support → MDR risk | L | Patient-finding vendors `[UNVERIFIED]` | Low | **Out** for this founder | None before a clinical co-founder exists |
| L19 | Kassen IT providers; gematik/BSI rules | No | L | Ident vendors (Nect, used by BARMER, A18) | Low | **Exclude** (S6 consistency) | None |
| L20 | **Pharmacy owner** (private, 16,601, self-serve), operating costs | **Yes**: small private buyers, remote sales | M | Wholesaler portals, pharmacy ERP vendors `[UNVERIFIED]`; shrinking pharmacy count | **Possibly wrongly out:** K1 fails only because purchases were "not searched in A7". Pain [B] 20.1 h/week is strong; top hurdle "consulting physicians" 72.4 % | Under-researched | Find one paid shortage/substitution tool for pharmacies with a price and a named pharmacy, and check whether ERP vendors bundle it free. Either outcome decides K1 and criterion 8 |
| L21 | Kasse head of claims (admin budget, capped from 2027) **or the BPO incumbents** (IQVIA HSS, SPS, GFS: private, not procurement-bound) | Direct: no (ISO 27001, § 302 references, § 80 SGB X). Channel: caery's Telekom channel is caery's, not the founder's | L | IQVIA HSS (5 of 13 awards), BPOs, caery | **Wrongly first:** the calibration leader (70/68) passes K2 only via another firm's channel | Re-frame: the realistic first customer is a BPO buying a tool, not a Kasse | (a) Is Telekom TechBoost an open, published intake? (b) Any named BPO–startup AI partnership? If both are no, L21 is "K2 unproven" |
| L22 | MD-IT (framework bids due 2 Dec 2026); TK (QuantCo) | Only as a subcontractor/consortium member. The window closes before the company exists | L | MD-IT framework winners, QuantCo | **Wrongly up** on K1 (€88m is "proven") | Out as direct; conflicts with L07 | After the award notice (TED, by procedure ID), check the winners. No action before Stage C |
| L23 | 15 MDs (insurer-financed) | €50k direct-award pilots; MD Nordrhein needs €600k turnover. **Only 15 buyers**, so the venture-scale case needs the EU | L | IT service providers of the MDs | Medium | Pilot-able, small market | Re-query TED for the MD RLP procedure and any other MD AI PoC notice in 2026 |
| L24 | PKV claims director; 39 full members; private (no procurement law); GOÄ 2028 | Enterprise insurer onboarding (outsourcing/ICT risk rules `[UNVERIFIED]`) | L | In-house + claims-software vendors `[UNVERIFIED]` | **Possibly wrongly out:** "no tenders" is expected for a private buyer, not proof of no spend | Under-researched; real post-2027 trigger | One named PKV customer of a ≤5-year-old claims-automation vendor (press) |
| L25 | Gesundheitsämter; pact money ends 2026 | Bavarian municipal direct award ≤€100k is legal, but buyers are cutting | L | IT service providers of local health offices | Low | **Out** (K1: budget not in force from 2027) | None |
| L26 | **Sponsor** clinical-ops/feasibility (often decided outside DE); sites have no budget | Pharma vendor qualification, long cycles; site SaaS is self-serve | L–M (interest, not experience) | MPIRIQ (Munich, 2024), TriNetX, CROs | **Pain mis-scored if site pain is used:** sites rate patient identification a big hurdle in 4–9 %, staffing in 50–74 %; an EHR patient-finder showed no enrolment effect [A] | The CEO's favourite domain, but the evidence supports a *capacity/German-share* wedge for sponsors (service + software), not a patient-finder SaaS | Count new active substances launched in DE per year (G-BA AMNOG procedure count) = size of the 5 %-rule buyer pool. Check whether MPIRIQ names a paying practice |
| L27 | Sponsor/CRO start-up teams; sites (overhead, no budget) | Site tools face free incumbents `[UNVERIFIED]` | L | CTMS/eISF vendors; standard contract clauses (policy fix) | Low | Low | Check whether a major eISF vendor gives site tools away free. If so, kill the site-paid wedge |
| L28 | Pharma market access; pays consultancies | Only with an HTA expert; ~58 JCAs in 2026 = tiny buyer count, high ACV | L | HTA consultancies, CROs | Low–medium | Out without an HTA co-founder | Any ≤5-year-old AI-for-JCA vendor with a named pharma customer |
| L29 | SME manufacturers; pay consultants | Bottleneck is the notified bodies; the revision may shrink the pain | L | RA consultancies, eQMS tools `[UNVERIFIED]` | Low | **Out** | None |
| L30 | Pharma RWE, academia | 53 FDZ applications so far | L | — | Low | **Merge into L26** | None |

## Rows to watch in B1
- **Likely wrongly in or too high:**
  - **L21** wins on a borrowed channel.
  - **L06 and L07** are carried by pain/market/future through the tier-B base-total fallback.
  - **L13** may be the only tier-A row because confidence is high in a commodity category.
  - **L05** passes if voize counts as K2 evidence, yet voize is the reason the wedge is taken.
  - **L22** passes K1 on money a startup cannot reach before 2027.
- **Likely wrongly out or under-researched:**
  - **L20** pharmacies: private, self-serve buyers with strong [B] pain; purchases were never searched.
  - **L24** PKV: private, with a 2028 trigger.
  - The **employer wedge of L01/L03**.
  - The **lung-screening wedge of L17**.
  - **L11** as the only row with a founder language edge (weak evidence).
- **Merge/exclude before B1:** L10→L07, L30→L26, L19 (S6 rule), L25 (K1). L02, L04, L14, L15, L16, L18 and L29 will very likely fail K1/K2. B1 can process them fast, but each should be listed with its reason.

## Cheapest tests (desk only, in order of value)
1. **CEO, 10 min, no outreach:** for each of the ~10 signer clusters above, do you know one person who signs such purchases, or who has bought from a company <3 years old? This settles criterion 4 (H vs M) and is the only discriminator on founder fit.
2. **calliora named hospital:** search hospital press releases and conference programmes for "calliora". One hit moves L07 from "unproven" to proven access (and confirms the competitor).
3. **voize earliest named customer and date:** settles L05 under either reading of "≤5 years" (see the scoring review).
4. **Telekom TechBoost intake + BPO–startup partnerships:** decides whether L21 really passes K2.
5. **Pharmacy shortage tool with a named paying pharmacy:** decides L20 K1.
6. **PKV named customer of a young claims vendor:** decides L24 K1/K2.
7. **heycare founding year + dated named employer:** decides the employer wedge for L01/L03.
8. **AMNOG procedures per year (G-BA):** sizes the L26 5 %-rule pool bottom-up.
9. **Care-software suites shipping AI documentation:** decides L05 criterion 8.
10. **Destatis recognitions by country of training:** tests the only founder edge (L11).

Tests 2–10 go into task A24 (researcher), except where A18 already covers them.

## Sources opened in this review
- https://www.gesetze-im-internet.de/sgb_10/__80.html — § 80 SGB X, processing of social data on behalf of a controller: prior notice to the supervisory authority (Abs. 1), conditions for non-public processors (Abs. 3) [A], accessed 2026-11-07
- Everything else is quoted from repo files (`longlist.md`, `pain-industry.md`, `pain-professionals.md`, `hospital-billing-audits.md`, `payer-processing.md`, `trial-recruitment-de.md`, `reimbursement-routes.md`, `munich-ecosystem.md`, `scoring.md`, A18 task notes), not re-opened.
