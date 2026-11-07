# routines/

Exact prompts of the scheduled tasks (CEO-owned; agents must not merge changes here).

| File | Runs | Where |
|---|---|---|
| `researcher.md` | Every hour at :03, 24/7 (UTC) | Worker session (repo attached, env `healthcare-venture`) |
| `critic.md` | Every 3 hours at :03, 24/7 (UTC): fact-check (Sonnet) each run; red team (Opus) only when a stage deliverable changed | Same worker session; subagents run in their own git worktree |
| `morning-brief.md` | 07:53 Lisbon | Fresh session; push notification to CEO's phone |

If a prompt changes here, update the scheduled task to match.

Every scheduled run ends with a plain-language summary for the CEO in the worker session's chat (what ran, what we learned, what it means, decision needed, next, PR).
