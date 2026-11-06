# Progress

## Current state
- Project: **Healthcare Venture** (scope opened from cancer to healthcare on 2026-11-06, see `decisions/2026-11-06-scope-pipeline.md`).
- Stage: **A — Scan** (in progress). A1 trends scan drafted (`research/trends.md`); A2 source map drafted (`research/sources-map.md`); A3 patient/caregiver pain drafted (`research/pain-patients.md`, 11 problems); A4 professional pain drafted (`research/pain-professionals.md`, 10 problems). A5 industry/payer pain drafted (`research/pain-industry.md`, 10 problems). Cancer-only work archived in `archive/`; its V1 draft feeds A7.
- Infrastructure: worker session on environment `healthcare-venture`. WebFetch fails DNS for many hosts (destatis.de, bundesgesundheitsministerium.de, vdek.com), but `curl` through the proxy reaches them: fetch with curl + local text extraction. Reddit is effectively unusable: direct fetch is bot-checked and `site:reddit.com` search returns almost no reddit.com hits (A2). Working alternatives and recipes are listed in `research/sources-map.md`.
- No interviews (by design until Stage D). Decisions: see `decisions/`.

## Next steps
1. Researcher: A6 → A9, A10, A11, A12, A13, A7 (one per run), using the recipes in `research/sources-map.md`. Critic: A8 alongside (`research/pain-patients.md`, `research/pain-professionals.md` and `research/pain-industry.md` ready for review).
2. Then B1 (score, top 5) → CEO picks 2–3.

## Open questions
- **Reddit API key (now more important):** A2 found Reddit unreachable (bot challenge; search returns almost no reddit.com hits). A free Reddit app/API key created by the CEO is the only clean route. Without it, A3–A5 rely on German forums, reviews, job ads and tenders.
- Optional allowlist / network change: WebFetch fails DNS for most hosts; curl is blocked by bot checks at trustpilot.com, indeed.com, glassdoor, crunchbase.com, dealroom.co, oecd.org (web), europepmc.org (web), gutefrage.net, aerztezeitung.de, springermedizin.de, background.tagesspiegel.de. Not bypassed.
- CEO: own budget, target date to go full-time, no-go areas (see `founder-brief.md`).

---

## Log
<!-- Newest first. Format:
### YYYY-MM-DD — <task id> <task title>
- Done:
- Not done / blocked:
- Next:
- Open questions:
-->

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
