# Progress

## Current state
- Phase: **1 — Validate** (in progress)
- Workspace set up: CLAUDE.md, tasks.json, folders, subagents, routines.
- V1 draft exists (`research/problem-statement.md`): 5 candidate problem spaces, provisional pick = lung-cancer screening uptake. **All numbers `[UNVERIFIED]`** — source hosts were blocked by the network allowlist. V1 still open.
- No interviews conducted. No decisions recorded.

## Next steps
1. CEO: allow research hosts in the session network settings (see open questions), then re-run V1 to verify the leads in `research/problem-statement.md`.
2. CEO picks a problem space from the 5 candidates → record in `decisions/`.

## Open questions
- Which part of the cancer space does the CEO want to focus on (prevention, screening/early detection, diagnostics, treatment access, patient navigation, survivorship, research tooling)? Any no-go areas (e.g. regulated medical devices)?
- Is the CEO targeting B2C, B2B (hospitals, insurers, pharma), or open?
- **Network allowlist blocks primary sources.** Blocked on 2026-11-06: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com. Likely also needed: ncbi.nlm.nih.gov, cdc.gov, cancer.gov, seer.cancer.gov, clinicaltrials.gov, fda.gov, ema.europa.eu, uspreventiveservicestaskforce.org, frontiersin.org, doaj.org, healio.com. Can the CEO allow these? Without it, research cannot meet rule 1.
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
