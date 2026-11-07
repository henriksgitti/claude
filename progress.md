# Progress

## Current state
- Project: **Healthcare Venture** (scope opened from cancer to healthcare on 2026-11-06, see `decisions/2026-11-06-scope-pipeline.md`).
- Stage: **A — Scan** (in progress). A1 trends scan drafted (`research/trends.md`); A2 source map drafted (`research/sources-map.md`); A3 patient/caregiver pain drafted (`research/pain-patients.md`, 11 problems); A4 professional pain drafted (`research/pain-professionals.md`, 10 problems). A5 industry/payer pain drafted (`research/pain-industry.md`, 10 problems). A6 Munich ecosystem drafted (`research/munich-ecosystem.md`). A9 reimbursement/funding routes drafted (`research/reimbursement-routes.md`). A10 applied the critic fixes to `research/trends.md` and `research/sources-map.md`. A11 drafted `research/hospital-billing-audits.md` (MD audits, 2027 rules, incumbents). Cancer-only work archived in `archive/`; its V1 draft feeds A7.
- Infrastructure: worker session on environment `healthcare-venture`. WebFetch fails DNS for many hosts (destatis.de, bundesgesundheitsministerium.de, vdek.com), but `curl` through the proxy reaches them: fetch with curl + local text extraction. Reddit is effectively unusable: direct fetch is bot-checked and `site:reddit.com` search returns almost no reddit.com hits (A2). Working alternatives and recipes are listed in `research/sources-map.md`.
- No interviews (by design until Stage D). Decisions: see `decisions/`.

## Next steps
1. Researcher: A12, A13, A14, A15, A16, A17, A7 (one per run), using the recipes in `research/sources-map.md`. Critic: A8 alongside (`research/munich-ecosystem.md`, `research/reimbursement-routes.md` and the revised `research/trends.md` / `research/sources-map.md` ready for review).
2. Then B1 (score, top 5) → CEO picks 2–3.

## Open questions
- **Reddit API key (now more important):** A2 found Reddit unreachable (bot challenge; search returns almost no reddit.com hits). A free Reddit app/API key created by the CEO is the only clean route. Without it, A3–A5 rely on German forums, reviews, job ads and tenders.
- Optional allowlist / network change: WebFetch fails DNS for most hosts; curl is blocked by bot checks at trustpilot.com, indeed.com, glassdoor, crunchbase.com, dealroom.co, oecd.org (web), europepmc.org (web), gutefrage.net, aerztezeitung.de, springermedizin.de, background.tagesspiegel.de. Not bypassed.
- CEO: own budget, target date to go full-time, no-go areas (see `founder-brief.md`).
- **CEO decision before B1: replace the scoring method?** Red team (`research/reviews/2026-11-07-redteam-scoring.md`) verdict: the current `research/scoring.md` fails. An idea with no payer can outscore one with a clear payer (68 vs 61 in a worked example), and the method does not capture whether a 1–2-person startup can sell to the buyer or the CEO's own buyer access. Options: (a) adopt the proposed scheme: 6 knock-outs (no proven spend, no startup-accessible first sale, MDR IIa+/drug, DACH SAM < €50m, draft-law-only revenue, not a product problem) + 8 weighted criteria (max 100) + confidence caps; (b) only add knock-outs K1/K2 to the current scheme; (c) keep as is. Recommendation: (a), and also answer the 10-minute founder-access check in the review ("Cheapest tests" 1). Changing `scoring.md` and `templates/venture-brief.md` ("/90") needs your OK.

---

## Log
<!-- Newest first. Format:
### YYYY-MM-DD — <task id> <task title>
- Done:
- Not done / blocked:
- Next:
- Open questions:
-->

