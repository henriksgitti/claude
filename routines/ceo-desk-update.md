CEO DESK UPDATE (scheduled). This chat is Henrik's single entry point (CEO, 2026-11-14): when he opens it he must immediately see what happened and what he must decide, without asking.

1. In /home/user/claude: `git fetch origin && git checkout -q -B main origin/main`. Read progress.md, tasks.json, decisions/, and every research/, research/reviews/, ventures/ file changed on main since the last CEO desk update (or the last 14 hours). List open PRs (GitHub tools) and unmerged claude/ branches. Check the scheduled tasks (list_triggers) for failed or paused runs.
2. Post the update in this chat, plain English, no task IDs or file names except in brackets, every term explained:
   - **Since last update:** one line per finished piece of work and its result; or "Nothing new, because …".
   - **What we learned:** max 4 bullets with numbers and source type, and why each matters.
   - **Where we are:** stage, active/parked ideas, next milestone with estimated time.
   - **Problems:** only if something failed, is blocked or hit a usage limit.
3. Then, for every open decision (tasks with owner "ceo", blocked_by waiting on the CEO, open questions addressed to the CEO, [CEO REVIEW] PRs): give 2–4 lines of context (what, why now, evidence for/against, my recommendation) and ask it with AskUserQuestion answer cards (options with consequences, recommended option first and marked). If none: say "No decisions needed."
4. Do not change the repo in this step unless the CEO answers; when he answers, record the decision (decisions/ file + tasks.json) via a claude/ branch, PR and merge, and fire the researcher if work was unblocked.
