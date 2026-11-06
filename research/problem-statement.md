# Problem statement and assumptions — candidate problem spaces
Task: V1 | Date: 2026-11-06 | Status: draft (blocked — no source could be opened)

> **Read this first.** In this run every source host tried (pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com) was blocked by the session's network allowlist. Only WebSearch result summaries were available, which do not count as "opened" sources. **Every number below is therefore `[UNVERIFIED]`** and must not be treated as fact, built on, or cited until a later run opens the listed URL and confirms it. URLs are listed as *leads to verify*, not as support.

## Findings
- 5 candidate problem spaces proposed (table below): (A) low lung-cancer screening uptake, (B) colorectal-screening gap in newly eligible 45–49-year-olds, (C) low cancer clinical-trial enrollment, (D) financial toxicity for patients, (E) delays from diagnosis to treatment start / care coordination.
- (A) Search summaries report ~18.1% of eligible US adults up to date on lung-cancer screening in 2022 (BRFSS), vs 76.6% breast and 61.4% colorectal `[UNVERIFIED]` — leads: https://pmc.ncbi.nlm.nih.gov/articles/pmid/38856988, https://www.healio.com/news/pulmonology/20261023/uptake-of-lung-cancer-screening-in-us-low-behind-breast-colorectal-cancer
- (C) Search summaries report a 7.1% national participation rate in cancer treatment trials (JCO 2024, Commission on Cancer data), 21.6% at NCI comprehensive centers vs 4.1% at community programs `[UNVERIFIED]` — lead: https://pubmed.ncbi.nlm.nih.gov/38564681/
- (D) Search summaries report a pooled financial-toxicity prevalence of 48% (95% CI 38–58%, 30 studies, COST scale) `[UNVERIFIED]` — lead: https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2023.1266533/pdf
- **Recommendation (inference, provisional):** (A) lung-cancer screening uptake — largest reported gap between eligible and screened, a defined eligible population, and an existing guideline/coverage basis `[UNVERIFIED]`. This recommendation stands only if the numbers verify; the CEO should treat it as a hypothesis to narrow, not a conclusion.

## Details

### Candidate problem spaces
| # | Problem statement (one line) | Who has it | Who might pay (inference) | Key data point (all `[UNVERIFIED]`) | Lead URL to verify |
|---|---|---|---|---|---|
| A | Most people eligible for lung-cancer screening never get screened. | Current/former heavy smokers 50–80 (US USPSTF 2021 criteria `[UNVERIFIED]`) | Health systems, payers (Medicare Advantage, Medicaid plans), employers | 18.1% up to date in 2022; state range 9.7% (WY) – 31.0% (RI); 16.4% under 2021 criteria vs 19.6% under 2013; uninsured 3.7% | https://pmc.ncbi.nlm.nih.gov/articles/pmid/38856988 ; https://ascopost.com/news/march-2024/eligibility-for-and-prevalence-of-lung-cancer-screening-in-the-united-states-in-2022/ |
| B | Newly eligible adults 45–49 rarely do colorectal screening. | US adults 45–49 (eligible since USPSTF 2021 `[UNVERIFIED]`) | Payers (quality measures, e.g. HEDIS COL-E `[UNVERIFIED]`), primary-care groups | 61.4% of 45–75 up to date (BRFSS 2022) vs 29.8% of 45–49; Healthy People 2030 target 72.8% | https://www.cdc.gov/pcd/issues/2025/25_0175.htm ; https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12335306/ |
| C | Few adult cancer patients enroll in clinical trials, especially outside big centers. | Patients at community cancer programs; trial sponsors and sites with slow accrual | Pharma/CRO sponsors, trial sites | 7.1% treatment-trial participation; 21.6% NCI comprehensive centers vs 4.1% community programs | https://pubmed.ncbi.nlm.nih.gov/38564681/ |
| D | Cancer treatment causes financial hardship for about half of patients. | Patients in active treatment and their families | Hospitals (bad debt), employers, payers, patient-advocacy orgs | Pooled prevalence 48% (95% CI 38–58%, I² 99.4%); very high heterogeneity across measures | https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2023.1266533/pdf |
| E | Time from diagnosis to first treatment is growing, and delay is linked to worse survival. | Newly diagnosed patients, esp. those transferring care between institutions | Cancer centers, payers | Median TTI rose 21 → 29 days; 1.2–3.2% absolute mortality increase per week of delay (curative settings, PLoS ONE 2019 — >3 years old); head-and-neck TTI >67 days "unacceptable" | https://doaj.org/article/0910c4e3845c48d9b1b4ec944c98300f ; https://pubmed.ncbi.nlm.nih.gov/39761486/ |