### 2026-11-07 — Red team of research/scoring.md (critic)
- Done: RED TEAM review of the Stage B method → `research/reviews/2026-11-07-redteam-scoring.md`. Verdict: **fail as is**. Reasoning only; 3 new facts checked for the proposed scheme (Art. 20 BayWiVG direct award ≤€100k; federal ≤€50k from 1 Jul 2026; EU threshold €216k 2026–27).
- Fatal objections: (1) purely additive: a "payer unclear" idea beats a clear-payer idea 68 vs 61; (2) "budget owner" ≠ startup can sell (tenders need €0.25–6m turnover, references, KHZG certificate), and direct-award/private-buyer routes are not rewarded either; (3) founder fit = topic match, not buyer access, domain edge, part-time feasibility or co-founder dependency; (4) a score of 3 needs no evidence, so unknowns hide in the middle, and a free pilot meets "achievable"; (5) "≥€1bn EU" market size is top-down and ignores buyer counts (e.g. 15 MDs).
- Proposed: 6 knock-outs + 8 criteria (weights 4/4/3/3/2/2/1/1, max 100) + H/M/L confidence (L capped at 3) + sensitivity check and tiers. `scoring.md` not edited.
- Tasks added: A18 (researcher: long-list fields signer / budget line / first-sale route / status quo / wedge / buyer count), after A7.
- Not done: no B1 scores computed; worked examples are illustrative only.
- Open questions: CEO decision on the scoring scheme (see Open questions).

### 2026-11-07 — A11 Hospital billing audits & coding: size, rules 2027, incumbents (researcher)
- Done: `research/hospital-billing-audits.md`.
  - Size [A]: 1,138,534 MD audit reports in 2025; 48.9 % led to a reduction (avg €2,219.51). My math: ≈ €1.58bn/yr back to insurers (reductions + pre-audit dialogue + penalties). 27 % of audit reasons are coding; 68 % are medical necessity / length of stay.
  - Rules [A]: the BStabG (law, 1 Jan 2027) raises audit quotas to 5/20/40 % (thresholds 80/65 %), with no cap below 50 %, and a €500 penalty and fee. The "switch to sample audits from 2027" in `pain-professionals.md` S3 was a 2024 KHVVG draft and was never enacted, so A14 should fix S3. A 1 % tier for hospitals ≥90 % is pending (Bundesrat 20 Nov).
  - Static simulation on Q2 2026 data: 1,100 of 1,524 hospitals would land in the 40 % tier, and the legal cap rises ~4×. The MD's capacity (2,135 physician FTE) is the real limit. MD Niedersachsen already outsources 20,000 audits (€2m tender).
  - Budget [B] (DKI, Sep 2026): ~4,000 FTE / €245m/yr on audit handling; 51 % of hospitals plan AI for MD audits (median €40k).
  - Incumbents: Tiplu (LOGEX since Jul 2026; MBEG-Assistent in ~30 hospitals; >130 partner hospitals) and calliora (Munich, $6m pre-seed, double-digit hospitals) target exactly the 2027 pain. Also ID Berlin and Dedalus RICO.
  - Inference: big, budgeted, deadline-driven pain, but a crowded window. A newcomer would need a wedge (the payer/MD side, psychiatry/rehab, small private hospitals).
- Not done / blocked: status of the 1 % tier; Q3 2026 statistics (due ~end Nov); GKV-SV/DKG § 17c Abs. 7 report not found; Solventum/3M PDFs blocked (403/404); identity of UK Frankfurt's winner unconfirmed.
- Next: A12. Critic: review `research/hospital-billing-audits.md`.
- Tasks added: A17 (refresh with Q3 2026 data and the 1 % tier decision), inserted before A7.
- Open questions: none new.

### 2026-11-07 — A8 Critic fact-check run 3 (critic)
- Done: fact-checked every research file changed or new since its last review: `research/reimbursement-routes.md` (pass with fixes), `research/munich-ecosystem.md` (pass with fixes), A10 revisions of `research/trends.md` and `research/sources-map.md` (pass). Re-opened ~45 sources; all key numbers match (Bitkom, BStabG/§ 134, PNOG § 11, KHZG penalty annex, DAK, Destatis, Senate answer). TED recipe (637 / 366 cn / 384 procedures / 232 / 140) and ClinicalTrials.gov (300 / 669) reproduce. Reviews: `research/reviews/2026-11-07-*.md`.
- Top issues: (1) SCE Incubation "rolling basis" is not on the SCE page (fixed deadline 2 Aug 2026, passed), and UnternehmerTUM "no equity" is not sourced: the part-time founder path depends on both. (2) A9 still carries the "weak uptake" framing and an unsourced causal claim ("IT capacity, not money") that A10's DAK data contradict; GKV-SV press release graded [A] should be [B]; PNOG Länder co-funding "must" vs draft "sollen". (3) Munich "capital available / B2B workflow AI trend" rests on two deals and omits Bayern VC volume -46% YoY (EY); FLÜGGE "funded up to six projects" is only a plan.
- Not done: pain-* files not re-checked after A14 (A14 still open); ~19 of 43 A9 URLs and ~10 A6 URLs not opened (listed in the reviews); KHSFV § 19 unreachable (connection reset).
- Tasks added: A16 (researcher: apply fixes, combine with A15), inserted before A7.
- Next: researcher A15 + A16, A11-A14; critic reviews new outputs.
- Open questions: none new.

