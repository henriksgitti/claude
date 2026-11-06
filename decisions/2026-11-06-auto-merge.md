# Agents merge their own PRs
- Date: 2026-11-06
- Decision: Agents open a PR for every session and merge it into `main` themselves, for all files (incl. CLAUDE.md, agents, routines). Builder merges only when all tests pass.
- Reason: CEO does not want to approve every change manually; nightly runs must build on the previous night's work.
- Alternatives considered: auto-merge research only (rules/decisions stay manual); weekly batch merge.
- Revisit if: agents change their own rules unexpectedly, or bad research lands on `main`. CEO can audit via merged PRs and `progress.md`.
