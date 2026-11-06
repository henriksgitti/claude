# CLAUDE.md — Mission Zero Cancer

## Idea
Mission Zero Cancer — exploring startup opportunities in the fight against cancer. The specific problem, customer, and product are NOT yet chosen; Phase 1 exists to find and validate one.

## Mission
1. **Validate** a specific startup idea with real evidence.
2. **Build** an MVP — only after the CEO declares Phase 2.

## Roles
- **CEO (human):** sole decision-maker. Approves phase changes, scope, and every outward action. Writes all interview notes.
- **Agents:** research, build, and critique. They propose; the CEO decides.
  - `researcher` — sourced web research → `research/`
  - `builder` — code with tests → Phase 2 only
  - `critic` — attacks claims and sources → `research/reviews/`

## Rules for all agents
1. **Sources.** Every factual claim needs a source URL. No source → mark it `[UNVERIFIED]` and never treat it as fact, build on it, or cite it as support.
2. **No fabrication.** Never invent progress, interviews, quotes, user feedback, data, or results. If something wasn't done, say so.
3. **No outward actions without CEO approval.** No emails, posts, messages, form submissions, sign-ups, purchases, or spending money. Propose them in `progress.md` under "Open questions" instead.
4. **Session start.** Read, in order: `CLAUDE.md`, `progress.md`, `tasks.json`, `decisions/`, `lessons.md`.
5. **One task per session.** Pick the top open task (first `"done": false` in `tasks.json`, unless the CEO says otherwise).
6. **Session end.**
   - Update `progress.md`: what was done, what's next, open questions.
   - Update `tasks.json` (set `"done": true` only if its definition of done is fully met; otherwise add a `"notes"` field explaining what's left).
   - Add to `lessons.md` if something is worth remembering.
   - Commit to a `claude/` branch (e.g. `claude/competitor-map`). Never commit to `main`.
7. **Be concise.** Findings first, no filler. Tables and bullets over prose.
8. **Medical caution.** This domain involves health claims. Prefer peer-reviewed sources, regulators (FDA, EMA), and registries (WHO/IARC, NCI SEER, ClinicalTrials.gov). Never present medical or regulatory guidance as settled without a source.
9. **Decisions are the CEO's.** Agents never write entries in `decisions/` unless the CEO dictated the decision in the session.

## Definition of done

### Phase 1 — Validate
- [ ] **Problem proven by real evidence:** a specific problem for a specific customer, backed by sourced data AND real CEO-conducted interviews in `interviews/` (not agent assumptions).
- [ ] **Competitors mapped:** direct, indirect, and substitutes, each with source URLs, pricing (if public), and positioning.
- [ ] **Pricing hypothesis:** price point + model, justified by sourced benchmarks.
- [ ] **3 riskiest assumptions listed:** each with how to test it and what evidence would kill the idea.
- [ ] Critic review exists for each core research file, and all `[UNVERIFIED]` items on the critical path are resolved or explicitly accepted by the CEO.
- [ ] CEO records a go / no-go decision in `decisions/`.

### Phase 2 — Build (starts only when the CEO says so, recorded in `decisions/`)
- [ ] **MVP scope** written and approved by the CEO: must-haves, explicit non-goals, success metric.
- [ ] **Tests passing:** all features covered by automated tests; test suite passes on the committed branch.
- [ ] Run instructions in a README; no secrets committed.

## Repo map
| Path | Purpose | Who writes |
|---|---|---|
| `progress.md` | Session log: current state, next steps | Agents |
| `tasks.json` | Task list per phase | Agents (status), CEO (priorities) |
| `research/` | Sourced findings | researcher |
| `research/reviews/` | Critiques of research | critic |
| `decisions/` | Decision log | CEO (or agent transcribing CEO) |
| `interviews/` | Customer interview notes | CEO only |
| `lessons.md` | What we learned about how to work | Anyone |
| `.claude/agents/` | Subagent definitions | CEO |
| `routines/` | Paste-ready scheduled-routine prompts | CEO |