### 2026-11-06 — A10 Apply critic fixes to trends.md and sources-map.md (researcher)
- Done: revised `research/trends.md` and `research/sources-map.md` per both critic reviews.
  - Counts verified [A]: 32,054 care facilities in Dec 2023 (16,505 nursing homes + 15,549 outpatient services, Destatis) and 1,807 hospitals in 2025 (529 public, 549 non-profit, 729 private; Destatis PM 28 Oct 2026). KHZG €4.3bn verified (BMG); DigitalRadar 33.3 → 55.0 (DKG).
  - Framing fixed: the 8.5% FTE cut is a conditional ("müssten"); PNOG and GeDIG are marked as draft everywhere (GeDIG 2nd/3rd reading planned 13 Nov, PNOG 11 Dec 2026); KIM 40% = "applied for"; Pflegestatistik: 800,000 in homes, the definition explains the rise only "zum Teil", 640,000 Pflegegrad-1 people used no services. The old-age-ratio row was correct (33 → 43/45/47 by 2038); I added a note on the second measure.
  - PNOG updated to the cabinet draft: €1.6bn for outpatient **and residential** care, Länder "sollen" co-fund 25%. New: § 113e "Transformationsstellen" lets nursing homes convert up to 10% of the staffing corridor into a tech budget (2028–2032), but only for systems on an evidence catalogue (from 30 Sep 2027).
  - § 8 Abs. 8 grant uptake: DAK processes 48% of facilities. ~11,300 of its ~17,500 used the grant by mid-2025 (64.6%), but only €81.2m ≈ 40% of the funds was drawn. This softens A9's "weak uptake": facilities apply, but small amounts.
  - TED de-duplicated: 637 notices = 384 procedures (366 contract notices = 232 procedures, 139 buyers). Medical-software CPV contract notices: 140 procedures from 110 buyers. Added coverage limits (public buyers only; 729 private hospitals invisible).
  - Job counts downgraded to [C]; kununu needs ≥3 employers; App Store recipe must report the low-star share.
  - New source sections: Munich/Bavaria (KVB, StMGP Krankenhausplan 2026 PDF, Bavarian statistics office, LGL, BKG, AOK Bayern, München Klinik) and provider directories/filings (G-BA quality reports, InEK, AOK-Pflegenavigator, CGM/NEXUS IR, Bundesanzeiger, gematik dashboard = JS only).
  - ClinicalTrials.gov: "Munich" finds 300 recruiting trials, "Munich OR München" 669. A13 must use both spellings.
- Not done / blocked: national (AOK or GKV-SV) uptake of the § 8 Abs. 8 grant not found; incumbent care-software vendors not checked (`[UNVERIFIED]`). Blocked: pflegelotse.de (reset), pflegeportal.bayern.de and lfstat.bayern.de (502).
- Next: A11. Critic: re-check `research/trends.md` and `research/sources-map.md`.
- Tasks added: A15 (update `research/reimbursement-routes.md` with § 113e and the DAK uptake data), inserted before A7.
- Open questions: none new.

### 2026-11-06 — A9 Reimbursement & funding routes for digital health products in DE (researcher)
- Done: `research/reimbursement-routes.md`. 11 routes, each with who decides, amount, timing, evidence and status, almost all from primary law texts and drafts.
  - DiGA: BStabG (in force 30 Jul 2026) adds volume discounts from 2027 (2 % above 3,000 uses/yr, up to 30 % above 100,000) and mandatory first-year price caps. GKV spent €171m in 2025 (0.05 % of GKV spending).
  - DiPA: still zero listed (BMG, Jun 2026). €53/month. Benefits navigation and admin apps are excluded by law.
  - PNOG fund (cabinet 30 Sep 2026): €1.6bn federal + €0.4bn Länder, now also for residential homes. Payouts from 1 Jul 2027; guideline due 30 Jun 2027. My math: ≈€62k per facility over 5 years. Bundestag vote planned 11 Dec 2026.
  - Precedent: the €12k digitisation grant had been used up by only ~20–30 % of facilities in Berlin/Brandenburg by 2024.
  - Hospitals: the transformation fund is not a software budget. No KHZG successor. The KHZG penalty starts weighting actual use: 20 % of it in 2027, 80 % in 2031.
  - Insurers: § 140a contracts are now bound by contribution stability; admin-cost cap from 2027; Innovationsfonds down to €100m/yr.
  - Inference: B2B sales to providers out of their own budgets come first; DiGA/DiPA are later options.
