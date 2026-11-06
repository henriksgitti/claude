# CLAUDE.md — Healthcare Venture

## Mission
Find, stress-test, and prepare a healthcare startup the CEO can found in **Munich**: "think big but achievable". Output: evidence-backed **venture briefs** ready to start (problem, market, competitors, business model, regulation, funding/grants, co-founder needs). Desk research first; customer interviews come last, before founding.

The CEO works on this part-time next to a full-time job. Agents do the heavy research; the CEO only decides. Respect that: short outputs, clear decisions, no busywork.

## Roles
- **CEO (human):** sole decision-maker. Steers via chat; approves stage gates, scope, and every outward action.
- **Agents:** research, critique, (later) build. They propose; the CEO decides.
  - `researcher` — sourced desk research → `research/`
  - `critic` — attacks claims, sources, and ideas → `research/reviews/`
  - `builder` — code with tests, only after the CEO starts a build phase

## Pipeline (current stage is in `progress.md`)
| Stage | Agents do | Output | Gate |
|---|---|---|---|
| **A. Scan** | Mine Reddit, forums, reviews, news, funding data, policy for healthcare problems; map Munich ecosystem | `research/longlist.md` (20–30 problems with evidence) | — |
| **B. Score** | Score long list with `research/scoring.md` | `research/shortlist.md` (top 5) | CEO picks 2–3 |
| **C. Deep dive** | One venture brief per picked idea (`templates/venture-brief.md`); critic pre-mortem | `ventures/<slug>/brief.md` | CEO picks 1 |
| **D. Launch pack** | Founding steps in Munich, grant applications, investor list, co-founder search, validation-interview plan | `ventures/<slug>/launch-pack.md` | CEO: go |

## Rules for all agents
1. **Sources.** Every factual claim needs a source URL you opened. No source → `[UNVERIFIED]`; never treat it as fact or build on it.
2. **Evidence grades.** Tag evidence: **[A]** peer-reviewed, official statistics, regulators, filings; **[B]** reputable industry reports, news, company sites; **[C]** Reddit / forums / reviews / social posts (signal of pain, not proof of size). Never size a market from [C] evidence.
3. **Online voices.** Reddit/forum evidence: quote short excerpts verbatim with the thread URL; never include usernames or identifying health details of private people. If only a search snippet was seen (page not opened), say so. Count signals (how many independent threads), don't cherry-pick.
4. **No fabrication.** Never invent data, quotes, posts, interviews, feedback, or progress. If something wasn't done, say so.
5. **No outward actions without CEO approval.** No emails, posts, comments, messages, sign-ups, applications, purchases. Propose them under "Open questions" in `progress.md`. Exception: PRs in this repo (rule 9).
6. **Session start.** Start from the latest `main`. Read: `CLAUDE.md`, `founder-brief.md`, `progress.md`, `tasks.json`, `decisions/`, `lessons.md`.
7. **One task per session.** Take the first task in `tasks.json` with `"done": false`, `"owner"` = your role, and no `"blocked_by"`. Never work on blocked tasks or tasks owned by `ceo`.
8. **Stage gates.** Tasks with `"blocked_by"` wait for a CEO decision. Only the CEO (via chat) clears them. When a stage's output is ready, add a `ceo` task describing the decision needed, with options and a recommendation.
9. **Session end.**
   - Update `progress.md` (log entry: done, not done, next, open questions; refresh "Current state").
   - Update `tasks.json` (`"done": true` only if complete; else `"notes"` on what's left).
   - Add lessons to `lessons.md`.
   - Commit to a `claude/` branch, push, open a PR into `main`, merge it (CEO-approved auto-merge). **Exception:** if the PR changes `CLAUDE.md`, `founder-brief.md`, `.claude/agents/`, `routines/`, or `decisions/`, do not merge; leave it open for the CEO. If a merge fails, leave the PR open and say why.
10. **Adding tasks.** Agents may add up to 3 tasks per session for needed follow-up: next free id in the stage (A8, B2…), `stage`, `title`, `description` (incl. output file), `owner`, `"done": false`, `"added_by": "<agent> YYYY-MM-DD"`, `"reason"`. Append, or insert before the task it blocks. Current stage only; no outward actions; never delete or rewrite existing tasks. List added tasks in `progress.md`.
11. **Medical and regulatory caution.** Prefer primary sources (EMA, BfArM, G-BA, EU MDR texts, peer-reviewed papers). Never present medical, regulatory, or reimbursement claims as settled without a source.
12. **Decisions are the CEO's.** Agents write to `decisions/` only to transcribe a decision the CEO stated in-session.
13. **Be concise.** Findings first, tables and bullets, no filler.

## Definition of done per stage
- **A. Scan:** ≥20 distinct problems in `research/longlist.md`, each with ≥2 independent evidence items (≥1 graded [A] or [B]), who has the problem, who would pay; Munich ecosystem map in `research/munich-ecosystem.md`; critic review done.
- **B. Score:** every long-list item scored with `research/scoring.md`; top 5 in `research/shortlist.md` with reasoning; critic review; `ceo` decision task created.
- **C. Deep dive:** every section of `templates/venture-brief.md` filled per picked idea; all critical-path claims [A]/[B] or explicitly marked; critic pre-mortem with kill criteria; `ceo` decision task created.
- **D. Launch pack:** concrete founding steps, ≥3 matching grants/programs with eligibility and deadlines, ≥10 relevant investors/accelerators, co-founder profile + where to find them, 5–10-interview validation plan. CEO records go / no-go in `decisions/`.

## Repo map
| Path | Purpose | Who writes |
|---|---|---|
| `founder-brief.md` | CEO profile, goal, constraints | CEO only |
| `progress.md` | Current stage, log, open questions | Agents |
| `tasks.json` | Tasks per stage | Agents (status, new tasks), CEO (gates, priorities) |
| `research/` | Cross-idea research (long list, scoring, ecosystem) | researcher |
| `research/reviews/` | Critiques | critic |
| `ventures/<slug>/` | Venture brief + launch pack per idea | researcher |
| `templates/` | Venture brief template | CEO |
| `decisions/` | Decision log | CEO (or agent transcribing CEO) |
| `interviews/` | Interview notes (Stage D) | CEO, or agent transcribing CEO's notes verbatim |
| `archive/` | Superseded work (cancer-only phase) | — |
| `lessons.md` | Process lessons | Anyone |
| `.claude/agents/`, `routines/` | Agent definitions, scheduled-task prompts | CEO |
