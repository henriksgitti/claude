# Progress

## Current state
- Phase: **1 — Validate** (in progress)
- Workspace set up: CLAUDE.md, tasks.json, folders, subagents, routines, founder brief.
- V1 draft (`research/problem-statement.md`), run 2: 5 candidates ranked by size × founder fit; provisional pick now **C — clinical-trial enrollment/recruitment**, runner-up A (lung screening). Verified: GLOBOCAN 2024 (world/PT/DE), US colorectal screening gap (B), US lung screening 2017 (A, old). Still `[UNVERIFIED]`: C, D, E core numbers and A 2022 figure. V1 open.
- No interviews conducted. No decisions recorded.

## Next steps
1. CEO: allowlist frontiersin.org, uspreventiveservicestaskforce.org, and an NCBI/Europe PMC API route (see open questions), then re-run V1 to verify C/D/E.
2. CEO picks a problem space from the 5 candidates → record in `decisions/`.
3. V10: EU/PT/DACH evidence for candidates C and A.

## Open questions
- Which part of the cancer space does the CEO want to focus on (prevention, screening/early detection, diagnostics, treatment access, patient navigation, survivorship, research tooling)? Any no-go areas (e.g. regulated medical devices)?
- Is the CEO targeting B2C, B2B (hospitals, insurers, pharma), or open?
- **Network access (run 2, 2026-11-06):** reachable — cdc.gov, gco.iarc.who.int (via WebFetch). Bot/cookie check (not bypassed) — pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov. DNS-blocked — www.frontiersin.org, www.uspreventiveservicestaskforce.org. Proxy 403 — eutils.ncbi.nlm.nih.gov. HTTP 403 — ascopubs.org, cdc.gov via curl (WebFetch works). No response — doaj.org, ascopost.com, healio.com, www.iarc.who.int, www.ebi.ac.uk, api.crossref.org. Allowing eutils.ncbi.nlm.nih.gov or www.ebi.ac.uk (Europe PMC API) would unlock most papers.
- **Network allowlist blocks primary sources (run 1).** Blocked on 2026-11-06: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com. Likely also needed: ncbi.nlm.nih.gov, cdc.gov, cancer.gov, seer.cancer.gov, clinicaltrials.gov, fda.gov, ema.europa.eu, uspreventiveservicestaskforce.org, frontiersin.org, doaj.org, healio.com. Can the CEO allow these? Without it, research cannot meet rule 1.
- Does the CEO want US focus, EU/Portugal focus, or global? V1 leads are US-only.
- Not yet verified: whether scheduled runs have permission to merge into `main`. Check the first run's PR.

---

## Log
<!-- Newest first. Format:
### YYYY-MM-DD — <task id> <task title>
- Done:
- Not done / blocked:
- Next:
- Open questions:
-->

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