- Not done / blocked: national uptake of the § 8 Abs. 8 grant (only regional vdek data); the current DiGA count (BfArM directory needs JS); the PNOG Bundestag Drucksache (AOK timetable used instead); prevention-course subsidy amounts; PKV. The task's "§64e" is genome sequencing, so § 140a/§ 68a–b were covered instead.
- Next: A10. Critic: review `research/reimbursement-routes.md`.
- Tasks added: none.
- Open questions: none new. Note for B1: suggest that a willingness-to-pay score of 4–5 requires a first revenue route within 12 months that does not depend on a reimbursement listing (`research/reimbursement-routes.md` §7).

### 2026-11-06 — A6 Munich ecosystem: grants, capital, co-founders (researcher)
- Done: `research/munich-ecosystem.md`. Grants (10 programs, with part-time fit), hubs (11), investors (~17), co-founder channels (9), all with sources.
  - Key: the founder stipends (EXIST €2,500/month, FLÜGGE) are not compatible with a full-time job. EXIST allows no active employment and ≤20 h/month of side work, but a sabbatical is OK; applications are accepted until 31 Dec 2027. FLÜGGE requires membership of a state Bavarian Hochschule.
  - Part-time-compatible now: SCE Incubation (≥10 h/week, rolling, prepares for EXIST), UnternehmerTUM Incubator (free, co-founder matching), BayStartUP business plan competition (phase 1 deadline 13 Jan 2027).
  - After founding: Start?Zuschuss! (50 %, max €36k; round 23 planned 25 Nov 2026–10 Jan 2027). EXIST must be approved before founding a company.
  - EIC Accelerator needs TRL 6+. EIT Health (HQ Munich) programmes are closed for now.
  - Competitor signal for A11: Calliora (Munich, AI for hospital billing) raised a >€5.3M pre-seed in Oct 2026 (BHI, Redalpine).
- Not done / blocked:
  - BayTOU 2026 status, INVEST end date and any 2026 BayDiGuP call are unverified.
  - Not opened: Heal Capital (DNS fail / reset), Peppermint and Redalpine (bot check), eu-startups (403). The Munich Startup Insights investor database has been shut down (410).
  - Not covered: pilot partners (Munich university hospitals, insurer innovation units).
- Next: A9. Critic: review `research/munich-ecosystem.md`.
- Tasks added: none.
- Open questions: CEO: is a sabbatical or leaving the job within ~12 months conceivable? EXIST (≈€30k stipend + €30k materials for a team) depends on it. Optional (outward, needs approval): ask SCE / UnternehmerTUM whether a non-alumnus working full-time can join.

### 2026-11-06 — A8 Critic review of Stage A, run 2 (critic)
- Done: reviewed `research/pain-industry.md` (needs work), `research/pain-professionals.md` (needs work) and `research/pain-patients.md` (pass, minor fixes). Re-opened ~45 sources, 9 TED notices (incl. selection criteria), 4 App Store review feeds and the ClinicalTrials.gov counts; nearly all numbers match, App Store and CT.gov counts reproduce exactly. Reviews in `research/reviews/2026-11-06-pain-*.md`.
- Top issues: (1) tenders used as "High WTP" (I5, S3, S8) exclude startups: AOK Hessen requires EUR 6m annual turnover, MUL Lausitz EUR 1m/yr in-field turnover, Charite 3 university-hospital references, Helios a KHZG certificate; DAK's re-tender ("weiterhin") has an incumbent. They prove buyer budget, not startup access. (2) DAK "EUR 890m" is claims volume processed, not contract value; "9 buyers" mixes scanning BPO with billing checks; "1.52m assessments in 2014" is not in the cited vdek page. (3) Harzklinikum "LLM discharge letter" tender is a clinical decision-support system (likely MDR software, needs primary source); A3 [C] counts mix opened threads with titles; ePA app tally picks the worst-rated standalone ident apps.
- Not done: ~40 sources not re-opened (sample-based); Jones Day (Biotech Act) behind Cloudflare on re-fetch. No venture briefs yet (no pre-mortem).
- Tasks added: A14 (researcher: apply A3-A5 fixes, incl. tender eligibility per WTP item), inserted before A7. A8 left open (notes updated).
- Open questions: none new.

