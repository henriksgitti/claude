# Problem statement and assumptions — candidate problem spaces
Task: V1 | Date: 2026-11-06 (run 2) | Status: draft (partially verified)

> **Verification status.** Run 2 opened: IARC GLOBOCAN 2024 fact sheets (World, Portugal, Germany), CDC *Preventing Chronic Disease* (colorectal 45–75), CDC MMWR (lung screening, 2017 data). Still not opened: PubMed / PMC (bot/cookie check, not bypassed), frontiersin.org and uspreventiveservicestaskforce.org (DNS blocked by session allowlist), ascopubs.org (HTTP 403). Claims tagged `[UNVERIFIED]` come from search summaries only and must not be built on.

## Findings
- **Scale (verified):** GLOBOCAN 2024 estimates **20 636 441** new cancer cases and **9 762 507** deaths worldwide; lung is #1 in both cases (2 637 005; 12.8%) and deaths (1 861 839; 19.1%), colorectum #3 in cases (2 041 007) and #2 in deaths (917 895). https://gco.iarc.who.int/media/globocan/factsheets/populations/900-world-fact-sheet.pdf
- **Founder home markets (verified):** Portugal 69 439 new cases / 33 590 deaths (colorectum #1 by cases, 10 732; lung #1 by deaths, 5 589). Germany 566 587 / 256 954 (lung #1 by deaths). https://gco.iarc.who.int/media/globocan/factsheets/populations/620-portugal-fact-sheet.pdf ; https://gco.iarc.who.int/media/globocan/factsheets/populations/276-germany-fact-sheet.pdf
- **(B) Colorectal screening gap (verified, US):** "Only 61.4% of adults aged 45 to 75 were up to date with CRC screening, below the Healthy People 2030 target (72.8%)"; 45–49-year-olds: 29.8% (95% CI 28.6%–31.0%), BRFSS 2022 (CDC PCD, 7 Aug 2025). https://www.cdc.gov/pcd/issues/2025/25_0175.htm
- **(A) Lung screening gap (partly verified, old data):** in 10 US states, 2017 BRFSS, 12.7% of adults 55–80 met USPSTF criteria and 12.5% of those reported a screening CT in the last 12 months (MMWR, 28 Feb 2020, **data >3 years old**). https://www.cdc.gov/mmwr/volumes/69/wr/mm6908a1.htm . The newer national 18.1% (2022) figure is still `[UNVERIFIED]`.
- **(C) Trial enrollment 7.1% and (D) financial toxicity 48%** remain `[UNVERIFIED]` (sources not reachable this run).
- **Recommendation (inference, changed from run 1):** rank **C (clinical-trial enrollment / recruitment)** first on combined size + founder fit; **A** second. Reason: `founder-brief.md` names clinical research and AI/automation as the founder's sweet spot and flags a clear B2B payer (sponsors/CROs); A has the strongest *verified* gap signal but is a US-centric, health-system-sold play. C's core number is unverified, so this is a hypothesis for the CEO, not a conclusion.

## Details

### Candidate problem spaces
| # | Problem statement (one line) | Who has it | Who might pay (inference) | Key data point | Status |
|---|---|---|---|---|---|
| A | Most people eligible for lung-cancer screening never get screened. | Current/former heavy smokers (US: USPSTF criteria; 2021 criteria `[UNVERIFIED]`) | Health systems, payers | 12.5% of eligible adults screened in last 12 months, 10 states, 2017 ([MMWR](https://www.cdc.gov/mmwr/volumes/69/wr/mm6908a1.htm)); 18.1% nationally 2022 `[UNVERIFIED]` | Partly verified (old) |
| B | Newly eligible adults 45–49 rarely do colorectal screening. | US adults 45–49 | Payers, primary-care groups | 29.8% up to date (45–49) vs 61.4% (45–75), target 72.8% ([CDC PCD 2025](https://www.cdc.gov/pcd/issues/2025/25_0175.htm)) | Verified |
| C | Few adult cancer patients enroll in clinical trials, especially outside big centers. | Patients at community programs; sponsors/sites with slow accrual | Pharma/CRO sponsors, trial sites | 7.1% participation; 21.6% NCI comprehensive vs 4.1% community `[UNVERIFIED]` | Not verified |
| D | Cancer treatment causes financial hardship for about half of patients. | Patients in treatment, families | Hospitals, employers, payers, advocacy orgs | Pooled prevalence 48% (95% CI 38–58%) `[UNVERIFIED]` | Not verified |
| E | Time from diagnosis to first treatment is growing; delay linked to worse survival. | Newly diagnosed patients | Cancer centers, payers | Median TTI 21 → 29 days; 1.2–3.2% mortality increase per week of delay `[UNVERIFIED]` (2019 data, >3 years old) | Not verified |

### Ranking: size/urgency × founder fit (inference)
Founder fit criteria from `founder-brief.md`: non-clinical founder; strengths in AI-agent implementation and health innovation; interests in drug development and clinical research; PT and DACH access; "big but achievable" (first pilot within ~12 months).

| Rank | # | Size/urgency | Founder fit | Why (inference) |
|---|---|---|---|---|
| 1 | C | High (trials are the bottleneck for new therapies `[UNVERIFIED]`) | **High** | Matches stated interest (clinical research) and the "sweet spot" (trial ops/recruitment); B2B buyer with budget (sponsors); recruitment is a global problem, so PT/DACH sites are a plausible entry. Risk: core number unverified; EHR data access; crowded vendor space (V3). |
| 2 | A | High (lung = #1 cancer killer worldwide, PT and DE — verified GLOBOCAN) | Medium | Biggest *verified* gap signal, but data are US and old; buyers are health systems; EU organised lung screening status `[UNVERIFIED]`. |
| 3 | E | Medium–high | Medium–high | Care coordination / navigation is in the founder's sweet spot; evidence on navigation is mixed `[UNVERIFIED]`. |
| 4 | B | Medium (colorectum #1 by cases in PT, #2 deaths worldwide — verified) | Medium | Verified gap, but at-home test vendors likely already strong (V3); payer-driven US model. |
| 5 | D | High for patients | Low–medium | Patients are a weak paying customer; product fit with AI automation unclear. |

### Key assumptions per candidate (none tested)
| # | Assumption that must hold for a startup |
|---|---|
| A | (1) Barrier is outreach/logistics, not CT capacity. (2) A payer/health system pays to raise screening. (3) Eligible patients can be identified from records (smoking history often missing `[UNVERIFIED]`). |
| B | (1) Low 45–49 uptake is awareness/convenience, not guideline recency. (2) Plans pay to close quality-measure gaps. (3) Not saturated by at-home stool-test vendors (V3). |
| C | (1) Community oncologists would refer if matching were easy. (2) Sponsors pay per enrolled patient. (3) A startup can get EHR/data access (GDPR in EU). |
| D | (1) A product measurably reduces out-of-pocket burden. (2) Hospitals/employers will pay. |
| E | (1) Delay is driven by coordination failures software can fix. (2) Navigation improves outcomes — mixed signal `[UNVERIFIED]`. |

## Gaps / [UNVERIFIED]
- C, D, E core numbers and A's 2022 national figure: unverified. Leads: https://pubmed.ncbi.nlm.nih.gov/38564681/ (C), https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2023.1266533/full (D), https://pubmed.ncbi.nlm.nih.gov/39761486/ (E), https://pmc.ncbi.nlm.nih.gov/articles/pmid/38856988 (A).
- PubMed/PMC show a cookie/bot check; not bypassed (by design). Need an allowlisted API route (e.g. eutils.ncbi.nlm.nih.gov — currently 403 at proxy, or europepmc/ebi.ac.uk — currently blocked).
- USPSTF criteria (lung 2021, colorectal 2021) not opened.
- No EU/PT/DE screening-uptake or trial-enrollment rates yet — needed for a PT/DACH entry (follow-up task V10).
- MMWR lung data are from 2017 (published 2020): >3 years old, 10 states only.

## Sources
- https://gco.iarc.who.int/media/globocan/factsheets/populations/900-world-fact-sheet.pdf — GLOBOCAN 2024 world cases/deaths, top cancers (fact sheet dated Sept 2026), accessed 2026-11-06
- https://gco.iarc.who.int/media/globocan/factsheets/populations/620-portugal-fact-sheet.pdf — Portugal 2024 cases/deaths, top cancers, accessed 2026-11-06
- https://gco.iarc.who.int/media/globocan/factsheets/populations/276-germany-fact-sheet.pdf — Germany 2024 cases/deaths, top cancers, accessed 2026-11-06
- https://www.cdc.gov/pcd/issues/2025/25_0175.htm — colorectal screening 45–75 and 45–49, BRFSS 2022, HP2030 target (B), accessed 2026-11-06
- https://www.cdc.gov/mmwr/volumes/69/wr/mm6908a1.htm — lung screening eligibility/uptake, 10 states, 2017 (A), accessed 2026-11-06
