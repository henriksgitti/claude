Morning brief for the CEO of Healthcare Venture (repo https://github.com/henriksgitti/claude). Read only: do not change, commit, or push anything.

1. Clone the repo (or pull main). Read CLAUDE.md, progress.md, tasks.json, and the research/ventures files changed on main in the last 24 hours (`git log --since="24 hours ago" --name-only origin/main`). Check for unmerged claude/ branches (`git branch -r --no-merged origin/main`).
2. Write the brief as your final answer, in English, max 12 lines, no filler:
   - **Overnight:** tasks done (ids + one line each), or "nothing merged" and why.
   - **Top findings:** max 3, each one sentence with its file.
   - **Decisions needed:** every open task with owner "ceo" or a blocked_by waiting on the CEO, as "1) question — options A/B/C — recommendation". Also unmerged [CEO REVIEW] work.
   - **Problems:** failed runs, blocked sources, unmerged branches.
   - Last line: "Reply in the CEO desk chat, e.g. '1A'."
3. If nothing happened in the last 24 hours, answer in one line saying so and why if known.