### 2026-11-06 — A5 Pain mining: pharma, clinical research, payers, health admin (researcher)
- Done: `research/pain-industry.md`, with 10 problems (I1–I10), each with who has it, who pays, [A]/[B] backing, [C] counts and purchase evidence.
  - Clinical trials (I1/I2), best founder fit:
    - German sites under-recruit: 72 % of university sites miss their plan by ≥25 % (pharma/CRO barometer, Aug 2026).
    - Germany's share of trial participants fell from 4.5 % to ~3 %. My own ClinicalTrials.gov count: industry trials with a German site fell from 15.4 % of all trials (2015) to 10.5 % (2025).
    - Policy is speeding up approvals (MFG, standard contract clauses, EU Biotech Act). Site staff and patient finding remain the gap.
    - Counter-evidence: sponsors rated digital tools a minor hurdle in 2025, and the tool market is crowded (65 trial-management products on Capterra DE).
  - Payers (I5/I6), clearest willingness to pay so far:
    - 9 statutory insurers tendered outsourced invoice/receipt processing since 2025. AOK Hessen: 19.3m invoices over 4 years. DAK: €890m/yr, 2.0m receipts.
    - The MDs are buying AI-assisted assessments (MD RLP care-level assessment pilot, MD Nordrhein malpractice reviews).
    - From 2027, insurers' admin spending may only grow with insured income (§ 4 Abs. 5 SGB V).
  - Other industry pain:
    - EU HTA joint clinical assessment (JCA) dossiers: resource-heavy, but only ~58 JCAs a year and the space is full of incumbents.
    - MDR/IVDR certification: 19.5–21.8 months; 53 % of DACH manufacturers cut R&D. The EU revision proposal (Dec 2025) may shrink this pain.
  - Weak buyers: public-health offices (the federal ÖGD pact ends in 2026) and pharmacovigilance (flat case volume).
- Not done / blocked:
  - The [C] base is thin. Industry pain is not in open forums: Elsmar Cove returned 403, medi-learn has only old career threads, and the krankenschwester.de search needs a session token. Reddit was not used.
  - Primary EU texts were not opened (eur-lex bot check): HTA Regulation, MDR revision, Biotech Act. Law-firm and trade-press summaries were used instead.
  - Not identified yet: the incumbent outsourcers in the payer tenders and the DACH trial-recruitment vendors (snippet only).
- Next: A6 (Munich ecosystem). Critic: review `research/pain-industry.md`.
- Tasks added: A12 (insurer invoice processing and MD assessment automation: incumbents, contract values, buying route) and A13 (clinical-trial recruitment in DE: site economics, vendors, Kapazitätsinitiative 2030), both inserted before A7.
- Open questions: none new. Interviews in Stage D matter more for B2B buyers (sponsors, insurers), whose pain does not show up in public forums.

### 2026-11-06 — A4 Pain mining: clinicians, nurses, practice & hospital staff (researcher)
- Done: `research/pain-professionals.md`, with 10 problems (S1–S10), each with who has it, who pays, [A]/[B] backing, opened [C] counts and purchase evidence.
  - Strongest pain: documentation load. The hospital association institute DKI puts it at 3 h/day for physicians and 2.8 h for nurses (self-estimate). The only measured German study found 93 min/day (19.4 %).
  - Clearest budget owner: hospital coding and MD-audit work. Charité tendered outsourced coding support, Lausitz tendered AI coding software, and DKI ranks MD queries as the most time-consuming duty.
  - Practices: payer requests cost more than 2m hours/yr (KBV), and more than half of practices have weekly TI outages.
  - Funding is shifting. From 2027 the KHZG penalty (up to 2 % per case) starts counting actual *use* of digital services. Under the BStabG, the 2.5 % nurse-relief top-up is clawed back from 2027, and Pflegebudget overruns are no longer refinanced.
  - Counter-evidence: measured AI-scribe gains are modest (16 min per 8 h in JAMA 2026; 15 min per shift in care homes), voize ($50m, 1,100 facilities) already leads in care homes, AI phone assistants are crowded at €9–229/month, and in employer reviews leadership is a bigger complaint than software.
