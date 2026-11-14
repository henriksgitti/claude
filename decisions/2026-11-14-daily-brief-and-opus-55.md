# One detailed daily brief; models back to Opus 5.5
- Date: 2026-11-14
- Decision: (1) The CEO is briefed once a day, in more detail, so that he can decide from the brief alone; researcher and critic runs no longer post a summary after every run. (2) All models are switched back to Opus 5.5 (`claude-opus-5-5`). This replaces `decisions/2026-11-11-workers-fable-52.md`.
- Reason: CEO in chat: the per-run summaries did not add up to a briefing he could decide from ("I didn't know how to make a decision based on what"); "Please switch all the models back to Opus 5.5".
- How it is applied: the daily brief (07:53 Lisbon) is longer and decision-ready and runs on Opus 5.5; researcher and critic subagents are spawned with model "opus"; their runs reply in one line and are skipped when there is nothing to do. Prompts: `routines/`. The worker session's own model is set by the CEO in that session.
