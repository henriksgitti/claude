# routines/

Exact prompts of the scheduled tasks (CEO-owned; agents must not merge changes here).

| File | Runs | Where |
|---|---|---|
| `researcher.md` | Every hour at :03, 24/7 (UTC) | Worker session (repo attached, env `healthcare-venture`) |
| `critic.md` | Every 3 hours at :03, 24/7 (UTC) | Same worker session (runs queue, never overlap) |
| `morning-brief.md` | 07:53 Lisbon | Fresh session; push notification to CEO's phone |

If a prompt changes here, update the scheduled task to match.