- Not done / blocked:
  - kununu shows page 1 only (the rest sits behind a sign-up, not bypassed), so only kununu's AI summaries were used.
  - krankenschwester.de and medi-learn are low-traffic: 8 threads opened, the rest are titles only. Reddit was not used.
  - LinkedIn job counts are unreliable (fuzzy matching) and StepStone no longer shows counts, so job ads were not used.
  - Not extracted: MD audit volumes, coding incumbents, uptake of the §8(8) SGB XI care-digitisation subsidy.
- Next: A5 (pain mining: industry/payers). Critic: review `research/pain-professionals.md`.
- Tasks added: A11 (hospital billing audits & coding: size, 2027 rule changes, incumbents), inserted before A7.
- Open questions: none new. A Reddit API key would help most for r/medizin and r/Pflege voices.

### 2026-11-06 — A3 Pain mining: patients & caregivers (researcher)
- Done: `research/pain-patients.md`. 11 problems (P1–P11), each with who has it, who pays, [A]/[B] backing, opened [C] signal counts and willingness-to-pay evidence. Strongest: P1 navigating home-care benefits (counselling used by 3% of those entitled, GKV-SV 2026; only 38.4% of Pflegegeld recipients use the relief budget); P2 finding care capacity (91% of home-care services refused new clients, DEVAP 2023); P3 carer overload (WIdO 2026: 46.9% of employed carers highly burdened, €469/month out of pocket); P4 specialist access (25% wait >30 days, GKV-SV 2025). Also: ePA onboarding friction (App Store: 271 of 300 recent reviews of DAK ePA, BARMER eCare and TK-Ident are ≤2 stars), medication shortages, discharge gaps, cancer orientation, rare-disease odyssey (4.7 years, EJHG 2024). Counter-evidence recorded: WIdO finds non-use of care benefits is mainly "no need" or preference, not missing information; the Innovation Fund navigator review found mostly no effect.
- Not done / blocked: [C] base is thin. Reddit was not used; alzheimer-forum.de (403), pflege-forum.org (502), demenz-portal/treffpunkt-pflege (TLS) and patient.info (empty) were unreachable, so P2 and P5 have no opened forum items. ME/CFS, rural GP access and 24-h care figures are snippet-only `[UNVERIFIED]`. Several key data points are >3 years old (flagged in the file).
- Next: A4 (pain mining: professionals). Critic: review `research/pain-patients.md`.
- Tasks added: none.
- Open questions: Reddit API key would mainly help P2, P3, P5 (caregiver and psychotherapy voices).

