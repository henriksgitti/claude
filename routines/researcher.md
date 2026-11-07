Scheduled RESEARCHER run (Healthcare Venture). The CEO is not available.

1. `git checkout main && git pull origin main`. If unpushed work from an earlier run exists, push it to its claude/ branch first; never discard it.
2. Spawn the `researcher` subagent (Agent tool, subagent_type "researcher") with this prompt: "Read CLAUDE.md and follow it exactly. Take the next researcher task per rule 7 (skip tasks with blocked_by or owner ceo). If there is none, add a progress.md log entry saying so. Go deep: many searches, EN + DE, cross-check sources, grade evidence. Finish per rule 9: commit and push a branch claude/research-<task-id>-<YYYYMMDD-HHMM> created from the latest main. Do NOT open or merge a PR. A critic may run in parallel in its own worktree: keep edits to progress.md / tasks.json / lessons.md minimal. When done, `git checkout main` again. Report: task, branch, key findings, done or what's left, decisions the CEO needs to take, blocked hosts."
3. If a branch was pushed: open a PR into main with the GitHub tools. If it changes CLAUDE.md, founder-brief.md, .claude/agents/, routines/ or decisions/, do not merge: prefix the title with [CEO REVIEW] and leave it open. Otherwise merge it (CEO-approved auto-merge). On conflict: merge main into the branch or rebase it, keeping both sides' entries in progress.md / tasks.json / lessons.md; never force-push over someone else's work. If merging still fails, leave the PR open and state why in its description. Afterwards `git checkout main && git pull origin main`.
4. Reply in this chat with a plain-language summary for the CEO (max 10 lines, no unexplained task IDs or jargon):
   - **What ran:** the task in plain words, and whether it is done.
   - **What we learned:** 2–4 bullets, most decision-relevant first (numbers with their source type, e.g. "official statistics", "one forum").
   - **What it means** for the idea search, incl. anything that contradicts earlier findings.
   - **Decision needed from you:** what, by when, my recommendation, or "none".
   - **Next:** what the next run will do.
   - **PR:** link, merged yes/no. **Blockers:** only if they matter.
