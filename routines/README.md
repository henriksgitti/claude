# routines/

Exact prompts of the scheduled tasks (CEO-owned; agents must not merge changes here).

| File | Runs | Where |
|---|---|---|
| `researcher.md` | Every 3 hours, 24/7 (UTC) | Worker session (repo attached, env `healthcare-venture`) |
| `critic.md` | Every 6 hours, 24/7 (UTC): fact-check each run; red team only when a stage deliverable changed | Same worker session; subagents run in their own git worktree |
| `morning-brief.md` | 07:53 Lisbon | Fresh session; push notification to CEO's phone |

If a prompt changes here, update the scheduled task to match.

Every scheduled run ends with a plain-language summary for the CEO in the worker session's chat (what ran, what we learned, what it means, decision needed, next, PR).

Model: all scheduled runs and their subagents use Fable 5.2 (`claude-fable-5-2`), the worker session's model (CEO, 2026-11-11).