### 2026-11-06 — A8 Critic review of Stage A (critic)
- Done: reviewed `research/sources-map.md` (pass, minor fixes), `research/trends.md` (pass, minor fixes), `research/scoring.md` (needs work before B1). Re-opened 21 trends sources and re-ran 10 source-map access tests; nearly all numbers match. Reviews in `research/reviews/2026-11-06-*.md`.
- Top issues: (1) the PNOG €1.6bn "budget for a startup" inference ignores the existing §8 Abs. 8 SGB XI care-digitisation grant (max €12k/facility since 2019), whose uptake is the best test of whether grant money becomes purchases; per-facility rules only come with GKV-SV guidelines due 30 Jun 2027. (2) The TED "637 notices" are not de-duplicated (30 of the first 50 are award notices) and half the titles are generic IT; they show public-hospital IT demand, not startup willingness to pay. (3) scoring.md is purely additive (no knock-out for "unclear who pays"), lists DiGA as a 5-level payer example, and has no evidence-confidence dimension.
- Not done: ~19 trends sources not re-opened (sample-based); no venture briefs exist yet (no pre-mortem).
- Tasks added: A10 (researcher: apply trends/sources-map fixes), inserted before A7. A8 left open (notes updated).
- Open questions: CEO: should `research/scoring.md` get knock-out rules (willingness to pay ≤2 or achievability ≤2 → not top 5), a confidence tag per score, and a non-DiGA example for criterion 3 before B1? (Stage B tasks can't be added from Stage A.)

### 2026-11-06 — A2 Source map (nightly researcher)
- Done: `research/sources-map.md`. About 200 URLs across 9 source types were access-tested (curl/WebFetch/WebSearch), each with signal type, grade, access result and recipe. Works: German forums (krankenschwester.de, krebs-kompass, rheuma-online, diabetes forums, onmeda, medi-learn), kununu (incl. review text), App Store API/RSS + Google Play, LinkedIn Jobs/StepStone counts, TED tender API (637 DE hospital IT notices since 2025), G-BA Innovationsfonds (861 projects), CORDIS/EU F&T APIs, BMG/G-BA/Bundestag/insurers, Destatis/Eurostat/OECD SDMX, PubMed E-utilities, Europe PMC REST, ClinicalTrials.gov API, most trade press. Per-task recipes for A3–A6/A9 are included.
- Not done / blocked: Reddit (bot challenge, 0 reddit.com hits in DE `site:` searches; third-party mirrors not used, and the sandbox denied testing them); Facebook/LinkedIn posts (login wall); Google Trends (429); Trustpilot, Indeed, Glassdoor, Crunchbase, Dealroom, OECD web, europepmc.org web, gutefrage, allnurses, Tagesspiegel Background, Ärzte Zeitung, Springer Medizin (bot checks); BA Jobsuche API, Förderkatalog, foerderdatenbank, BAS, SVDGV, Medical Valley EMN (403/502/reset). WebFetch DNS fails for nearly all hosts.
- Next: A3 (pain mining: patients & caregivers). Critic: review `research/sources-map.md`.
- Tasks added: none.
- Open questions: Reddit API key (see Open questions, now more important).

### 2026-11-06 — A1 Trends & policy scan (DE/EU) (nightly researcher)
- Done: `research/trends.md`. Ageing (Destatis 16. kBV), care demand and workforce gap, physicians, chronic disease, hospital reform (KHVVG/KHAG, €50bn fund), digitisation (ePA, GeDIG, FDZ, DiGA, Notfallreform, EHDS, AI Act Omnibus) and cost pressure (GKV/SPV, FinanzKommission, BStabG), each with figures, who is affected and who pays. ~40 sources opened, graded [A]/[B]. Key inference: payers are cutting costs, while new public digitisation money is flowing to providers (PNOG €1.6bn for outpatient care 2027–31, hospital transformation fund). Treat this as input for A7, not as a conclusion.
- Not done / blocked: primary Destatis releases for health spending 2024 and causes of death 2025 (used [B] reports instead); RKI/GBE prevalence data; PNOG cabinet version (used the 5 Jun 2026 draft). WebFetch DNS-blocked destatis.de, bundesgesundheitsministerium.de and vdek.com, so all were fetched via curl. eur-lex.europa.eu returns 202/empty (bot check), oecd.org returns 403, gesetze-im-internet.de does not connect.
- Next: A2 (source map). Critic: review `research/trends.md`.
- Tasks added: A9 (reimbursement and funding routes for digital health products), inserted before A7 because the long list and B1 criterion 3 need it.
- Open questions: none new. (Optional: allowlist eur-lex.europa.eu and oecd.org for primary EU texts.)

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher, run 2)
- Done: verified GLOBOCAN 2024 world/Portugal/Germany figures, CDC colorectal 45–75 gap (B), CDC MMWR lung screening 2017 (A, >3 yrs old); added founder-fit ranking per updated task description; recommendation changed A → C (inference). Rewrote `research/problem-statement.md`.
- Not done / blocked: C, D, E core numbers and A's 2022 national figure still `[UNVERIFIED]` (PubMed/PMC bot check; frontiersin.org and uspreventiveservicestaskforce.org DNS-blocked; ascopubs 403). V1 left open.
- Next: verify C first (it is now the top pick); V10.
- Tasks added: V10 (EU/PT/DACH evidence for C and A).
- Open questions: host allowlist (updated list above); does the CEO agree founder fit should outweigh verified-gap size?

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher)
- Done: drafted `research/problem-statement.md` — 5 candidate problem spaces (A lung screening uptake, B colorectal screening 45–49, C trial enrollment, D financial toxicity, E time-to-treatment), each with problem, who has it, likely payer, key assumptions; provisional recommendation A, runner-up C.
- Not done / blocked: no source could be opened (hosts blocked by network allowlist: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com). All numbers come from WebSearch summaries and are marked `[UNVERIFIED]`. V1 left open with notes.
- Next: verify leads once hosts are allowed; add IARC/EU data.
- Tasks added: none.
- Open questions: host allowlist; US vs EU vs global focus (see Open questions).

### 2026-11-06 — Setup
- Done: created workspace structure.
- Not done: no research yet (by design).
- Next: V1.
