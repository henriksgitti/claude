# routines/

Exact prompts of the scheduled tasks (CEO-owned; agents must not merge changes here).

| File | Runs | Where |
|---|---|---|
| `researcher.md` | Every 3 hours, 24/7 (UTC); skips the run when no researcher task is open | Worker session (repo attached, env `healthcare-venture`) |
| `critic.md` | Every 6 hours, 24/7 (UTC): skips the run when nothing changed; fact-check when a research file changed; red team only when a current-stage deliverable changed | Same worker session; subagents run in their own git worktree |
| `morning-brief.md` | 07:53 Lisbon | Fresh session; push notification to CEO's phone. The CEO's one detailed briefing per day |

If a prompt changes here, update the scheduled task to match.

Researcher and critic runs end with one line in the worker session's chat. The CEO is briefed once a day by the daily brief, which is built only from the repo; agents therefore write decision-ready log entries in `progress.md` (CEO, 2026-11-14).

Model: Opus 5.5 (`claude-opus-5-5`) for the researcher and critic subagents (spawned with model "opus") and for the daily brief (CEO, 2026-11-14). The worker session that orchestrates the runs keeps the model the CEO selects in that session.
