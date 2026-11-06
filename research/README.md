# research/

Sourced findings, written by the `researcher` agent. One file per task (see `tasks.json` for filenames).

Rules:
- Every factual claim has a source URL inline. No URL → `[UNVERIFIED]`. Grade evidence [A]/[B]/[C] (see `CLAUDE.md` rule 2).
- Start each file with **Findings** (3–7 bullets), then details, then **Sources**.
- Header line: `Task: <id> | Date: YYYY-MM-DD | Status: draft / reviewed`.

`reviews/` holds critiques by the `critic` agent. Researcher responds by updating the research file, not the review.