### Key assumptions per candidate (all to be tested; none verified)
| # | Assumption that must hold for a startup |
|---|---|
| A | (1) The main barrier is patient/clinician outreach and logistics, not supply of CT capacity. (2) A payer or health system will pay to raise screening rates (quality bonuses or downstream revenue). (3) Eligible patients can be identified from available data (smoking history is often missing in records `[UNVERIFIED]`). |
| B | (1) Low uptake at 45–49 is an awareness/convenience gap, not just recency of the guideline change. (2) Plans pay for closing quality-measure gaps. (3) Space is not already saturated by at-home stool-test vendors (competitor check needed, V3). |
| C | (1) Community oncologists would refer if matching were easy. (2) Sponsors pay per-enrolled-patient for faster accrual. (3) Data access (EHR) is achievable for a startup. |
| D | (1) A product can measurably reduce out-of-pocket burden (e.g. aid-program matching). (2) Hospitals or employers will pay, since patients in distress are a weak paying customer. |
| E | (1) Delay is driven by coordination failures a software/service product can fix. (2) Navigation programs show benefit — one 2025 JCO OP randomized trial reported timely post-op radiotherapy 74% vs 39% with enhanced navigation `[UNVERIFIED]`, but an AACR 2024 abstract found navigation encounters were not a significant determinant `[UNVERIFIED]` — mixed signal. |

### Why A is the provisional recommendation (inference)
- Largest reported gap (≈18% screened vs ≈61–77% for colorectal/breast) suggests the most room to improve `[UNVERIFIED]`.
- Clear, guideline-defined target population, which makes customer definition (V2) and market sizing (V4) tractable.
- Payer-aligned: screening rates appear to vary by insurance type (Medicare 26.3% vs private 14.4% vs uninsured 3.7% `[UNVERIFIED]`), hinting payers may care.
- Risks: crowded with health-system navigator programs (unknown — V3); CEO may not want US-only focus; lung screening carries false-positive and incidental-finding burdens that need sourcing.
- Runner-up: C (trial enrollment) — clearer B2B payer (sponsors) but harder data access.

## Gaps / [UNVERIFIED]
- **All quantitative claims above are `[UNVERIFIED]`.** Hosts blocked this run: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com. Not attempted (per instruction to stop after repeated blocks): cdc.gov, ncbi.nlm.nih.gov, frontiersin.org, doaj.org, healio.com, uspreventiveservicestaskforce.org.
- No global/EU data (IARC GLOBOCAN, Europe's Beating Cancer Plan) — US-only bias; needed if the CEO targets Europe (routine runs on Lisbon time).
- USPSTF criteria for lung (2021) and colorectal (2021) screening not opened.
- Data for E (PLoS ONE 2019) is older than 3 years.
- No competitor or willingness-to-pay evidence for any candidate (V3, V5).

## Sources
None opened this run. Leads to verify (from WebSearch results, 2026-11-06, not opened):
- https://pmc.ncbi.nlm.nih.gov/articles/pmid/38856988 — lung screening prevalence 2022 (A)
- https://ascopost.com/news/march-2024/eligibility-for-and-prevalence-of-lung-cancer-screening-in-the-united-states-in-2022/ — lung screening 2013 vs 2021 criteria (A)
- https://www.healio.com/news/pulmonology/20261023/uptake-of-lung-cancer-screening-in-us-low-behind-breast-colorectal-cancer — lung vs breast/colorectal comparison (A)
- https://www.cdc.gov/pcd/issues/2025/25_0175.htm — colorectal screening 45–75, BRFSS 2022 (B)
- https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12335306/ — same study, PMC copy (B)
- https://pubmed.ncbi.nlm.nih.gov/38564681/ — cancer trial participation 7.1% (C)
- https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2023.1266533/pdf — financial toxicity meta-analysis (D)
- https://doaj.org/article/0910c4e3845c48d9b1b4ec944c98300f — PLoS ONE 2019 time-to-treatment (E)
- https://pubmed.ncbi.nlm.nih.gov/39761486/ — time-to-treatment study (E)
