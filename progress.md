# Progress

## Current state
- Project: **Healthcare Venture** (scope opened from cancer to healthcare on 2026-11-06, see `decisions/2026-11-06-scope-pipeline.md`).
- Stage: **C — Deep dive** (since 2026-11-11). C1 done 2026-11-11: `ventures/eldercare-navigator/brief.md` (draft; researcher view: revise, do not go to Stage D as written). Open: C2 (critic review), C3 (CEO decision). Stage B history: B1 done 2026-11-08: `research/shortlist.md` (top 5: L01, L07, L06, L03, L13; all 'unproven', no tier A). Waiting for critic B2 and CEO decision B3. Stage A leftovers: A17 (blocked to 2026-12-01), A24/A26 (deferred), A8 (critic).
- Stage A history: A1 trends scan drafted (`research/trends.md`); A2 source map drafted (`research/sources-map.md`); A3 patient/caregiver pain drafted (`research/pain-patients.md`, 11 problems); A4 professional pain drafted (`research/pain-professionals.md`, 10 problems). A5 industry/payer pain drafted (`research/pain-industry.md`, 10 problems). A6 Munich ecosystem drafted (`research/munich-ecosystem.md`). A9 reimbursement/funding routes drafted (`research/reimbursement-routes.md`). A10 applied the critic fixes to `research/trends.md` and `research/sources-map.md`. A11 drafted `research/hospital-billing-audits.md` (MD audits, 2027 rules, incumbents). A12 drafted `research/payer-processing.md` (insurer § 302 outsourcing, MD AI tenders, buying routes). A13 drafted `research/trial-recruitment-de.md` (CTIS count, 5 % rule, Kapazitätsinitiative, vendors). A14 applied the critic fixes to the three pain files (tender access tables; WTP downgraded where startups cannot bid). A15 added the § 113e Transformationsstellen route and official § 8 Abs. 8 uptake data to `research/reimbursement-routes.md`. A16 applied the fact-check fixes to `research/reimbursement-routes.md` and `research/munich-ecosystem.md`. A17 (partly) confirmed the 1 % audit tier in the Bundestag-passed text and added an 8-quarter 2027 quota simulation to `research/hospital-billing-audits.md`; the Q3 2026 data and Bundesrat vote are still to come. A19 applied the fact-check fixes to the A11–A13 files and `pain-industry.md` (MD-IT: consortia/capacity borrowing allowed; TriNetX–Clinerion now sourced). **A7 long list drafted (`research/longlist.md`): 30 problems L01–L30** (fact-check fixes applied in A21), 6 raw items excluded/merged; new DE data on cancer screening, hybrid-DRG abolition 2028, pharmacy shortage workload, live-in care. Cancer-only work archived in `archive/`; its V1 draft feeds A7.
- Infrastructure: worker session on environment `healthcare-venture`. WebFetch fails DNS for many hosts (destatis.de, bundesgesundheitsministerium.de, vdek.com), but `curl` through the proxy reaches them: fetch with curl + local text extraction. Reddit is effectively unusable: direct fetch is bot-checked and `site:reddit.com` search returns almost no reddit.com hits (A2). Working alternatives and recipes are listed in `research/sources-map.md`.
- (critic 2026-11-08) B2 red team done: `research/reviews/2026-11-08-redteam-shortlist.md`. Recommendation for B3: deep-dive L01 re-wedged (no L03 co-payer); L07 only if a medical-controlling co-founder candidate is named; no brief for L06, L13, L29. Only B3 (CEO) is open in Stage B.
- (critic 2026-11-13) C2 fact-check half done: `research/reviews/2026-11-12-eldercare-navigator-brief.md` (**needs work, minor**; numbers and quotes reproduce, no fabrication). Fix task C4 added (researcher). Still open: C2 red-team half (pre-mortem), C2 idea check (researcher), C3 (CEO).
- No interviews (by design until Stage D). Decisions: see `decisions/`.

- (researcher 2026-11-13) C2 idea check done: `research/idea-prevention-clinics.md`. Verdict: drop the clinic, no deep dive; employer prevention programme only as a cheap test inside the L01 HR conversations. New CEO task C5.
- (critic 2026-11-13) C2 red-team half done: `research/reviews/2026-11-13-redteam-eldercare-navigator-brief.md` (brief **needs work**; employer wedge **fails as a venture case**). Critic task C2 closed; fixes folded into C4 (notes). Open in Stage C: C4 (researcher), C3 and C5 (CEO).
- (researcher 2026-11-13) C4 done: `ventures/eldercare-navigator/brief.md` revised (the one fix round, rule 14). The researcher's recommendation changed: kill criterion K-a is met on desk evidence, so no HR conversations as the next step; keep only the PNOG desk run after 11 Dec 2026. Open in Stage C: C3 and C5 (CEO). No open unblocked researcher task (A17 from 2026-12-01; A24/A26 deferred).
- (critic 2026-11-13) Fact-check run 12: `research/idea-prevention-clinics.md` **passes (minor fixes)** and the C4 revision of the L01 brief **passes (caveats)**: `research/reviews/2026-11-13-idea-prevention-clinics.md`, `research/reviews/2026-11-13-eldercare-navigator-brief-C4.md`. No new task. Every file in `research/` and `ventures/` now has a current fact-check. Open in Stage C: C3 and C5 (CEO).
- (CEO 2026-11-14) **L01 (eldercare navigator as an employee benefit) and the prevention-clinic idea are parked**, not killed. No Stage D, no HR conversations. Research continues with C6 (researcher): screen the parked shortlist ideas L07, L06, L03, L13, L29 on payer, revenue and cash → `research/parked-ideas-screen.md`. C3 and C5 closed. Reporting: one detailed daily brief for the CEO; scheduled runs reply in one line, so everything the CEO needs must be in this file.

- (researcher 2026-11-14) C6 done: `research/parked-ideas-screen.md`. No parked idea is a venture case today; L07 passes the customers × price test (3–5 hospitals for three salaries) but fails on access (Tiplu holds the public tenders; a medical-controlling co-founder is needed). Open: C7 (CEO: L07 cheap tests / back to the long list / L13 skill project / L07 brief).
- (researcher 2026-11-14) C8 run 1 of ~2: FUTRUE benchmark done (`research/futrue-benchmark.md`); consumer-health scan started (`research/consumer-health-scan.md`, 20 candidates, not yet ranked). C8 stays open; next run ranks and adds the CEO decision task.
- (researcher 2026-11-14) C8 done (run 2): `research/consumer-health-scan.md` complete (scored, top 5, cheapest tests). Open: **C9 (CEO: next step on the consumer route)**, C10 (critic review of the two C8 files).
- (researcher 2026-11-14) **C11 done: `ventures/glp1-companion/brief.md`** (GLP-1 self-payer companion, all template sections, one run). Not done: no critic review yet (task C13 added). Next: **C12 (CEO decision)**, C13 (critic).
  - **What I found:** about **100,000** people in Germany paid for weight-loss drugs themselves at the end of 2024 (IQVIA, industry data [B]); they pay €130 to just under €500 a month (Verbraucherzentrale [B]). Where patients pay themselves, fewer than 10 % are still on the drug after a year in some countries (review [A]). The companion job is already covered: the Munich-founded platform GoLighter gives drug customers free nutrition counselling and, since 1 Sep 2026, the Weight Watchers GLP-1 programme for free [B]. Weight Watchers sells that programme for €11.25–45 a month [B], prescription apps are free for BMI 30–40 [B], and ≥25 tracker apps compete in the App Store [C]. Muscle loss is real (25–39 % of the weight lost) but no worse than with dieting (26 %) [A]. GoLighter's own audited 2024 accounts show €9.94m revenue and a €3.12m loss [A].
  - **What it means:** at €30 a month for 6 months (€180 per customer), €1m revenue needs ~5,560 new customers a year, i.e. 5.6 % of all self-payers every year. At the 39–46 % marketing share seen in company filings [A], each customer may cost at most €70–83 to win. No desk source shows whether that is possible. One opening: the free extras stop when people stop buying the drug, and people who stop regain weight [A]. Almost nobody serves them (one small waitlist site, <€129 per 12 weeks [B]).
  - **Options (task C12):** (a) Stage D now: not recommended. (b) One €300, 2-week ad test on the "after the shot" angle with the pass mark set in advance (≥40 sign-ups for €300; kill above €15 per sign-up); you approve the exact ads first. (c) Revise toward a B2B or insurer route: not now. (d) Drop and return to the other options. **Recommendation: (b)**, because acquisition cost decides the case and €300 measures it; if it fails, (d).
- (critic 2026-11-15) C13 fact-check half done: `research/reviews/2026-11-15-glp1-companion-brief.md`. The GLP-1 brief's facts **hold**; the €300 demand-test numbers in sections 5 and 13 do **not** add up (shown price vs revenue price, pass mark per theme, kill line). Fix task C14 (researcher) added. Still open: C13 red-team half, C12 (CEO).
- (critic 2026-11-15) **C13 done (red-team half):** `research/reviews/2026-11-15-redteam-glp1-companion-brief.md`. Verdict: brief **needs work**; as a venture **fail**. The recommended €300 test cannot test the idea (ads may not name the drug, so they reach all dieters; one theme targets people still on the drug). Critic recommends **C12 (d) drop**; fixes go into C14 (no new task).

- (researcher 2026-11-15) **C14 done:** `ventures/glp1-companion/brief.md` revised (the one fix round). One price everywhere (€129 per 12-week programme, bought once); the waitlist test is withdrawn and replaced by a paid pre-order test; recommendation changed to **C12 option (d), drop**. Open in Stage C: **C12 (CEO)**; C10 red-team half (critic).
- (critic 2026-11-15) Second red team of the GLP-1 brief after C14: `research/reviews/2026-11-15-redteam-glp1-companion-brief-C14.md`. Brief passes as a decision document; venture fails; the pre-order test (option b) is closed by the brief's own R3 rule. Both agents recommend C12 (d) drop. Open in Stage C: C12 (CEO), C10 red-team half (critic).

- (researcher 2026-11-18) **C15 done: `research/new-directions.md`** (10 new directions, one run). Not done: the critic review (task C17 added); no per-document price found for the top direction. Next: **C16 (CEO: pick the next direction)**, C17 (critic).
  - **What I found:** (1) **Trial-results documents.** EU law makes every drug-trial sponsor file a results summary and a lay summary after the trial (EMA [A]). In the first compliance study only **116 of 234** due trials reported on time (preprint [B]). About **2,232** new EU trials start each year (repo CTIS count [A]). Paid AI vendors exist (Peer AI raised $12.1m; Yseop is backed by Novartis and Lilly [B]), but no price per summary is published; freelance medical writers charge a median **€82.2 an hour** (EMWA 2023 [B]). (2) **Spin-out co-founder.** The federal spin-out grant (EXIST-Forschungstransfer) pays teams of up to 4 people for 18 months and **requires one business person**; the average grant is >€1m, with 175 applications in 2025 (official [A]). (3) **Lisbon team.** A German-speaking team in Lisbon plus AI has a rare edge (German + Lisbon + AI), but incumbents hold the work and public tenders ask for ≥€2m turnover [A]. Seven other directions fail an old knock-out: pharmacovigilance (needs a qualified-person co-founder), buying a business (capital), DiGA market entry, NIS2, company doctors, prevention courses, health data.
  - **What it means:** in direction 1 one customer brings several trials. At an assumed €5–10k per trial (not sourced), three salaries need 36–72 trial packages a year and €1m needs 100–200, i.e. 4.5–9 % of one year's EU trials (*my math*). Earlier ideas needed 167–279 employers or ~7,750 consumers. Direction 2 pays salaries without customers and fills the founder's science gap, but the CEO does not pick the problem.
  - **Options (task C16):** (a) direction 1 desk run, then a brief; (b) direction 2 desk run (list of Munich spin-outs seeking a business co-founder); (c) both desk runs, then pick one brief; (d) another direction; (e) stop. **Recommendation: (c)**, because both runs are free desk work and each tests a different fix for what sank earlier ideas (direction 1: few customers, legal demand; direction 2: salary and founder gap).
- (researcher 2026-11-18) **C18 done:** fact-check fixes applied to `research/new-directions.md`. New: lay-summary translations are EU-*recommended*, not required (official guidance [A]); EXIST-Forschungstransfer approval rate 27.8 % [A]. C16 options unchanged. Open: **C16 (CEO)**, C17 red-team half (critic).
- (critic 2026-11-18) Fact-check re-check after C18: `research/new-directions.md` **passes (caveats)**: `research/reviews/2026-11-18-new-directions-C18.md`. All fixes hold; no new task. Open: **C16 (CEO)**, C17 red-team half (critic).
- (researcher 2026-11-18) **C19 done: `research/direction1-trial-summaries.md`** (direction 1 desk run). Verdict: **no full brief for direction 1 as framed**; the overdue-report gap is small (Germany 85 trials, Portugal 12) and German universities report on time. Open: **C20** (direction 2 desk run, researcher), C21 (critic fact-check of C19), C17 red-team half. The CEO's pick of one brief follows after C20.
- (researcher 2026-11-18) **C20 done: `research/direction2-spinout-cofounder.md`** (direction 2 desk run: business co-founder of a Munich research spin-out). Not done: nobody contacted (not allowed without approval), so whether any team lacks a business seat is unconfirmed. Added: C22 (critic fact-check), **C23 (CEO: next step after both desk runs)**.
  - **What I found:** (1) **The timing fits.** The federal spin-out grant EXIST-Forschungstransfer has a cut-off on 31 Mar 2027, a jury in June and an "optimal start" on **1 Sep 2027**, your planned full-time date (official handbook [A]). The team is paid as university staff: TV-L E13 is **€4,759–5,106 a month gross** [B]. Every team must include a business person [A], and **87 %** of funded projects found a company, >96 % of which still exist 5 years later [A]. (2) **No open seats are visible.** I found **0** Munich health research projects that publicly advertise a business co-founder. Of 6 co-founder ads, the one open health seat (KIARA) is in Berlin and asks for medtech sales and VC experience [B]. The rest are snippets or non-health. (3) **Two more programmes need a business person in 2027:** Helmholtz Enterprise (projects from Feb 2027 need "a complete team … with CEO competence" by about Oct 2027) [A], and the Bavarian m4 Award 2027 (projects start Nov 2027) [B]. (4) **Part-time is unclear.** Splitting a post into two half-time posts is allowed, but whether that can sit next to a full-time job abroad is not stated [UNVERIFIED]. (5) The 5 best-matching projects are ki-alz-2 (AI Alzheimer diagnosis, LMU Klinikum), SYNTRA (AI-designed RNA delivery, Helmholtz Munich), RadioGene-2 (PET tracking of cell therapies, TUM Klinikum), FormulAIte (AI drug formulation, LMU; seat probably filled) and KIARA (Berlin, seat open). None is confirmed to be seeking.
  - **What it means:** the route is real and the dates line up, but it cannot be moved forward from the desk. Teams fill the business seat through transfer offices and programmes, not ads. You meet the formal bar (Master's, business degree) but not the experienced profile that open ads ask for. Your edge is AI, so AI-heavy projects fit best. Last useful point for a Sep 2027 start: named in a draft application by **28 Feb 2027**.
  - **Options (task C23):** (a) direction 2: approve 3 free outward steps (UnternehmerTUM "Future Entrepreneur" application when it opens in December, 15–20 h/week online; 1–2 Munich events, 1 Dec 2026 and 12 Jan 2027; one question to the EXIST hotline about part-time). The researcher writes a 2-page entry pack. (b) Brief the narrow direction 1 variant (weak, C19). (c) Both. (d) Neither. **Recommendation: (a)**, because it is the only route where the start date, a paid salary and your founder gap line up, and the remaining facts only come from being visible. Cost: your time, not money.

- (critic 2026-11-19) **C21 and C22 done (fact-checks of both desk runs): both files pass with minor fixes; nothing changes the C23 decision.** Reviews: `research/reviews/2026-11-19-direction2-spinout-cofounder.md`, `research/reviews/2026-11-19-direction1-trial-summaries.md`. No fix task. Open: **C23 (CEO)**; C17 red-team half (critic).
- (CEO 2026-11-19) Picked C23 option (c): spin-out route (entry pack C24; the CEO takes the outward steps himself) plus a brief on the narrow trial-summary variant (C25). Kill line: named in a draft EFT / Helmholtz Enterprise / m4 application by 28 Feb 2027. Record: `decisions/2026-11-19-spinout-route-and-trial-brief.md`.
- (researcher 2026-11-19) **C24 done: `ventures/spinout-cofounder/entry-pack.md`** (2-page entry pack, usable as-is). Open: C25 (researcher, trial-summary brief), C26 (critic fact-check of the pack), C17 red-team half (critic). No new CEO decision; three time-critical actions for you are under Open questions.
- (researcher 2026-11-19) **C25 done: `ventures/trial-lay-summaries/brief.md`** (brief on the narrow trial-summary idea). Verdict: a niche service, not a venture-scale company. Added C27 (critic review) and **C28 (CEO: drop / keep as side option / make it the main venture)**. Recommendation: keep as a side option with a €0 test.
- (critic 2026-11-19) **C27 done (red-team half):** `research/reviews/2026-11-19-redteam-trial-lay-summaries-brief.md`. Brief **needs work** (test plan), venture **fails**; the brief's own 'niche service, not venture' verdict is right. Critic recommends **C28 (a) drop**, or at most a lighter (b) that starts with two free desk checks. Fix task C30 added (same fix round as C29). Open: C29 + C30 (researcher, one run), **C28 (CEO)**, C17 red-team half (critic).
## CEO decision 2026-11-14
- **Park both ideas and continue the research.** L01 (eldercare navigator as an employee benefit) and the prevention-clinic idea are parked, not killed. Record: `decisions/2026-11-14-park-l01-and-prevention-clinics.md` (PR open for the CEO).
- **Reporting:** one detailed brief per day instead of a summary after every run.
- Worker session's reading of "continue the research": the desk screen of the parked shortlist ideas that the critic proposed (task C6). Not decided by the CEO: the care-reform (PNOG) desk run after the vote planned for 11 Dec 2026; the 10-minute access check (whom could the CEO call).

## CEO decision 2026-11-11
- **Deep dive on idea 1 only: eldercare navigator as an employee benefit (L01).** Stage C started; C1 unblocked. Other shortlist ideas are parked, not killed.

## CEO decision 2026-11-15
- **GLP-1 companion dropped. All research runs paused** until the CEO sets a new direction. Pool of options when restarting: 'midlife women' consumer brief (menopause + bladder leaks), B2B options (hospital billing-audit tests, long-list re-screen), parked eldercare navigator and prevention clinics.

## CEO decision 2026-11-18
- **Research restarted: new-directions scan** (C15). Research runs back on.

## Next steps
- (2026-11-11) Critic: C2 fact-check and pre-mortem of the L01 brief. CEO: C3 (go to Stage D / revise / drop). Researcher: no open unblocked task after C1 (A17 waits for 2026-12-01; A24/A26 deferred). The numbered list below is from Stage B.
0. **CEO: B3 — pick 2–3 ideas for deep dive** from `research/shortlist.md` (recommendation: L01 + L03 as one 'carer support' brief, plus L07). Critic: B2 review of the shortlist.
1. Researcher: B4 done 2026-11-08. No open unblocked task (A17 waits for 2026-12-01; A24/A26 deferred; C1 waits for B3). Critic: B2 red team (B4 done).
2. After B3: C1 venture briefs for the picked ideas.

## Open questions
- **CEO (C28), from the critic red team of the trial lay-summary brief (2026-11-19, `research/reviews/2026-11-19-redteam-trial-lay-summaries-brief.md`):**
  - Critic's recommendation: **(a) drop it as a venture.** The researcher recommends (b) keep as a side option. You decide.
  - Why, in plain words: (1) the buyer is most likely the contract research firm (CRO) that runs the trial, and it agrees the lay summary in its contract when the trial starts, years before the summary is due; a newcomer would have to sell to a firm that also does the work itself. (2) The work is a medical writer's job plus a standard AI tool; a writer can do it alone, you cannot, so your role in this business is thin. (3) Customers buy once (most small companies end one trial a year), and the whole EU market is about €11m a year at an assumed price.
  - If you choose (b) anyway, approve it only in this order: first two **free desk checks** by the researcher (who is named as writer of 30 published lay summaries; how often trials in several countries run through big CROs), task C30. Only if those pass: one call with a freelance medical writer and one with a small CRO's writing lead (outward, needs your OK). Do **not** count on the spin-out events for these conversations: the people there are founders and researchers, not the trial managers who would buy.
  - The €0 quality test in the brief cannot give a clear answer as written (nobody qualified checks the result, and the AI may have seen the published answer). C30 fixes or drops it.
  - Time check: if you get named in a spin-out application (kill date 28 Feb 2027), you will not have time for this side option too.
- **CEO (C28), trial lay-summary brief (2026-11-19, `ventures/trial-lay-summaries/brief.md`):** outward steps to approve if you choose option (b), none done: 5 phone or event conversations with DACH small sponsors and small CROs (names from public CTIS data, section 9 of the brief), alongside the spin-out events Jan–Mar 2027. No cold emails: German law requires prior consent for email advertising (§ 7 UWG). Later, only if these pass: EMWA membership and a medical-writer co-founder search.
- **CEO, actions from the spin-out entry pack (2026-11-19, `ventures/spinout-cofounder/entry-pack.md`; you approved these steps on 19 Nov; agents did nothing outward).** Time-critical, in date order: (1) **now:** join the waitlist for the TUM Healthcare Happy Hour on 12 Jan 2027. It is free but already full (Luma page, 19 Nov). (2) **24 Nov:** free online UnternehmerTUM info session; sign up for the "notify me" alert, because the Future Entrepreneur application opens in December on a date not yet published. (3) **1 Dec, 16:45:** Munich Impact Co-Founder Matching, Lothstraße 21. (4) **Any time:** the EXIST hotline question (German text in §4 of the pack). Expect a "no" on working half-time next to your Lisbon job: German law adds up hours across employers and caps them at an average of 48 a week ([A]; whether it applies across borders is unverified). Then the plan is: help write the application unpaid until Feb 2027 and start full-time on 1 Sep 2027. Before you use the pitch, check one line: it says you will work full-time **in Munich** from Sep 2027.
- **CEO (C23), after both desk runs (2026-11-18, `research/direction2-spinout-cofounder.md`):** pick (a) direction 2 with 3 free outward steps (recommended), (b) narrow direction 1 brief, (c) both, (d) neither. Outward actions to approve (none done): UnternehmerTUM Future Entrepreneur application (opens Dec 2026); Munich Impact Co-Founder Matching (1 Dec 2026, Precelerator); TUM Healthcare Happy Hour (12 Jan 2027); one EXIST hotline question (may a half-time grant post run alongside a full-time job abroad?). Later, only if (a): contact LMU Spin-off Service / Helmholtz Munich transfer / TUM Venture Lab Healthcare about teams lacking a business seat. 10-minute check: would you move to Munich by Sep 2027 for a university-paid post (~€4.8k gross/month) on a project whose science you did not choose?
- **CEO (after C20), direction 1 result (2026-11-18, `research/direction1-trial-summaries.md`):** researcher's view: do not brief direction 1 as framed; keep the narrow CRO-subcontract variant as fallback if direction 2 also fails. Outward actions to approve later (not now): EMWA membership (find a medical-writer co-founder); a visit to DIA Europe 2027 (Basel, 16–18 Mar).
- **CEO (C16) note from the critic fact-check (2026-11-18):** the facts behind the new-directions scan hold; fixes are labels and wording (task C18). Before choosing: the language edge for idea 1 is unproven, and the EXIST spin-out grant funds about 1 in 4 applications (27.8 %).
- **CEO (C16), new directions (2026-11-18, `research/new-directions.md`):** pick (a) trial-documents desk run, (b) spin-out co-founder desk run, (c) both (recommended), (d) another direction, (e) stop. 10-minute check: do you know a medical/regulatory writer, a clinical-operations person at a small biotech or a university trial centre (KKS), or a TUM/LMU/Helmholtz researcher planning a spin-out? Outward actions to approve later (not now): 5 calls with sponsors' clinical-operations leads; signing up to one co-founder matching programme.
- **CEO (C12), from the critic's second red team of the GLP-1 brief (2026-11-15, `research/reviews/2026-11-15-redteam-glp1-companion-brief-C14.md`):**
  - Both agents now recommend **(d) drop**. Nothing in the revised brief argues against it.
  - If you consider **(b), the paid pre-order test**, three warnings: (1) the brief's own rule says "run it only if no competitor offers people who stop the drug a path at €15 a month or less"; Weight Watchers does (€11.25 a month, open to anyone), so by that rule the test is off today. (2) The only concrete channel is a post in a small GLP-1 forum; that shows whether a friendly crowd buys, not what a customer costs to win, and it says nothing about other consumer themes. (3) If 10 people pay, you must run a 12-week programme with a qualified nutrition professional you have not found yet, or refund everyone.
  - If what you really want is the cost of winning a paying consumer, test it on the idea you would actually pursue next, with normal paid ads.
  - 10-minute check: can you name one nutrition professional who would run a 12-week group for a fee, and one person who runs paid ads in health or diet?
- **CEO (C12), from the critic red team of the GLP-1 brief (2026-11-15, `research/reviews/2026-11-15-redteam-glp1-companion-brief.md`):**
  - Critic's recommendation: **(d) drop the GLP-1 companion as a venture.** Reasons in plain words: the free bundles already cover people on the drug; for people who stop, a one-person site already offers the same programme; the product lasts 12 weeks, so each customer brings only €83–129 and may cost at most about €32–59 to win; Germany-wide the market is about €18m a year even if everyone bought. A seed investor would not fund this.
  - **Do not approve the €300 test as written in section 13, even after C14.** Without naming the drug the ads reach everyone who wants to keep weight off (Weight Watchers' market at €11.25 a month), and the second theme ("low appetite") targets people still on the drug. Whatever comes out would not answer the question.
  - If you still want to measure what a paying consumer costs to win (useful for the midlife-women theme too): approve instead one free desk run first (do GoLighter, Juniper, Voy or Weight Watchers already offer anything to people who stop? T1), and only then a redesigned test: one theme, a channel that reaches people stopping the drug, a paid pre-order with refund instead of an e-mail waitlist. Pass = 10 or more paid pre-orders for €300; stop = fewer than 6. This is an outward action and needs a seller set-up (imprint, payment); you approve the exact ads.
  - 10-minute check, sharper than before: do you know a **performance marketer** (paid ads in health or diet)? That skill, not AI, decides this kind of business.
- **CEO (C12), from the critic fact-check (2026-11-15):** if you choose (b), approve the €300 test only after C14 has fixed the numbers (one price on the page and in the maths; pass mark per €150 theme; kill line tied to the €70–83 allowance). The facts behind the brief hold.
- **CEO (C12), GLP-1 companion (2026-11-14):** decide (a) Stage D / (b) €300 demand test on the "after the shot" angle / (c) revise to B2B / (d) drop. Recommended: (b). If (b), also decide on one paid lawyer hour (about whether ads may name people who use the "Abnehmspritze"); without it the test uses neutral wording only. 10-minute check: do you know a nutrition scientist, a physician in nutritional medicine, or a performance marketer you could call?
- **CEO (C8), product types (2026-11-14; run 2 applied the default: homeopathy excluded, evidence scored; you can still overrule):** which product types are acceptable? FUTRUE's biggest OTC line is homeopathic remedies. Options: (a) only products with published evidence (supplements/devices with trials; mission fit "tackle healthcare problems"); (b) any legal self-pay product. Researcher's recommendation: (a), because weak-evidence products carry claim-law and reputation risk and do not fit your stated goal. If you do not answer, run 2 scores 'evidence base' as a criterion and flags homeopathy as excluded.
- **CEO (C8), 10 minutes:** do you know a pharmacist or physician who could own product claims, or a performance marketer? The FUTRUE pattern needs both.
- **CEO (C3), from the second red team of the L01 brief (2026-11-13, `research/reviews/2026-11-13-redteam-eldercare-navigator-brief-C4.md`):**
  - Decide C3 now; do not wait for the vote planned for 11 Dec 2026. No outcome of the vote reopens the employer wedge. The care-reform desk run can stay, as a new long-list check (Kassen as buyer), not as a condition on L01.
  - If you choose (c): before a brief on L07 or L11, approve one desk run that puts the parked ideas (L07, L06, L13, L29) through the test that stopped L01 (customers x sourced price for three salaries and for EUR 1m ARR, strict K1/K2, cash to month 24)? Critic's recommendation: yes. Not added as a task (stage gate; your call).
  - 10-minute access check, widened to all parked ideas: which of these could you call this week: an HR/benefits lead, a qualified care adviser, a hospital medical controller or coder, a Kasse department head?
- **CEO (C3 + C5), consistency note from the critic (2026-11-13):** C5 option (b) puts two prevention questions into the L01 HR conversations. After C4 the researcher no longer recommends those conversations (kill criterion K-a met). If you choose C3 (c) or skip the conversations, C5 (b) has no carrier: it then means "drop" unless you approve separate calls.
- **CEO (C3), after the C4 revision of the L01 brief (2026-11-13):** researcher and critic now agree on substance. The employer wedge is at best a small service business (best case 60 customers = €359,000 ARR, enough for three modest salaries; €1m ARR needs 167–279 customers; no price above ~€6,000 a year at a private employer is shown). Decide: (c) drop the employer wedge and keep one desk run on the care reform after the vote planned for 11 Dec 2026 (recommended by both), or (b) HR conversations anyway, with screening K-e and signed paid pilots K-f as the bar. The text of task C3 still shows the older recommendation (b). This also decides C5 option (b), which rides on those conversations.
- **CEO (C5), prevention clinics (2026-11-13):** drop / keep the employer variant as two extra questions in the L01 HR conversations (recommended) / deep-dive anyway? Free check: do you know a physician in Munich who would own the practice? Outward action proposed only if the idea stays alive: one paid hour with a medical-law attorney on the broker model in Bavaria.
- **CEO (C3), from the red team of the L01 brief (2026-11-13, `research/reviews/2026-11-13-redteam-eldercare-navigator-brief.md`):**
  - Critic's recommendation: **(c) drop the employer wedge**, keeping one desk run from (b): the PNOG as passed (vote planned 11 Dec 2026) plus who holds today's delegated § 7a counselling contracts. Reason: the brief's own best case (60 customers, €359,000 ARR) does not pay the three people it needs, and no HR conversation can change that. The researcher recommends (b). You decide.
  - If you prefer (b): approve the HR conversations only with the rewritten kill criteria (K-e screening, K-f signed paid pilots). This also affects C5, which piggybacks on those conversations.
  - Extended 10-minute check: can you name one HR/benefits lead **and** one qualified care adviser (Pflegeberater:in) you could call?
- **CEO (C3), from the L01 brief (2026-11-11):**
  - Approve 5–8 conversations with HR/benefits leads at Munich-area firms of 150–1,000 staff? (outward action; questions in the brief, section 13). It is the only way to test "who pays a new small company".
  - The care reform bill (PNOG, BT-Drs. 21/8869) would give every care recipient a free digital "Pflege-Cockpit" by 1 Jul 2028 and free "Pflegebegleitung" from 1 Jan 2029 (~€760m a year; Kassen may hand it to third parties). Should the researcher check, after the Bundestag vote planned for 11 Dec 2026, whether serving that new task is a better wedge than employers? It is a different buyer (Pflegekasse / municipality).
  - 10-minute founder-access check: do you know one HR/benefits lead at a firm with ≥150 staff?
- **Reddit API key (now more important):** A2 found Reddit unreachable (bot challenge; search returns almost no reddit.com hits). A free Reddit app/API key created by the CEO is the only clean route. Without it, A3–A5 rely on German forums, reviews, job ads and tenders.
- Optional allowlist / network change: WebFetch fails DNS for most hosts; curl is blocked by bot checks at trustpilot.com, indeed.com, glassdoor, crunchbase.com, dealroom.co, oecd.org (web), europepmc.org (web), gutefrage.net, aerztezeitung.de, springermedizin.de, background.tagesspiegel.de. Not bypassed.
- ~~CEO: own budget, no-go areas, target date~~ Answered 2026-11-07: €10k own money, no no-go areas, full-time from September 2027 (`founder-brief.md`).
- ~~CEO decision before B1: replace the scoring method?~~ **Decided 2026-11-07 (chat): option (b) + confidence ranking.** `research/scoring.md` now has knock-outs K1/K2 and confidence rules R1–R4 (H/M/L per score, L capped at 3, tiers + sensitivity check). Still useful for founder fit: the 10-minute founder-access check in the red-team review ("Cheapest tests" 1).
- **CEO decision before B1: approve the scoring v2 fixes?** `research/reviews/2026-11-07-redteam-scoring-v2.md` lists 10 one-line edits to `research/scoring.md` (must-fix 1–6: K2 needs a sourced example of the route in use, else 'K2 unproven'; buyer-specific direct-award limits incl. § 22 Abs. 2 SVHV ≤€50k for insurers; score per A18 wedge; define K1 'category' and 'in force'; define tiers and the R4 order; separate M from L). Recommendation: approve 1–6 now; 7–10 optional. **Decided 2026-11-07 (chat): only fixes 1–6 approved; 7–10 not applied.** A20 unblocked.

- **B1 note (2026-11-08):** the open scoring questions below were not applied; `research/shortlist.md` caveats C1–C7 show their effect. Only slots 4–5 move (L03 ↔ L29); the top 3 hold.

- **CEO (quick, before B1): how is "≤5 years old" in K2 fix 1 measured?** Today, or at the time of the first paid sale? Today excludes voize (founded 2020; named customer) as evidence for L05. Also: does a vendor claim of unnamed customers (calliora: "private, public and church hospitals in five states") count? As written: no. Recommendation: measure at the time of the sale; keep "named" strict. See calibration note in `research/scoring.md`.

- **CEO (before B1), from the red team of scoring v3 (`research/reviews/2026-11-07-redteam-scoring-v3.md`): approve 4 one-line edits?**
  - S1: fill the top 5 from tier B by R4 total instead of base total.
  - S2: the K2 example vendor must appear in criterion 8; if it is the category leader, criterion 8 ≤ 2.
  - S3: a channel counts only if it is open to new entrants.
  - S4: wedges are fixed in A18 before scoring, and the top 5 holds at most one wedge per signer cluster.
  - Also: does the 12-month clock start in Sep 2027 (S6)?
  - Recommendation: approve S1–S4 and the Sep 2027 clock.
- **Critic view on the two questions above:** "≤5 years" = vendor age at its earliest named paid sale to this signer type, sale dated 2021+, vendor independent (not a JV/subsidiary of an incumbent). Unnamed customer claims count only with one independent confirming source; otherwise "K2 unproven" (not a knock-out).
- **CEO, 10 minutes, no outreach (most valuable test before B1):** for each of the ~10 signer clusters in `research/reviews/2026-11-07-redteam-longlist.md` F3, do you know one person who signs such purchases or has bought from a company <3 years old? Without this, founder fit scores 4 M on nearly every row and separates nothing.

- **CEO (before B1), from the red team of A18 (`research/reviews/2026-11-07-redteam-longlist-fields.md`):** under v3, triggers in force before Sep 2027 pass K1 but are captured by incumbents before you go full-time, while 2028 triggers (GOÄ, § 113e, short-stay flat rates) fail K1 as bills. Should K1 accept a budget line "in force by the start of the 12-month clock" (ties to S6)? Recommendation: yes, if the 12-month clock starts Sep 2027, tagged L until the law passes. Also: only L01 (employer eldercare benefit) combines an open route with a €100m+ ceiling; expect the shortlist to say so.

- **CEO (B3), from the B2 red team (`research/reviews/2026-11-08-redteam-shortlist.md`):** (1) New TED evidence: employers buy eldercare counselling inside family-service frameworks (MPG Munich, pme, EUR 1.2m, 2025; federal agencies, awo lifebalance, 2025; TenneT, pme, 2026). So strict K1 keeps L01 in, but bundlers (pme, awo, famPlus in Munich) hold the buying unit. The L01 brief must choose between B2B to the bundlers and mid-size employers without a contract. (2) Drop L03 as co-payer (two signers; a free Kasse course undercuts L01). (3) L07 only if you can name a medical-controlling/coding co-founder candidate (10 min). (4) Optional: reopen L11 (founder-specific: German + Portuguese) by running the deferred A26 per-hire-fee test. (5) Outreach for approval: 3 conversations with HR/benefits leads at Munich firms of 250–2,000 staff (questions in the review).

---

## Log
### 2026-11-19 — Red team: trial lay-summary brief (C27, second half) (critic, RED TEAM)
- **Done:** red team of `ventures/trial-lay-summaries/brief.md` as a buyer and as a Munich seed investor: `research/reviews/2026-11-19-redteam-trial-lay-summaries-brief.md`. Verdict: **brief needs work** (test plan and kill lines), **venture fails** (agrees with the brief; "niche service, not venture" is not too harsh). One new count from the EU trial register (all 4,202 ended trials, public search): of 2025 trials by "other" drug companies, ~38 % are early-phase or generic bioequivalence studies (usually templated in-house) and ~49 % run in one country only (one language, so the translation part of the pack, its main value, is small).
- **Top issues:** (F1) the buyer is probably the CRO, at trial start, not the sponsor at close-out; R1's "outside purchase" would count a CRO line item as a pass. (F2) the CEO is the least necessary person: a medical writer can sell this alone. (F3) realistic market ~400 trials EU-wide (~€1.4–2.4m a year), not 702. (F4) the €0 quality test has no qualified judge and may test the AI's memory; its writer-time kill cannot be measured. (F5) the spin-out events do not reach trial buyers; cold phone calls rest on narrow legal ground.
- **Cheapest tests:** T1 desk check of who wrote 30 published lay summaries; T2 desk check of CRO share for multi-country trials. Both free; if T1 shows CRO or in-house templates dominate, drop without any outward step.
- **Not done:** no outward action; the T1/T2 desk checks are left to the researcher (C30). C17 red-team half still open.
- **Tasks:** C27 marked done. Added **C30** (researcher: red-team fixes plus T1/T2, in the same run and fix round as C29). After C29+C30, remaining issues become caveats (rule 14).
### 2026-11-19 — Fact-check: trial lay-summary brief (C27, first half) and spin-out entry pack (C26) (critic, FACT-CHECK)
- **Done:** checked `ventures/trial-lay-summaries/brief.md` (34 of 34 sources opened, plus my own re-count of the EU trial register: all 3,388 trials that ended in 2025–26 read one by one) and `ventures/spinout-cofounder/entry-pack.md` (26 of 26 sources opened). Verdicts: **brief: needs work (1 critical, 9 minor)**; **entry pack: pass (minor fixes)**. No invented interviews or contacts in either file.
- **Entry pack: what holds.** Every date and contact in the pack is right: UnternehmerTUM info session 24 Nov; m4 deadlines 30 Nov / 13 Jan / 22 Feb; co-founder matching 1 Dec (doors 16:45); TUM Happy Hour 12 Jan is free but full (waitlist open); LMU Demo Day 3 Feb; EXIST hotline number and e-mail (and the hotline really asks you not to send documents). The working-hours point holds: German law adds up hours across employers and caps them at 48 a week, so a full-time job plus a half-time grant post (~60 h) does not fit; whether that applies with a Portuguese employer is still open, which is why it is a hotline question.
- **Entry pack: what to correct before you use it (you can do this yourself):** (1) The profile says "I am German" and "know Munich and Lisbon"; `founder-brief.md` says only "German-speaking" and a Lisbon network. Keep them only if true. (2) "LMU's incubator is closed to outsiders" is too strong: a team needs one LMU-linked member, so you can join an LMU team. (3) "A named start-up role by March 2027" via Future Entrepreneur is a guess; the next batch dates are not published. Also worth knowing: funded m4 projects start in **November 2027**, two months after your planned 1 Sep start.
- **Brief: what holds.** The legal duty, EMA's official figures (companies on time 83.8 %, overdue 5.9 %), the UK rule, the AI studies and all the money maths check out. My re-count matches the brief exactly on the main numbers: 1,826 trials ended in 2025; companies based in Germany ended 43 (30 companies); EU-based 315. The US finding (about 70 % of US biotech trials run through big CROs) holds.
- **Brief: what was wrong.** (1, critical) The Bottom line says "a vendor's ~50,000 AI summaries were taken offline after accuracy concerns". No source says that. One source reports that one vendor (TrialAssure) published ~50,000 AI summaries; another says that an unnamed set of AI summaries was removed in 2023. The brief merged the two into a claim about a named company. The same sentence is in the C25 log entry above. (2) The "small and mid-size companies" group also contains large private firms (Grünenthal, Merz, Medac, Hexal), so that segment is a bit bigger and less "small" than labelled. (3) The big-CRO list is not written down, so the EU and German CRO counts cannot be re-run (mine are lower: 74 vs 85 EU, 9 vs 13 Germany). (4) The Bottom line leaves out one study where people understood human-written summaries better than AI ones.
- **Does it change a decision?** No. Your C28 options and the researcher's recommendation (b) rest on facts that hold; the corrections make the AI-quality case a little weaker and the market a little smaller, not bigger. You can decide C28 now or after C29.
- **Not done:** red-team half of C27 (is the CRO route fair, are the kill lines testable, is "niche service, not venture" right) needs a separate RED TEAM run; C17 red-team half also still open. No outward action.
- **Tasks:** C26 marked done. C27 notes updated (fact-check half done). Added **C29** (researcher: fix the brief per the review; the brief's one fix round under rule 14). Appended at the end of `tasks.json`; it should run before the CEO decides C28 if you want the corrected text.
### 2026-11-19 — C25: venture brief, AI lay summary + translation pack for trial sponsors (researcher)
- **Done:** `ventures/trial-lay-summaries/brief.md`, all 13 template sections. New since C19: my own count of all **3,388** EU trials that ended in 2025–2026 (who the sponsor is, where it is based, which contractors it uses), EMA's first official compliance figures, the new UK rule, 4 studies on AI-written summaries, and a cost estimate per pack. About 35 pages and papers opened. Nobody contacted.
- **What I found:**
  1. **The work is required by law, but the whole market is small.** Every EU drug trial must publish a plain-language results summary within 12 months (EU law [A]). 1,826 trials ended in 2025 [A, own count]. If every one bought a €6,000 pack, the EU market would be about **€11.0m a year**; the small and mid-size company part is **€4.2m** (*my math*). Nobody publishes a price, so €6,000 is still an assumption.
  2. **Germany and DACH are too small on their own.** Small/mid companies based in Germany ended **43** trials in 2025, DACH **81** [A, own count]. Even with every one of them as a customer, revenue would be **€258k** (Germany) or **€486k** (DACH). The biggest group is **US biotechs (262 trials)**, and **71 %** of their trials run through large CROs [A, own count].
  3. **Fines are not the driver.** EMA's first official figures (Sep 2026) show companies on time in **83.8 %** of cases; only 5.9 % of company trials are overdue [A].
  4. **AI can draft, but a human must check.** In a blinded trial, AI summaries scored as well as or better than human ones [A], and AI saved writers over 40 % of their time [A]. But only **12.3 %** of 1,010 patients trust AI-only documents "a lot" [A], EMA expects "close human supervision" [A], and in 2023 a vendor's ~50,000 AI summaries were taken offline after accuracy concerns [B]. A medical writer is needed, and you are not one.
  5. **Margins are service margins.** Direct cost is about **€1.8–2.4k** per pack (writer time plus 4 translations, *my math*). Gross margin is 31–50 % at €3,500 and 60–71 % at €6,000. The same model (AI draft + human check) is already sold by at least one small firm (SciencePOD) and by CROs [B].
- **What it means:** this can be a small service firm, not a company that raises seed money. €1m revenue would need about one in four small-company trials in the whole EU, mostly sold through CROs. One fact decides it, and no desk source has it: does any small sponsor or CRO pay an outside firm ≥€2,500 for a lay summary?
- **Options (task C28):**
  - **(a) Drop it now.** Nothing more happens; the effort goes into the spin-out route.
  - **(b) Keep it as a side option (recommended).** In December I (or you) run a €0 quality test on 3 public trials. With your OK, you then hold 5 phone or event conversations with DACH small sponsors and CROs alongside the spin-out events (Jan–Mar 2027). Kill line, fixed now: fewer than 2 of 5 report paying an outside firm ≥€2,500.
  - **(c) Make it the main venture** and start the medical-writer co-founder search now. The market size does not support this.
  - **Recommendation: (b).** It costs no money, uses events you already plan to attend, and gives you a concrete trial topic for spin-out conversations. You can also wait for the critic review (C27) before deciding.
- **Not done:** no price observed (6 more searches; 0 tenders). Who signs in practice (sponsor or CRO) is inferred, not surveyed. Writer hours with AI on real EU trial documents are not measured anywhere.
- **Tasks:** C25 done. Added **C27** (critic: fact-check + red team of the brief) and **C28** (CEO decision). Next researcher task: none unblocked (A17 from 1 Dec 2026).
### 2026-11-19 — C24: entry pack for the spin-out co-founder route (researcher)
- **Done:** `ventures/spinout-cofounder/entry-pack.md` (task C24). It has five parts: (1) a profile paragraph, CV lines from `founder-brief.md` and a table of gaps with how to offset each; (2) 5 target projects and 6 offices or programmes, with public contact routes; (3) a calendar from 24 Nov 2026 to 31 Mar 2027; (4) the EXIST hotline question in German, with an English translation; (5) a 5-line pitch. I re-checked the dates and routes on 19 Nov (about 20 pages opened). Nobody was contacted.
- **What I found (new since C20):** (1) The **TUM Healthcare Happy Hour on 12 Jan 2027 (18:00) is free but already full**. The Luma page shows "Event Full" and an active waitlist [B]. (2) UnternehmerTUM holds a **free online info session on 24 Nov 2026**. The current Future Entrepreneur batch runs 31 Aug–9 Dec 2026, and the next application phase "starts in December" [B]. (3) Target 2, SYNTRA (AI-designed RNA transporters, Helmholtz Munich), now has a sourced spin-off plan. It was published in Nature on 2 Sep 2026, and the team "plans to transfer the technology into a spin-off company" [B]. It holds a federal GO-Bio next grant of **€3,054,897** running 1 Nov 2025–31 Oct 2028 [A]. (4) LMU's incubator accepts only teams with an LMU member, but its **Demo Day on 3 Feb 2027 is public** [B]. (5) **The part-time question probably has a "no" answer.** German law adds up working hours across employers and caps them at 8 hours per working day on average (§§ 2–3 ArbZG [A]). A 40-hour job plus a half-time post is about 60 hours a week; the cap is 48 (*my math*; whether this applies with an employer in Portugal is [UNVERIFIED]). The EXIST FAQ allows founding the company during the grant, but only with a side-job agreement or reduced hours [A]. (6) Still no open business seat on a Munich health project. Helmholtz Enterprise winners from the 13 Nov jury are not yet published, and no ki-alz or RadioGene company was found.
- **What it means:** the realistic plan is unpaid help with an application until February 2027, then a paid full-time start on 1 Sep 2027. The cheapest early contacts are the transfer offices (TUM Venture Lab Healthcare, LMU Spin-off Service, Helmholtz Munich, BioM for m4), not the scientists. m4 stage II (22 Feb 2027) and the 28 Feb kill line are the real deadlines.
- **Decisions for the CEO:** none new; you chose this route on 19 Nov. The time-critical actions are listed under Open questions.
- **Not done:** no outward action. The Future Entrepreneur opening date and the Happy Hour venue are not published.
- **Tasks:** C24 done. Added **C26** (critic, fact-check of the entry pack), because you will use it for outward steps. Next researcher task: C25 (trial-summary brief).
### 2026-11-19 — Fact-check: both desk runs, direction 2 (spin-out co-founder) and direction 1 (trial summaries) (critic, FACT-CHECK, tasks C22 and C21)
- **Done:** checked `research/direction2-spinout-cofounder.md` (33 of 33 sources opened) and `research/direction1-trial-summaries.md` (25 of 25 sources, plus a full re-count of the EU trial register: 12,873 trials, all 4,194 ended trials read one by one). Verdicts: **both pass (minor fixes)**. No invented data, quotes or contacts. No fix task (none critical).
- **What holds (direction 2, the recommended option in C23):** the dates are right. A spin-out grant application handed in by 31 Mar 2027 goes to a jury in June and can start on 1 Sep 2027; every funded team must include a business person; about 87 % of funded projects found a company; the university pays the team (a typical research post pays about €4,760–5,110 a month gross). The Helmholtz and Bavarian (m4) programme dates and the amounts of the five example projects are as stated.
- **What was wrong (direction 2), none of it changes the decision:** (1) The file says TUM's job board could not be searched. The board's own page links a backup list; I searched its 40 newest ads (October 2026) and found **no** business co-founder seat either, so the finding "no visible open seat in Munich" holds. (2) For the Helmholtz programme, the business lead must be in place at the review after month 7 (about Aug–Sep 2027 for a Feb 2027 start), a little earlier than the file's "about Oct 2027". (3) The salary assumes the usual research-staff pay grade (E13); the grant handbook says the grade must be justified by prior work or qualification, so the CEO's grade is not certain. (4) One example project (SYNTRA) is not shown to plan a spin-off on the page that was opened.
- **What holds (direction 1):** my re-count matches the file exactly for trials ending per year (1,826 in 2025; 609 with German sites) and for translations (75 % of German multi-country trials post a German lay summary). German universities do report on time (18 of 22).
- **What was wrong (direction 1):** (1) The number of overdue trials comes out somewhat **lower** in my re-count (Germany 80 instead of 85 trials with no summary at all; EU 291 instead of 331). That makes the "rescue overdue reports" market even smaller, so the researcher's "no brief as framed" verdict stands. (2) One US price is mislabelled: Emory's $5,400 is a registration fee only; updates and results reporting cost extra. It was not used in the price maths.
- **Does it change a decision?** No. C23 options and the researcher's recommendation (a) rest on facts that hold. One point for the CEO: if you choose (a), the Helmholtz route needs you named by about Aug–Sep 2027, and the 28 Feb 2027 kill line in the file stays the earliest real deadline.
- **Not done:** no red team of either file (business judgement); C17 red-team half still open. The federal funding catalogue count (136 grant entries) could not be reproduced because the exact query is not recorded; it is not used for any conclusion.
- **Tasks:** C21 and C22 marked done. Tasks added: none.
### 2026-11-18 — C19: desk run on trial-results and lay-summary documents (researcher)
- **Done:** `research/direction1-trial-summaries.md`. Own count of the official EU trial register (all 12,873 public trials, 4,194 ended), prices, competitors, translations, access routes. Not done: no per-trial price from any EU vendor exists publicly (10+ searches, 0 tenders); the package price is built from effort × hourly rate.
- **What I found:**
  - **Late reports are common but the unpaid backlog is small.** Of 1,621 EU trials past their deadline, 51.5 % reported on time, 27.3 % late, 21.2 % not at all (own count from the official register [A]; matches a 2026 study [B]). For trials with German sites only **85** have no report today; Portugal **12**. Most belong to big pharma groups (42 in Germany) or foreign biotechs, some of which have shut down. **German universities and university hospitals report well** (82 % and 75 % on time; only 4 trials missing).
  - **Every trial still needs these documents:** about **1,800 EU trials ended in 2025, ~600 with German sites** (own count [A]). Germany can fine a late report up to **€25,000** (drug law § 97 AMG [A]).
  - **Price (indirect):** one lay summary takes 35–105 hours (industry/patient-group report [B]); at the €82.2 freelance median (EMWA [B]) that is **€2,900–8,600**. US universities charge **$1,000–2,500** per study for results posting (UCLA) and **$5,400** for registration plus upkeep (Emory) [B]. A full package (summary + lay summary + ~4 translations) works out at roughly **€5–12k per trial** (*my math*).
  - **Sponsors pay for translations:** 75 % of German multi-country trials post a German lay summary, although the law does not require it (own count [A]). That work goes to CROs and language companies.
  - **Competition:** CROs (Quanticate, Certara), a Frankfurt writing firm bought by Indegene in 2024 to add AI, and AI start-ups with $12–36m funding (Peer AI, Weave Bio) [B].
- **What it means:** the "rescue overdue reports" idea fails: too few overdue trials, and the late ones are big pharma (with their own teams) or failing biotechs. What remains is a crowded service for ~700 trials a year from ~480 smaller companies, most of them one-trial buyers outside Germany. Three salaries need **60 packages a year** at €6,000, €1m needs **167** (8.5–24 % of that group, *my math*), with no medical writer on the team.
- **Options (CEO pick after C20, no task yet):** (a) brief direction 1 anyway, narrowed to "AI lay summary + translation pack sold through CROs"; (b) park direction 1 and wait for the direction 2 desk run (C20, next researcher run), then pick; (c) drop direction 1. **Recommendation: (b)**, because the desk test removed the main reason to prefer direction 1 (a large, legally forced, underserved gap), and C20 costs one more free run. If C20 also fails, (a) is the fallback.
- **Access without contacts (no outreach made):** the register itself names every sponsor with reports due; EMWA (medical writers; Spring 2027 conference in Amsterdam, date snippet-only); DIA Europe, Basel, 16–18 Mar 2027; PtCRIN (Portuguese academic trial network); BioM events in Munich.
- **Tasks added:** C21 (critic fact-check of the C19 file).

### 2026-11-18 — Fact-check re-check: new-directions scan after the C18 fixes (critic, FACT-CHECK, task C17)
- **File checked:** `research/new-directions.md` (the only research file changed since its last check). Review: `research/reviews/2026-11-18-new-directions-C18.md`. **Verdict: pass, with caveats. Nothing is made up.** All 8 new or changed sources opened and read in full; every new quote is word for word in its source; the two tender counts (125 and 36 award notices) reproduce exactly.
- **What holds (plain words):** all five errors from this morning's check are fixed. The key new fact is correct: the EU's official lay-summary guidance says the law asks for **one** plain-language summary per trial; translating it into each trial country's language is **recommended, not required**. The same guidance says most research funders do not budget for these summaries. The grant approval figure (634 of 2,280 applications, 27.8 %) and the TUM figure (115 start-ups by researchers, students and alumni) are quoted correctly.
- **Caveats (no new task, this was the one fix round):**
  1. "About one in four" EXIST applications approved is a **pessimistic** reading: the 27.8 % counts short pre-2023 outlines as applications, which lowers the rate. Today's odds for a full application may be better; the report gives no 2025-only rate.
  2. An older 2017 EU recommendation worded the translation rule more strongly ("is expected"), so some sponsors may treat translation as expected in practice. Whether they pay for it is still untested.
  3. Task C16 was written before these fixes and does not mention the 27.8 % or "translations recommended, not required"; both are in the C18 log entry below.
- **Does it change a decision?** No. C16 options and the recommendation (c) are unaffected by the fact-check. Two things to weigh: idea 1's multilingual edge depends on sponsors choosing to translate; the grant odds are roughly one in four or somewhat better.
- **Tasks added:** none. C17 stays open for the red-team half.

### 2026-11-18 — C18: fact-check fixes to the new-directions scan (researcher)
- **Done:** all 5 critical and all minor fixes from `research/reviews/2026-11-18-new-directions.md` applied to `research/new-directions.md` (the one fix round, rule 14). Not done: nothing left in C18. Next: **C16 (CEO)**; C17 red-team half (critic).
- **Most important new fact (official EU guidance [A]):** the EU lay-summary guidance says "the EU CTR does not request translations". The law requires **one** lay summary per trial. Translating it into each trial country's language (matching the patient consent form) is only **recommended** ([Good Lay Summary Practice, EudraLex Vol. 10, 2021](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf)). The same guidance warns that "most funding bodies do not foresee budget allocation" for lay summaries.
- **What it means:** direction 1 (trial-results documents) still rests on a legal duty, but the **language edge (DE/PT/EN) is weaker**: it only pays where sponsors follow the recommendation. **Academic sponsors** have the duty but often **no budget**, so small biotechs are the likelier payers. The Lisbon team (direction **3**, numbering fixed) is now only a *possible* delivery model.
- **Other corrections:** EXIST-Forschungstransfer approves **634 of 2,280** applications so far (**27.8 %**, official [A]); the invalid "fewer than 55 projects" sum is deleted. TUM's 115 start-ups (2025) are by researchers, students and alumni, mostly not spin-outs (TUM release [B]). Peer AI quote replaced (customers: "top 20 pharmaceutical firms and emerging biotechs" [B]). Occupational-health tender counts re-run and the query recorded (125 / 36 award notices [A]). With its bonus, the Lisbon job ad pays ~97 % of the German minimum wage, not 79 %. AbD counts corrected to 2 running / 2 started / 10 stopped.
- **Effect on C16:** the options and the recommendation (c) stay the same. Two cautions for the CEO: the multilingual edge in direction 1 is unproven, and the spin-out grant succeeds about one time in four.
- **Tasks added:** none.

### 2026-11-18 — Fact-check: new-directions scan (critic, FACT-CHECK, task C17 first half)
- **File checked:** `research/new-directions.md` (the only research file changed since its last check). Review: `research/reviews/2026-11-18-new-directions.md`. **Verdict: needs work (minor). Nothing is made up.** 27 of 29 links read in full; 2 sites blocked or down (GTAI, Pharmazeutische Zeitung).
- **What holds (plain words):** the EU law behind idea 1 is real and quoted correctly: every sponsor of a drug trial must upload a results summary and a summary for lay readers after the trial ends, and the authorities are tightening checks. The study saying only about half of trials reported on time matches its source (a study not yet peer-reviewed, as the file says). The EXIST grant rules for spin-outs (up to 4 paid people for 18 months, one seat for a business person) and the 2025 grant figures are correct. The wage, price and market numbers for the other 8 directions check out. All the sums are right.
- **What was wrong:**
  1. The recommendation says "keep **direction 4** as the delivery model", but the Lisbon team is **direction 3** in the table; direction 4 is drug-safety services. Only a label, but it sits in the sentence you act on.
  2. The language edge for idea 1 (German, English, Portuguese) assumes lay summaries must be translated into each country's language. The file itself marks that rule as unchecked, yet builds the recommendation on it.
  3. "TUM spun out 115 start-ups" links to a page that says 103 (for 2024). The 115 is real but counts mostly student and alumni start-ups, not research spin-outs.
  4. A quoted phrase about Peer AI ("plain language summaries") is not in the article cited.
  5. A sum about the EXIST grant is invalid, and the same report shows that only about **1 in 4 applications (27.8 %)** gets funded. That matters if the plan is to have the grant pay your salary.
- **Does it change a decision?** Not the choice between options (a) to (e) in C16. Two points to keep in mind when you decide: the language edge for idea 1 is not proven yet, and the spin-out grant is won by about one application in four.
- **Tasks added:** C18 (researcher): apply these fixes to `research/new-directions.md` (first and only fix round, rule 14). C17 stays open for the red-team half.
- **Not done:** red-team half of C17 (separate run).

### 2026-11-15 — Red team: GLP-1 companion brief after the C14 fixes (critic, RED TEAM)
- **Done:** second red team of `ventures/glp1-companion/brief.md`: only the C14 changes, and whether the first review's six objections were answered. Review: `research/reviews/2026-11-15-redteam-glp1-companion-brief-C14.md`. **Verdict: the brief passes as a decision document (it recommends drop and says why); the idea still fails as a venture; the optional pre-order test needs work.**
- **What was answered:** one price everywhere, no-moat and marketing gap stated, wider lawyer question, score caveat, waitlist test withdrawn. Four of six objections fully answered, two partly.
- **Top issues (caveats, rule 14, no new tasks):**
  1. **The test is closed by the brief's own rule.** It may run only if no competitor offers leavers a path at ≤ €15 a month; Weight Watchers does (€11.25). The brief calls this "met in the loose reading" instead of "met".
  2. **The test would not measure what a customer costs to win.** Its only concrete channel is a sponsored post in a 1,200-member forum: a negotiated price and a friendly audience, not an ad price that repeats or transfers to other themes.
  3. **A pass creates an obligation:** a 12-week programme with a nutrition professional nobody has named yet, or refunds. This should be a precondition.
  4. The brief still reads the Danish exercise trial in its favour (flagged by the fact-check); the consumer scan still ranks the GLP-1 row 4th at 37 points (for the C10 red team).
- **Does it change a decision?** No. It strengthens (d) drop. No `ceo` task added (C12 exists).
- **Not done:** no sources opened (reasoning review only).
- **Tasks added:** none. **Next critic work:** C10 red-team half (FUTRUE benchmark and consumer-health scan), including the GLP-1 re-score.

### 2026-11-15 — Fact-check: GLP-1 companion brief after the C14 fixes (critic, FACT-CHECK, run 14)
- **Done:** re-checked `ventures/glp1-companion/brief.md` after the researcher's fix round (C14). I opened all 16 new or changed sources, re-ran the App Store counts and re-did all the maths. Review: `research/reviews/2026-11-15-glp1-companion-brief-C14.md`. **Verdict: pass with caveats.**
- **What holds:** all 12 issues from the first check are fixed. The brief now uses one price everywhere (€129 for a 12-week programme, bought once), and every number built on it re-computes exactly: ~7,750 new customers a year for €1m revenue, at most €50–59 to win each customer, and a test pass mark of ≥10 paid pre-orders for €300 of ads. The new facts are right as cited: regain of 0.4 kg a month after stopping (BMJ 2026), the lower-dose trial (−16.6 % vs −9.9 % on placebo), Juniper UK patients staying 183 days with cost as the top reason to stop, and the formoline pharmacy product that already targets people who stop the drug.
- **What was wrong (top 3, all minor for the decision):**
  1. **The best evidence for the product is weaker than the brief says.** The brief cites a Danish trial: people who exercised *while on* the drug regained 6.0 kg less after stopping. In the trial, the 6.0 kg is for people who exercised *instead of* taking the drug. People who exercised *and* took the drug regained 2.5 kg less, which could be chance (not statistically significant). They did weigh 5.1 kg less a year later than people who took only the drug. The C14 log entry above repeats the 6.0 kg.
  2. **The Munich hospital programme (ZEPmedi-doc) is not an exit programme.** It treats patients with the drug; some of them later stopped without regaining much. The brief calls it a programme that "phases the drug out".
  3. Small wording leftovers: section 7 still says Gerresheimer "offers white-label" software (it is still developing it); "one-person project" for nachderspritze.de is a guess without a tag.
- **Does it change a decision?** No. Point 1 makes the case for the programme weaker, so it supports the researcher's recommendation to drop the idea (C12 option d). If you choose the pre-order test (option b) anyway, its numbers are now consistent and can be approved as written, after the lawyer hour.
- **Not done:** sources unchanged since this morning's check were not re-opened. Meta's ad-rules page could only be read through a summary tool (curl HTTP 400), so its wording is not checked word for word.
- **Tasks added:** none. C14 was this brief's one fix round (rule 14), so the remaining points are caveats in the review. Next critic work: C10 red-team half (FUTRUE benchmark and consumer-health scan).

### 2026-11-15 — C14 fixes to the GLP-1 companion brief (researcher)
- **Done:** applied all fact-check fixes (items 1–12) and red-team fixes (1–6) to `ventures/glp1-companion/brief.md`, plus the red team's desk test T1 (do incumbents serve people who stop the drug?). 15 new sources opened 2026-11-15.
- **What I found (new):**
  - No drug platform has a programme for people who stop (GoLighter, Voy checked; Juniper DE site blocked) [B]. But Weight Watchers is open to anyone at €11.25/month and in the US tells leavers that members who stayed "continued to see results" [B]; a pharmacy brand (formoline) already advertises "Gewicht halten nach der Abnehmspritze" with a free app, ~€30–60/month [B]; a Munich hospital phases patients off the drug (ZEPmedi-doc) [B]; the GLP-1 forum has free articles on stopping [C]; nachderspritze.de describes the same programme, still a waitlist [B].
  - Staying on a lower dose is a real alternative to stopping: tirzepatide 5 mg kept −16.6 % body weight vs −9.9 % on placebo (Lancet 2026 trial [A]). Regain after stopping is ~0.4 kg a month (BMJ 2026 meta-analysis [A]). Exercise *during* treatment cut regain after stopping by 6.0 kg (Danish trial [A]); no trial tests a programme started at the time of stopping.
  - UK self-payers at Juniper stayed 183 days on average; cost was the top reason to stop (38.7 %) (company-reported study [B]).
- **What it means:** with one consistent price (€129 for a 12-week programme, bought once), €1m revenue needs ~7,750 new customers a year (7.8 % of all 2024 self-payers, every year), and each may cost only €50–59 to win (my math from filings [A]). Germany-only market: €12.9m a year if every self-payer bought once. No moat; the decisive missing skill is paid acquisition, not product.
- **Recommendation changed:** from (b) "€300 waitlist test" to **(d) drop**. The waitlist test was flawed: without drug names the ads reach all dieters, and e-mails are not payments. If the CEO still wants a consumer-cost data point, the brief now has a redesigned **paid pre-order test** (one theme, €129 with full refund, €300 ads; pass ≥10 paid, kill <6), which needs a seller set-up and a lawyer hour first.
- **Not done:** formal re-score of the GLP-1 row (critic's math: 31/55, out of the top 5); GoLighter terms on WW access after the last order (page loads by script); Juniper DE and ZAVA pages (403).
- **Next:** CEO decides C12. Critic: C10 red-team half. Researcher: A17 after 1 Dec 2026.
- **Open questions:** none new; all outward actions (lawyer hour, pre-order set-up, ads) wait for C12.

### 2026-11-15 — Red team: GLP-1 companion brief (critic, RED TEAM, task C13 second half)
- **Done:** attacked the reasoning of `ventures/glp1-companion/brief.md` (facts taken from the fact-check). Review: `research/reviews/2026-11-15-redteam-glp1-companion-brief.md`. **Verdict: brief needs work; as a venture, fail.** First red team of this brief.
- **Top issues:**
  1. **The test does not test the idea (fatal for option b).** Ads may not name the drug, so they cannot find people who stop it; a pass would show general diet interest. Theme B ("low appetite") is about people still on the drug, the wedge the brief already rejected. A waitlist e-mail is not a payment.
  2. **Revenue per customer is overstated.** The product is 12 weeks; the maths assumes 6 months of payment. On 12 weeks each customer brings €83–129 and may cost at most ~€32–59 to win (*my math*); the waitlist would have to convert 13–21 %, not the assumed 10 %.
  3. **No moat, wrong skill.** nachderspritze.de already describes the same programme; GoLighter could keep its free Weight Watchers access on for people who stop at almost no cost. What decides success is paid-ads skill in a restricted health category, which neither the CEO nor any named person has.
  4. **Regulation read too narrowly.** The brief checks drug-ad rules and dosing features only; a programme sold purely to people leaving an obesity drug, promising to keep weight off, may itself fall under health-ad law or count as a medical device. The lawyer question should be wider.
  5. **Score was for another product.** 37/55 scored the "during treatment" companion. With today's evidence (free bundles, unproven benefit, weaker fit) it would be ~31/55, below every other top-5 theme (*my math*).
- **Pre-mortem kill criteria (dated):** any one incumbent offers people who stop a free or ≤€15/month path (check now, desk); fewer than 6 paid pre-orders for €300; fewer than 30 % of finishers buy a second period; no compliant ad wording per the lawyer; by 31 Mar 2027 no named nutrition co-founder and no named performance marketer.
- **Cheapest tests:** T1 desk check of incumbents' offers to leavers (free, now); T2 re-score the row; T3 redesigned paid pre-order test (€300, outward); T4 one conversation with a drug platform's product lead (outward).
- **Not done:** no sources opened (reasoning only). No tasks added: C14 is this brief's one fix round and already takes these fixes (rule 14); the recommendation change goes to the CEO via Open questions (C12 is already an open CEO task).

### 2026-11-15 — Fact-check: GLP-1 companion brief (critic, FACT-CHECK, task C13 first half)
- **Done:** checked every source in `ventures/glp1-companion/brief.md`. I opened 55 of the 56 links; the EU software guidance (MDCG) was offline. I also re-ran the App Store counts and re-did the section 5 maths. Review: `research/reviews/2026-11-15-glp1-companion-brief.md`. **Verdict: needs work (minor).**
- **What holds:** every number the bottom line rests on matches its source, and no quote is invented. That covers ~100,000 self-payers at end-2024 (IQVIA), €130 to just under €500 a month for the drug, fewer than 10 % still on the drug after a year where patients pay themselves, lean mass about a quarter to a third of the weight lost (the same as dieting), GoLighter's free Weight Watchers programme since 1 Sep 2026, and Wellster's audited 2024 revenue of €9.94m with a €3.12m loss. Hims & Hers' marketing share (39 % in 2025, 46 % in 2024) re-computes from the SEC data. The App Store counts reproduce.
- **What was wrong (top 3):**
  1. **The test page would show a higher price than the maths uses.** The brief computes revenue at €30 a month, but the landing page shows €129 per 12 weeks, which is about €47 a month. The pass mark, and with it what "acquisition cost is affordable" means, depends on which price is real.
  2. **The pass mark does not fit the budget split.** Each of the two ad themes gets €150, but the pass rule asks for 40 sign-ups "for €300". As derived, it should be 20 sign-ups per €150 theme.
  3. **The cohort kill line is too loose.** The pass mark assumes 1 in 10 sign-ups later pays, but the brief only stops if fewer than 1 in 20 pay. Between those two rates, each customer would cost €75–150 to win, above the €70–83 the brief allows.
  - Minor: one YouGov date is wrong (Jan, not Nov 2026); one quote is reworded; the $1.15bn Juniper deal value is not in its source; there is a free forum with content for people who stop the drug, which the brief does not list as an alternative.
- **Does it change a decision?** Not the direction: the facts still support the researcher's view that acquisition cost is the open question and a small test should come before Stage D (C12). But if you pick option (b), do not approve the test numbers as written; wait for fix task C14 (one price, a per-theme pass mark, a kill line that matches the €70–83 allowance).
- **Not done:** red-team half of C13 (pre-mortem, kill criteria), separate run. MDCG guidance not re-read (HTTP 503).
- **Tasks added:** C14 (researcher): apply these fixes plus the coming red-team fixes to the brief (the one fix round, rule 14).

### 2026-11-14 — Fact-check: FUTRUE benchmark, consumer-health scan, parked-ideas screen (critic)
- **Done:** checked the sources behind the three new research files (C10 fact-check half; C6 output). Reviews: `research/reviews/2026-11-14-futrue-consumer-scan.md`, `research/reviews/2026-11-14-parked-ideas-screen.md`.
- **Verdicts:** all three **pass, minor fixes**. No invented data, no forum post used to size a market, and every filed figure matches its source. That covers PharmaSGP's 44 % marketing share, Hims & Hers' 46 %, Natsana's €19m loss, the TED awards to Tiplu and fonio's price and customer numbers. The scoring and customer-count arithmetic re-computes exactly.
- **What was wrong (none changes a decision):**
  1. Consumer scan: the scan says no € figure per category exists, but a source it already cites gives NielsenIQ 2024 figures: stomach and digestion products €419m, weight-loss products €204m in Germany. Under the file's own scoring rules no rank moves.
  2. Consumer scan: IBS's top spend score rests on a Forbes *estimate* of Kijimea's maker's total revenue (all products, all countries), not German IBS revenue. Scored more cautiously, IBS drops from 38 to 36. The top 5 stays the same five ideas.
  3. Smaller points: one menopause startup (Femna) is named without a source; "pelvic trainers add little" comes from a review of resistance devices, not app trainers; the phone-assistant price range starts at €9, not €69 (this supports the file's "price collapse" point).
- **What it means for C9:** the facts behind the consumer-health top 5 hold. The open questions are judgment questions (does admitting "weak" spend evidence favour unproven ideas; are the tests decisive). Those go to the red-team half of C10, which is still open.
- **Not done:** C10 red team (separate run). § 393 SGB V and § 5 NemV could not be re-opened (government site down); the pelvina article now blocks automated access. Neither is contradicted.
- Tasks added: none (no critical issue). C10 stays open with a note.
### 2026-11-14 — C8 run 2: consumer-health scan scored, top 5, CEO task (researcher)
- Done: `research/consumer-health-scan.md` complete; `research/futrue-benchmark.md` grants row updated. C8 closed. Default applied (you did not answer): homeopathy excluded, "evidence base" scored.
- **What I found (numbers, source type):**
  - The model works at scale but buying customers is expensive: marketing was 44 % of revenue at PharmaSGP and 46 % at Hims & Hers (stock-exchange filings [A]). A young German supplement group (Natsana, founded 2020) reached €87m revenue with a €19m loss before Bayer bought it (trade press [B]). Period-underwear brand Snuggs (founded 2019) made €20m with a profit before interest, tax and depreciation (press [B]).
  - 11 of 21 needs ranked (10 excluded: drug or device routes too costly, no proven spend, homeopathy, services, or traps). Top 5 of 55 points: **IBS 38, menopause 38, female bladder leaks 38, GLP-1 self-payer companion 37, fertility 36.** Ranks 1–4 are a tie.
  - Where consumers clearly pay (IBS, fertility, sleep), one brand owns the shelf (Kijimea with a clinical trial; Femibion 60 % share in 2016 [B]). Where the shelf is open, spend is shown only indirectly: 57.6 % of women with strong hot flushes buy OTC products (study [A]); incontinence care is "on the way to a pure self-pay market" (urologist, Apotheken Umschau [B]); GLP-1 self-payers pay up to €490 a month for the drug, but no figure shows what they spend on companion products [B].
  - Rules: a supplement needs only a notification, but may not claim to treat a disease (Verbraucherzentrale on EU law [B]). Grants fit poorly; only a digital part could qualify.
  - €10k pays for one product test, not a launch: a 2,000-unit minimum batch plus a small ad budget (my estimate, unit price not published).
- **What it means:** the open themes are **midlife women (menopause + bladder leaks, one brand family)** and **GLP-1 self-payers** (best fit with your AI/automation skills). The question that decides all of them is how much it costs to win a paying, returning customer. Desk research cannot answer that; a small ad test can.
- Not done: no customer-acquisition cost per category, no contract-maker price, Reddit and Amazon not reachable (3 UK forum threads used instead, [C]).
- Tasks added: **C9 (CEO)**, C10 (critic: fact-check + red team of the two C8 files).
- **Decision for you (C9):** (a) desk tests first, then a ~€300-per-theme ad test that you approve before it goes live; (b) a venture brief on the midlife-women brand now; (c) a brief on the GLP-1 companion now; (d) back to the B2B options (C7). **Recommendation: (a)**, because ranks 1–4 are too close to pick from desk scores and only a real test measures acquisition cost. If you want no outward action yet, (b).

### 2026-11-14 — C8 run 1: FUTRUE benchmark + consumer-health scan started (researcher)
- Done: `research/futrue-benchmark.md` (part 1, complete). Started `research/consumer-health-scan.md` (parts 2–3, partial).
- **What FUTRUE is:** a founder-owned holding (Gräfelfing, 2008) of ~20 companies, not a studio for outside founders. Founders: a physician with a Harvard MBA who sat on Novartis Germany's executive board, and a lawyer ex-BCG (CVs in stock-exchange filings [A]).
- **How it makes money (PharmaSGP IPO prospectus [A], 2019):** revenue €62.6m, marketing €27.8m (44 %), profit before interest and tax €22.4m (36 %), 30 staff. All production by contract makers; sold only in pharmacies; customers pay themselves; products that do not break even in 3–6 months are dropped. 2024: €118.8m revenue (filing [A]). Forbes estimates the Kijimea company at ~$100m revenue [B].
- **How it started (trade press [B], 2015–18):** first product Kijimea (2009) flopped; the restart came through a deal where a TV group took a share of sales instead of cash for ad time. Two brands were sold in 2014–15.
- **What it means for you:** the model is proven at large scale, which none of the B2B ideas showed. The copyable part with €10k: pick a common self-treated complaint, use the cheapest legal product class (food supplement: notification only, § 5 NemV [A]), contract maker from 2,000 units [B], sell online first, kill fast. Not copyable: their starting position, the multi-million ad budgets, and two of their routes (gut devices now need a notified body under MDR; the pain brands are homeopathic remedies).
- **First scan signals (not ranked yet):** menopause (9m women aged 40–55 [B]; 57.6 % of women with strong hot flushes buy OTC products [A]); GLP-1 self-payers (~100,000 in DE end-2024, €276–490 a month [B]); tinnitus (9.8 % bothersome [A]); female incontinence (48 % in one German survey [A, 2017]). Trap: the €42 care-supplies box (fraud warnings, 2024 rules [B]).
- Not done: rows marked "not checked" in the scan, CAC and margins, contract-maker prices, grants, scoring, top 5. Amazon pages are bot-blocked (not bypassed); EUR-Lex returned empty pages (Rule 21 quoted from a trade-association paper).
- Tasks: none added. C8 notes updated; C8 stays open (run 2 finishes parts 2–3 and adds the CEO task).
- Next: researcher C8 run 2. Critic: fact-check of the two new files.
- Open question for the CEO: see "Open questions" (product types).

### 2026-11-14 — C6 parked-ideas screen (researcher)
- Done: `research/parked-ideas-screen.md`. It puts L07, L13, L03, L29 and L06 through the test that stopped L01: who signs, a sourced price, customers needed for three salaries (€180,000 a year, my assumption) and for €1m ARR, and cash to month 24.
- **Result in one line: no parked idea is a venture case today. Only L07 passes the arithmetic, and it fails on access.**

| Idea | Customers for 3 salaries / €1m ARR (my math on sourced prices) | Main blocker (source type) | Verdict |
|---|---|---|---|
| L07 MD-audit defence for hospitals | **3–5 / 17–25** hospitals at €40,000–60,600 (DKI survey [B]; UK Frankfurt award [A]) | Tiplu won every public AI-coding award 2025–26 (LMU, Würzburg €545,250, Lausitz); Lausitz required ≥€1m turnover in the field (EU tenders [A]); Tiplu now part of LOGEX; calliora (Munich, $6m) [B]. Needs a medical-controlling co-founder | Cheap test first |
| L13 AI phone for practices | 75–152 / **419–842** practices at €99–199 a month (price lists [B]) | IONOS €99 flat rate; fonio >7,000 customers, €14.6m seed; CGM and Doctolib bundle it [B] | Skill test only |
| L03 § 45 carer course for Kassen | 4 / 20 Kassen at the €50,000 cap; no price shown | All carer courses ≈€14.6m a year nationally (one Kasse's statutory statistic [A], my scaling); free courses already exist [B] | Drop |
| L29 AI post-market surveillance | No price found | Flinn "200+" customers [B]; the EU proposal would halve PSUR frequency [B] | Drop |
| L06 LLM discharge letters | No price found | One tender, still no award after 15 months [A]; Microsoft Dragon Copilot drafts letters in Germany since Oct 2025 [B] | Drop |

- What it means: cash to month 24 for three people is ~€360,000, and the money in sight is ≤€166,000 (€10,000 own, EXIST best case €120,000, Start?Zuschuss! €36,000). L07 is the only idea where three contracts close that gap. Whether the CEO can reach a co-founder for it is the open question.
- New cross-cutting fact: cloud processing of health data by providers, Kassen and their processors needs a C5 attestation (§ 393 SGB V [A]).
- Not done: count of independent (non-chain) private hospitals (needs a Destatis match); hospital sales-cycle length; C5 audit cost; no sourced price for L03, L06 or L29.
- Task added: **C7 (CEO)**. Options:
  - (a) L07 cheap tests first: you name a medical controller or coder you could reach (10 min), plus one desk run on a small-private-hospital, service-first wedge;
  - (b) back to the long list with this screen;
  - (c) L13 as a skill project;
  - (d) an L07 brief now.

  **Recommendation: (a), and (b) if no co-founder candidate.**
- Next: critic fact-check of `research/parked-ideas-screen.md`; CEO C7.

### 2026-11-14 — CEO decision: park L01 and prevention clinics; C6 added (worker session)
- CEO in chat: "For now let's park both of these ideas and continue the research." Also: one daily brief, more detailed, instead of per-run summaries.
- Done: C3 and C5 closed with notes. C6 added (researcher): screen L07, L06, L03, L13, L29 with the test that stopped L01. Decision record and routine-prompt changes are in a separate PR left open for the CEO.
- Not done / open: PNOG desk run after 11 Dec 2026 (not decided); access check (which buyer roles the CEO could call).
- Next: researcher C6; then a CEO decision on which idea, if any, gets the next brief.

### 2026-11-13 — Critic red team, second pass: L01 venture brief after C4 (critic, RED TEAM)
- Mode: RED TEAM. File: `ventures/eldercare-navigator/brief.md` as revised in C4. Review: `research/reviews/2026-11-13-redteam-eldercare-navigator-brief-C4.md`. No new sources opened; calculations marked as the critic's own.
- Verdict: **pass (caveats)** for the brief as a decision document; wedge (ii) still **fails as a venture case**. F1–F3 and F5–F7 of the first red team are answered; F4 (founder, co-founder incentive, timing) only partly.
- Top caveats (rule 14: no tasks):
  - "K-a: Met" is absence of evidence on a judgment threshold (EUR 15,000 follows from an unfounded 60 customers), and the Eldercare24 list price has no paying customer behind it. Incumbent prices (K-b) are still unchecked.
  - Stronger reason, from the brief's own SWR row: the three lots together are about EUR 36 per employee per year, the eldercare lot EUR 4–6 (critic's math). Employers pay for the bundle; eldercare is about 17 % of it. The bundle is heycare's and pme's ground.
  - "Best case pays three modest salaries" holds only at month 24. With a linear ramp the low case leaves a gap of about EUR 252,000 over two years against EUR 10,000 own money and one grant of max EUR 36,000.
  - K-d (the vote) is redundant: it cannot reopen L01 either way. K-g's usage half is close to a coin flip at about 4 expected cases; K-f needs the co-founder, the legal opinion and most of the budget before it can run.
  - Option (c) points to L07 / L11, which have not had the test that stopped L01; the shortlist and task C5 still show L01 at 64–66.
- Not done: no source re-opened (red team); no incumbent price check; no screen of the parked ideas (proposed to the CEO, not started).
- Tasks added: none. Open question added for the CEO (above). `tasks.json` unchanged.
- Next: CEO C3 and C5.

### 2026-11-13 — Critic fact-check run 12: prevention-clinic idea check, L01 brief after C4 (critic, FACT-CHECK)
- Mode: FACT-CHECK. Files new or changed since their last fact-check: `research/idea-prevention-clinics.md` (researcher C2) and `ventures/eldercare-navigator/brief.md` (C4; merged to `main` while this run was under way, so it was checked too).
- Reviews:
  - `research/reviews/2026-11-13-idea-prevention-clinics.md`: **pass (minor fixes)**. 50 of 50 listed URLs opened, plus 3 TED notices.
  - `research/reviews/2026-11-13-eldercare-navigator-brief-C4.md`: **pass (caveats)**. 11 URLs and 5 TED notices, i.e. every source behind a changed line.
- Re-run counts, all match: Aware app (60 ratings; 21 reviews: 11 five-star, 7 one-star), wellabe (41 ratings), Hacker News (53 comments, 10 top-level), TED 594202-2026 / 370897-2026 / 664823-2026 and the five notices re-used in C4, score arithmetic (50 / 52 / 54, R4 49), all new arithmetic in the brief.
- What holds: idea check: YEARS prices, Neko 2025 accounts, Aware insolvency and €100,000 sale, Art. 18 HKaG, Aeon in Munich, Neko Germany 2027, Cochrane and Eur Radiol figures, tax rule, Präventionsbericht amounts. Brief: all 9 fact-check fixes applied correctly; new PNOG quotes (§ 7a functions and dates, § 7a Abs. 2, delegation to third parties) are verbatim. No fabrication in either file.
- Top issues (all minor; no verdict, recommendation or CEO option changes):
  1. Idea check: stale sources not flagged. The TUM Manager-Check brochure is from 2017 and the AXA wellabe flyer from 2021, both used in the present tense for employer spend. Also, IKK classic's €604,750 is a framework value with no purchase obligation, not money spent. K1 for the employer wedge still passes on the two 2026 TED notices.
  2. Idea check: Finding 3 ("cannot own the clinic") is firmer than the file's own gap list (§ 30 GewO `[UNVERIFIED]`; MVZ via a hospital). Correct reading: a company cannot run a practice directly; the other routes are out of reach at €10k or unverified. Two snippet-only prices (AYUN, Function Health) lack the `[UNVERIFIED]` tag.
  3. Brief: heycare's homepage names eight customers (three with the EAP tag), not three (one); and "a bill with a €7.6bn financing gap" misreads the source (€7.6bn is the expected 2027 deficit; the bill leaves at least €1.35bn open).
- Tasks: none added (no critical issue; the brief has had its fix round, rule 14). A8 notes updated. Nothing else in `tasks.json` changed.
- Not done: no red team of the idea check (not a stage deliverable); unchanged sources of the brief were not re-opened.
- Next: CEO C3 and C5.
- Open questions: one consistency note on C3 + C5 added above.

### 2026-11-13 — C4 Fixes to the L01 venture brief (researcher)
- Done: all 9 fact-check issues and all 7 red-team edits applied to `ventures/eldercare-navigator/brief.md`. Every changed figure was re-opened at its source (TED API, PNOG cabinet draft, Bertelsmann, iwd, heise, heycare.com, nui.care). No new searches (task: edits only).
- Main changes:
  - SWR headcount from the notice itself (ca. 3,500 permanent staff + ca. 1,800 freelancers): €4–6 per employee per year; per-head TAM cross-check €103m–154m. One buyer's estimate, no award.
  - New customer-count table: three salaries need 31–76 customers (salary levels are assumptions); €1m ARR needs 167–279. K1 not shown, K2 unproven for this wedge.
  - One usage estimate everywhere (0.4 cases per 100 staff in 6 months); pilot is paid; kill criteria K-a to K-h are dated and measurable. K-a is met today.
  - €760m stated as the Kassen's delivery budget, not a market. Wellthy labelled non-comparable. Section 2 now reads the evidence as weak willingness to pay.
- Differences from the reviews (for the CEO):
  - The red team says the best case "does not pay the three people". At €60,000 employer cost each it does, just (€180,000 of €359,000); the low case does not. The verdict "not a venture case" stands either way.
  - K-g uses 2 cases in total (half the expected ~4) instead of the critic's 0.5 per 100, which sits above the brief's own estimate.
  - Nui's news item on the KI-Pflegegradassistent is dated 12/11/2026 on nui.care (the review says 02/11/2026).
  - New from the PNOG draft: § 7a Abs. 2 asks Kassen to give digital information before a care need is established (no date), which touches the "weeks before the first care grade" the brief called untouched.
- Not done: no survivorship search (failed eldercare startups), no check of incumbents' small-firm prices (K-b). Both are caveats per rule 14, listed in the brief's Gaps.
- Tasks: C4 done. No tasks added. C3 text not changed (CEO task).
- Next: CEO C3 and C5. Researcher: nothing unblocked until A17 (2026-12-01).

### 2026-11-13 — Critic red team: L01 venture brief (critic, RED TEAM)
- Mode: RED TEAM. File: `ventures/eldercare-navigator/brief.md`. Review: `research/reviews/2026-11-13-redteam-eldercare-navigator-brief.md`. No new sources opened (reasoning only).
- Verdict: brief **needs work**; wedge (ii), employer-paid eldercare alone, **fails as a venture case**.
- Top issues:
  - F1: the brief's own evidence says weak willingness to pay, not an open market (offer rate 14.0 % → 15.7 % in 11 years; Eldercare24 at €299 without a customer; heycare entered with a bundle and €4m). "No paying-customer proof" is fair and understated.
  - F2: best case 60 customers = €359,000 ARR for a three-person team; €1m ARR needs 167–279 customers; per-head pricing gives no lever. HR conversations cannot repair this.
  - F3: pilot and kill rows contradict the brief's usage estimate (0.4 cases per 100 staff in 6 months vs conversion at ≥3 % of staff and kill at <1 per 100).
  - F4: nothing uses the founder's AI edge; the product is a care adviser the company cannot pay; funding path is one €36,000 grant.
  - F5/F6: PNOG over-weighted as a new market (€760m is a delivery budget; buyer is the Kasse cluster already rated closed), under-weighted as a sales objection in 2027–28.
  - F7: not re-scored; under `research/scoring.md` wedge (ii) reads K1 not shown, K2 unproven.
- Pre-mortem (5 reasons) and rewritten kill criteria K-a to K-h are in the review.
- Tasks: critic C2 marked done. No new task (rule 14): the 7 red-team edits were added as notes to C4. Nothing else in `tasks.json` changed.
- Not done: no desk re-check of incumbent small-firm prices or of failed eldercare startups (listed as cheapest tests / caveats).
- Next: researcher C4; CEO C3 and C5.
- Open questions: see "CEO (C3), from the red team" above.

### 2026-11-13 — C2 Idea check: prevention clinics (researcher)
- Done: `research/idea-prevention-clinics.md` (operators and prices, payers, regulation, capital, Munich, score, cheapest tests). Verdict: **drop the clinic; no deep dive**.
- Key findings:
  - Demand is real (YEARS €1,990–16,900; Neko revenue SEK 157m in 2025), but benefit for healthy adults is not shown (Cochrane; whole-body MRI meta-analysis 2026).
  - Clinics burn capital: Neko net loss SEK 677m in 2025; Aware Health insolvent in May 2026 and sold to Aeon for €100,000.
  - Art. 18 HKaG: no company may run a medical practice in Bavaria.
  - Munich: Aeon sells via a partner practice; Neko plans Germany for 2027; Diagnostik München, TUM Manager-Check, wellabe/Mavie.
  - Employers buy prevention (TED: WBM check-ups 2026; IKK classic €604,750), but tenders need references, and extended check-ups are taxable wage.
  - Scores: clinic 50, consumer platform 52, employer programme 54/49 "unproven"; L01 66/62.
- Not done: YEARS and wellabe accounts; Aeon German prices; legal opinion on the broker model; Neko $700m round only as snippet.
- Tasks added: C5 (CEO decision; renumbered from C4 at merge because the critic added a C4 in parallel). Note: `tasks.json` holds two tasks with id C2 (researcher, critic); not renumbered.
- Blocked hosts: nekohealth.com (429), radiologybusiness.com, fiercehealthcare.com, sifted.eu, ziprecruiter.de, jobs-radar.com, emarketer.com (403), affarsvarlden.se (login redirect), beyond-imaging.de (empty page). Reddit search: 0 reddit.com hits.
- Next: critic C2 (L01 brief); CEO C3 and C5.

### 2026-11-13 — Critic fact-check run 11: L01 venture brief, shortlist B4 (critic, FACT-CHECK)
- Mode: FACT-CHECK. Files new or changed since their last fact-check: `ventures/eldercare-navigator/brief.md` (C1) and `research/shortlist.md` (B4 edits). Checks were run on 2026-11-12; the run was interrupted and finished on 2026-11-13 (no change on `main` in between).
- Reviews: `research/reviews/2026-11-12-eldercare-navigator-brief.md` (**needs work, minor**; 37 of 37 URLs, 16 of 16 TED notices) and `research/reviews/2026-11-12-shortlist-B4.md` (**pass**).
- Re-run counts: TED 7 queries (19 / 4 / 4 / 23 / 2 / 8 / 9) and App Store (Nui 185, heycare 31, DAK 8, mitpflegeleben 15; 24 reviews) all match.
- What holds: TED values and lot titles, PNOG quotes for §§ 7a / 7c / 7d (cabinet draft), IW table A-3, Destatis size classes, Eldercare24 prices, all section 5 arithmetic. No fabrication.
- Top issues:
  1. SWR headcount is `[UNVERIFIED]` (snippets) but feeds the "€6 per employee" price, the €154m cross-check and the section 7 price hypothesis. The cited TED notice itself gives ca. 3,500 staff + ca. 1,800 freelancers, so €4–6 per head; it is one buyer's estimate with no award.
  2. Three statements say more than the source: Nui Pflege-Kompass "already analyses" (heise: "is intended to"); TenneT "€1.1m" (winning tender €880,000); Charité "own procedure" (only value and a full-text match are retrievable). Firm examples of eldercare as its own lot are two, both inside family-service procedures.
  3. Stale items not flagged (iwd = 2022 data; Nui price complaints from 2020/2021), and heycare's homepage shows named customers that the brief cites only "according to the company".
- None of this changes the brief's recommendation (revise); the corrections make the price evidence slightly weaker.
- Tasks added: C4 (researcher: apply the fact-check fixes; the one fix round for the brief, rule 14). C2 (critic) stays open with notes: the red-team half (pre-mortem, kill criteria) is not done.
- Note: `tasks.json` holds two tasks with id "C2" (researcher idea check, critic review). Not renumbered.
- Not done: red team of the brief; Charité notice text (TED XML/PDF returned HTTP 202).
- Next: critic red team of the brief (C2), researcher C4 and C2 (idea check), then CEO C3.

### 2026-11-11 — C1 Venture brief: eldercare navigator as an employee benefit (researcher)
- Done: `ventures/eldercare-navigator/brief.md`, all 13 template sections, wedge (ii) mid-size employers without a family-service contract.
- Key findings:
  - No sourced example of a company ≤3 years old paid by a named employer for eldercare alone.
  - Eldercare is tendered on its own in 3 of 7 TED procedures (SWR lot 3: est. €84,034 / 48 months; Straßen.NRW lot 2; Charité 2022), but references are required. Family-service tenders draw 1–2 bids.
  - Price points are low: Eldercare24 list price €299–499 per company per month. SOM estimate €108,000–359,000 ARR at 30–60 customers (inference).
  - Only 15.7 % of firms offer care-placement help, while 79.5 % call support for caring staff important (IW 2026).
  - Munich is occupied: famPlus, pme, heycare (employers), Nui Care (insurers; AOK Bayern, DAK, Allianz PKV).
  - PNOG bill: free Pflege-Cockpit (1 Jul 2028) and Pflegebegleitung (1 Jan 2029, €146 per home-care recipient a year) = substitute and possible new buyer.
- Not done: interviews (by design); re-scoring; ≥10-investor list (Stage D); first-sale dates of heycare/famPlus (not found); SWR award and headcount.
- Tasks added: C2 (critic: fact-check and pre-mortem of the brief), C3 (CEO: go / revise / drop; recommendation: revise).
- Blocked hosts this run: wds.care (proxy 502), amiravita.de and work-life-management.de (HTTP 403), startbase.de (403), evergabe.nrw documents (404 after deadline). Reddit search: 0 reddit.com hits.
- Next: C2, then C3.

### 2026-11-08 — B2 Red team of shortlist.md (critic, RED TEAM)
- Mode: RED TEAM. File: `research/shortlist.md` (as corrected by B4). Review: `research/reviews/2026-11-08-redteam-shortlist.md`. Verdict: **needs work (as caveats; rule 14, no new tasks)**.
- Per idea:
  - L01: deep-dive, re-wedged.
  - L07: deep-dive only if a co-founder candidate is named.
  - L03: footnote in L01, not a co-payer.
  - L06, L13, L29: no brief.
- Top issues:
  - (R1) NEW: TED awards show employers pay for eldercare counselling only inside family-service/EAP frameworks (EUR 0.4–1.4m), won by pme (4x) and awo lifebalance. famPlus (Munich) sells the L01 product and is missing from the shortlist. The B4 strict-K1 fallback therefore does not remove L01, but the sketched wedge ("depth vs pme") attacks the wrong layer.
  - (R2) No top-5 idea uses anything specific to this founder. The founder works in Lisbon until Sep 2027, which weakens in-person sales.
  - (R3) § 393 SGB V C5 attestation applies to L03/L06/L07/L13 vendors; § 87 BetrVG works-council review for L01.
  - (R4) Bundling L03 into L01 doubles sales and creates a free substitute.
- B3 view: option (a) modified (L01 re-wedged + L07 conditional). The strict fallback L07 + L13 is not recommended.
- Tasks added: none (rule 14). B2 marked done.
- Next: CEO B3.

<!-- Newest first. Format:
### 2026-11-07 — A7 Long list of 20–30 problems (researcher)
- Done: `research/longlist.md`: 30 problems (L01–L30) merged from P1–P11, S1–S10, I1–I10 and cancer A–E; each with one-line statement, who has it, who pays (proven / budget / plausible / unclear), evidence count and grades, links. Excluded/merged: S6, S9, I10, cancer D; cancer A/B replaced by German data (L17); P7+S8 → L08; I6 split into L22 (hospital-audit work, MD-IT) and L23 (care assessments).
  - New sourced items: colorectal screening participation 7.75 % vs EU minimum 45 %, documented follow-up after positive stool test 12.9 % (G-BA report, Mar 2026) [A]; lung LDCT screening GKV benefit since Apr 2026 [A]; § 115f (hybrid DRG) deleted, short-stay flat rates from 2028 (BT-Drs. 21/8629) [A] → new row L10; pharmacies 20.1 h/week on shortages (ABDA) [B]; live-in care 100k–210k carers/day (BMG report 2024) [A]; ~4m rare-disease patients (BMG 2026) [A]; BARMER runs cancer navigators in-house [B].
  - All rows have ≥2 evidence items with ≥1 [A]/[B]; proven spend in 15 rows, but direct startup access is rare (A14 tender check).
- Not done: scoring fields (signer, budget line, wedge, first-sale route, buyer count) = A18. L10 has no purchase or [C] evidence yet; [C] layer thin overall (Reddit blocked).
- Next: researcher A18; critic A8 review of `research/longlist.md`.
- Tasks added: none.
- Open questions: none new (Reddit API key still open).

### YYYY-MM-DD — <task id> <task title>
- Done:
- Not done / blocked:
- Next:
- Open questions:
-->

### 2026-11-08 — B4 Restate L01 K1/K2 labels and top-5 sensitivity (researcher)
- Done: edits to `research/shortlist.md` only; no new searching. L01 K1 is now **"weak / eldercare spend not isolated"**. pme's 1,400 firms are EAP customers. heycare's named employers come from the vendor and buy a bundled EAP. Aon is an offering page with no buyer. AOK PLUS is a free Thüringen project. Strict fallback: L01 out → top 5 = L07, L06, L03, L13, L29, and the recommendation falls back to L07 (+ L13 test). 18,632 are legal units, so the L01 ceiling is an upper bound. Optional fixes: L26 K1 is stale (2021/2022) and would be "not shown" (rank 8, no top-5 effect). L07 rebased to private hospitals: 729 × €20–40k = €14.6–29.2m. The DKI €40k is acquisition plus running cost. With market 3→2, L07 = 61/56 and swaps with L06; the top 5 is unchanged.
- Not done: fact-check issues 4–12 stay as caveats (rule 14).
- Next: critic B2 red team; CEO B3.
- Tasks added: none.
- Open questions: **CEO (B3): accept L01 K1 as "weak" (bundled-EAP purchase), or read it strictly as "not shown"?** Weak → recommendation (a) stands. Strict → deep-dive L07 (+ L13 test; L06 optional). Note: the B3 task text still shows recommendation (a) without this condition.

### 2026-11-08 — Fact-check of shortlist.md (B1) (critic, run 10)
- Mode: FACT-CHECK. File: `research/shortlist.md`. Review: `research/reviews/2026-11-08-shortlist.md`. Verdict: **needs work (minor)**; 24 of 41 sources opened.
- Reproduces: all 10 base totals, 10 R4 totals, R2 caps, tiers, C1/C2/C6 variants and ceilings. The top 5 (L01, L07, L06, L03, L13) is the correct base-total order; no mechanical change. No fabrication; quotes verbatim.
- Top issues: (1) L01 K1 passes on pme's EAP count and heycare's vendor-claimed bundled-EAP customers, a weaker standard than the one that knocks out L12/L20; if K1 fails L01 drops out and L29 enters (task B4, the one fix round). (2) L26 K1 evidence (Clariness) is dated 2021/2022, against the file's own "2024+" reading (no top-5 effect). (3) L07 market/ceiling uses all 1,807 hospitals though the wedge is private hospitals <300 beds (729 private); the DKI EUR 40k median is acquisition plus running cost, not annual. Also: L06 pain tag H has a counter-source; L06 K1 treated differently from L08 (KHZG money); the L23 evidence procedure was cancelled.
- Tasks added: B4 (researcher, before B2). A8 and B2 notes updated; B2 (red team) still open.
- Next: researcher B4; critic B2 red team after B4. B3 (CEO) is not blocked, but the recommendation "deep-dive L01" depends on B4's outcome.
- Open questions for the CEO: none new.

### 2026-11-08 — B1 Score long list, pick top 5 (researcher)
- Done: `research/shortlist.md`. `scoring.md` applied as written; the open CEO questions (vendor age, S1–S4, Sep 2027 clock, K1 'in force by then') are listed as caveats C1–C7, each with its rank effect.
  - 17 of 27 wedges fail K1 (evidence must name the wedge's signer and job); none fails K2 outright. 10 survivors, **all "unproven"** (criterion 5 L everywhere), so no tier A.
  - Top 5 by base total: **L01 66, L07 63, L06 62, L03 59, L13 59**; runner-up L29 57. Slots 1–3 are robust. S1, S4, re-scoring L03's pain or a strict L06 K1 each swap one slot for L29.
  - New sources: § 106b SGB XI TI-Pauschale [A] (L05 K1); employer eldercare incumbents pme (>1,400 firms), Aon, AOK Pflegelotsen [B] (L01); practices paying for AI phone assistants, Ärzteblatt 7/2024 [B] (L13 K1); Clariness × Boehringer Ingelheim and Servier DE [B] (L26 K1); DORA covers insurers [A] (L24); Harzklinikum LLM tender has no award notice (TED).
- Not done: A24/A26 desk tests (deferred by CEO; listed as open checks per idea).
- Next: critic B2; CEO B3.
- Tasks added: B3 (ceo, stage gate).
- Open questions: B3 (above). Optional: the open scoring questions only move slots 4–5.

### 2026-11-08 — A8 Critic fact-check run 9: A18 scoring fields, A23 long list, A25 scoring.md (critic, FACT-CHECK)
- Done: `research/reviews/2026-11-08-longlist-scoring-fields-A23-A25.md`. Verdict: pass with minor fixes (caveats only; the long list and scoring.md already had their fix round, rule 14, so no fix tasks). Opened ~49 sources (all A18 vendor and statistics URLs, all A25 and A23 URLs) and re-ran 4 TED queries: 53 MD notices since 1 Jan 2026 and 9 MD "KI" notices since 2025 match; MD Niedersachsen 383478-2026 (4 x EUR 500k, 3 Jul 2026) matches; long-list counts (27 rows, 13 clusters, 8/4/3/12 spend status) and scoring.md arithmetic (L21 64/59, L03 59/52) reproduce. All 8 earlier scoring.md issues closed. No fabrication.
- Top caveats: (1) "Seven wedges with a young vendor with a named customer" is really five (CrewLinQ and calliora name no customer; only heycare and Flinn pass the age test today). (2) L23 uses the MD Nordrhein tender (TED 762721-2026), which is malpractice review ("Behandlungsfehler"), not care assessment; TED 343840-2025 is MD Rheinland-Pfalz, not Nordrhein as `pain-industry.md` says. (3) "Category leader" for Recare/Flinn and "$20m Series A" for Flinn are not in the cited sources; L01 "proven" rests on a vendor claim ("laut Unternehmen"). Also: TED has a result notice for MD RLP (483916-2025) without a winner, so "no award notice" should read "no winner".
- Not done: snippet-only items stay unverified (labelled in the files); WIdO PDF and the EU central-government threshold (EUR 140,000) not re-confirmed. WebFetch could not resolve most hosts; curl was used.
- Next: B1 (researcher). B1 should read the A18 table, not its headline count, and list the caveats above as open checks. Critic: B2 after the shortlist.
- Tasks added: none (rule 14). Open questions: none new.

### 2026-11-08 — A25 Apply fact-check fixes to scoring.md v3 (researcher)
- Done: all 8 issues from `research/reviews/2026-11-07-scoring-v3-and-A22.md` fixed in `research/scoring.md`.
  - L03 pain cell filled (4 M, WIdO 2026 [B]); 59/52 now reproduce.
  - L03 K1 passes on the § 45 budget line only; vendor payment is not sourced.
  - L21 K2 relabelled "unproven": the Telekom TechBoost release names no insurer or sale; 2 more searches found none. L21 v3 drops 70/68 → 64/59.
  - UKL-GPT is no longer a discharge-letter signal. The €15,000 rule is limited to federal-level bodies. L06 reads "possible, rules unverified".
  - voize sourced: founded 2020 [B]; Caritas Stuttgart Jan 2022 [B]. The unsourced "BruderhausDiakonie" was removed.
  - EU threshold €216,000 cited to Delegated Reg. (EU) 2025/2152 [A] + IHK Hannover [B].
- Not done: none.
- Next: researcher B1.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A23 Apply red-team fixes to research/longlist.md (researcher)
- Done: `research/longlist.md`:
  - Who-pays split into "spend on this job" vs "adjacent spend" for all rows. **Proven job spend: 8 rows** (L01, L05, L07, L08, L09, L21, L22, L29), not 15.
  - Added 13 signer clusters (C1–C13).
  - Merged L10 → L07 (KVs give practices free groupers [B]) and L30 → L26.
  - Excluded L19; S6 stays excluded. The ePA must be gematik-approved and gematik sets the ident rules with the BSI (§§ 342, 325, 291 Abs. 8 SGB V [A]).
  - L25 kept but flagged "budget ended": the last ÖGD tranche of €750m is paid in 2026 "abschließend" (BT-Drs. 21/8237 [A]); the 2027 federal draft has €0 for the ÖGD [B].
  - L22 noted as the opposite side of L07. New L02/L08 incumbent: Verbund Pflegehilfe [B]. 27 rows remain.
- Not done: no new per-row purchase searches (A24/A26 cover the open tests).
- Next: researcher A24, A25, A26, then B1.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A8 Critic red team: A18 long-list scoring fields (critic, RED TEAM)
- Done: `research/reviews/2026-11-07-redteam-longlist-fields.md` — verdict **needs work before B1**. Reviewed `research/longlist-scoring-fields.md` with `research/longlist.md` under `scoring.md` v3.
- Top issues: (G1) K1/K2 evidence often belongs to another product than the wedge (L05 TI onboarding backed by voize; L08 by Recare; L21 BPO wedge backed by Kasse spend; L06 labelled "adjacent" but calibration says K1 pass); (G2) "Job: opex, no observed purchase" fails K1 (L12, L20, L24); (G3) accessible rows are too small to fund, only L01 has a €100m+ ceiling; (G4) in-force triggers precede the founder's Sep 2027 start, later triggers are bills; (G5) DORA makes L24 near-closed. Missing incumbents: pme Familienservice (L01), ePA eML (L08), Insiders Technologies (L21/L24).
- B1 will wrongly pass K1: L06, L12, L20, L21, L24; wrongly pass K2: L05, L08; may wrongly fail: L11. Tier-B candidates with one desk test each: L01, L20, L03, L11, L07 (reserve L23).
- Not done: no sources opened as pages (search summaries only, used as pointers); no fact-check of A18.
- Tasks added: A26 (researcher, before B1).
- Open questions: K1 "in force" vs Sep 2027 clock (added above).

### 2026-11-07 — A8 Critic fact-check run 8: scoring.md v3 and A22 changes (critic, FACT-CHECK)
- Done: `research/reviews/2026-11-07-scoring-v3-and-A22.md` — verdict **pass with minor fixes**, no critical issues. All 19 scoring.md sources opened; legal thresholds (Art. 20 BayWiVG EUR 100k, § 22 Abs. 2 SVHV EUR 50k, § 280 Abs. 3 SGB V, Art. 5 BayUniKlinG, § 45 SGB XI) and BAS circular quotes reproduce; calibration arithmetic reproduces. A22 TED deadlines (7 notices) match; DTVP links 404 as stated.
- Top issues: (1) L03 calibration row has no pain score in the table though the total uses 4; (2) L21 "channel" (Telekom TechBoost) and L03 K1 rest on programme/press text that names no sale or fee, so they overstate fix-1 evidence; (3) UKL-GPT does not mention discharge letters; also the EUR 15k "before" rule covers federal-level bodies only, voize facts cite "A18 notes" with no URL.
- Not done: A18 output (`research/longlist-scoring-fields.md`) was merged to main after this check began and is unchecked; full read of pain-patients.md / pain-professionals.md still pending.
- Next: researcher A25 (fixes), then critic fact-check of A18 output.
- Tasks added: A25 (researcher, before B1).
- Open questions: none new.

### 2026-11-07 — A18 Long-list scoring fields (researcher)
- Done: `research/longlist-scoring-fields.md` (linked from `longlist.md`): per row user, signer, budget line (job vs adjacent), wedge + price/ACV guess, status quo, trigger, first-sale route, young-vendor K2 example, DE buyer count.
  - K2 examples with a named customer: voize (Caritas Stuttgart, Jan 2022), heycare (Daimler Truck etc., Mar 2026), PflegeBetreuer (Mobil Krankenkasse, ZF BKK, 2026), Flinn (Paul Hartmann, 2026), Recare (Uniklinik Köln 2023). voize, Flinn and Recare lead their categories (S2).
  - None found for L06, L07, L12, L13, L17, L20, L21, L23, L24, L26, L27, L28.
  - New [A]: MD Niedersachsen bought ~20,000 DRG audits from external review firms (€2m, TED 383478-2026). TechBoost needs completed B2B customer projects (S3: not a first-sale channel). RLP § 19a credits voice documentation as 0.5 FTE since 1 Oct 2026 [B].
  - Buyer counts: 1,807 hospitals (729 private), 16,505 care homes, 15,549 home-care services, 92 Kassen, 18,632 firms ≥250 staff [A]; ~98,000 practices, 39 PKV, 1,480 medtech firms [B].
- Not done: AT/CH counts; founding years of Recare, Gesundheit von Morgen, CrewLinQ; prices mostly inference.
- Next: researcher A23 and A24 (remaining A24 tests: AMNOG count, care-suite AI, recognitions by country); then B1.
- Tasks added: none.
- Open questions: CEO decision on how "≤5 years" is measured is still open (decides voize/L05).

### 2026-11-07 — A22 Apply fact-check fixes from the A21 re-check (researcher)
- Done: all 5 issues of `research/reviews/2026-11-07-A21-longlist-payer-pain-industry-recheck.md`, plus low-priority issue 6.
  - Buyer count 33 → 32. Unread thresholds = 7 notices / 7 buyers (gkv informatik counted; it is "No" on its 3-reference requirement alone).
  - DAK 396194-2026 and gkv informatik 481787-2026 closed (14 Jul / 10 Aug 2026, TED); DTVP document links return HTTP 404, so not read.
  - UK Saarland 508395-2025 and MD Bayern 63363-2025 also closed (TED). No checked notice is open to a newcomer alone.
  - MD Nordrhein (re-downloaded aumass package): R6 needs one reference with ≥€500k net own development work. Added to `longlist.md`, `pain-industry.md`, `payer-processing.md`. Subcontractor route labelled inference: it counts only via Eignungsleihe (§ 47 VgV).
  - Stale MD RLP present tense fixed (`pain-industry.md`, `payer-processing.md` route table); Charité two notices noted in `pain-professionals.md`.
- Not done: nothing left in A22.
- Next: researcher A18, then A23/A24.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A8 Critic red team of longlist.md and scoring.md v3 (critic, RED TEAM)
- Done: `research/reviews/2026-11-07-redteam-longlist.md` (verdict: **needs work**) and `research/reviews/2026-11-07-redteam-scoring-v3.md` (verdict: **needs work**, small edits).
- Top issues, long list:
  - (F1) No row shows why *this* founder wins. €10k, part-time and no buyer network block ISO 27001 / § 80 SGB X-type prerequisites for institutional buyers.
  - (F2) "Proven" who-pays labels count care, labour, physician fees and grant pools as spend on a product job (L02, L04, L05, L06, L14, L26).
  - (F3) 30 rows ≈ 10 signer clusters. Merge L10→L07 and L30→L26; exclude L19 (S6 rule); L25 fails K1.
  - (F4) The 2027 triggers favour funded incumbents (Tiplu, calliora, voize). The founder starts in Sep 2027.
- Rows to watch:
  - Likely too high: L21 (borrowed caery channel), L06/L07 (base-total fallback), L13 (confidence-high commodity), L05 (voize = K2 evidence and leader), L22.
  - Likely under-researched: L20 pharmacies, L24 PKV, the employer wedge of L01/L03, lung screening in L17, L11 (only language edge).
- Top issues, scoring v3:
  - (S1) With no tier A, the top 5 is filled by base total, so the confidence rules do not affect the order. Fix: order tier B by R4 total.
  - (S2) K2 evidence selects crowded categories.
  - (S3) The channel clause accepts another firm's channel.
  - (S4) Wedge proliferation.
  - Also: €500k achievability anchor vs €10k own budget; 12-month clock start; JV/subsidiary loophole in "≤5 years".
- Not done: no source re-checks (red-team scope); A18 fields not yet available, so signers/wedges in the review are inference.
- Next: researcher A22, A18, then A23/A24; CEO decisions under Open questions before B1.
- Tasks added: A23 (researcher, long-list labels/clusters/merges), A24 (researcher, desk tests), both before A8.
- Open questions: S1–S4 approval, the 12-month clock, the founder-access check (see Open questions).

### 2026-11-07 — A8 Critic fact-check run 7 (critic, FACT-CHECK)
- Done: re-checked the A21 changes in `research/longlist.md`, `research/pain-industry.md`, `research/payer-processing.md` (review: `research/reviews/2026-11-07-A21-longlist-payer-pain-industry-recheck.md`). Verdict: pass with minor fixes. MD Nordrhein terms (EUR 600k average in-field turnover, 4.0 FTE, 2 productive AI references, consortia) reproduce from the downloaded aumass tender package; MD RLP re-tender deadline 5 Sep 2025 and MD Nordrhein 3 Dec 2026 confirmed via TED API; tender tables recount 36 notices (match) but 32 buyers (file says 33); the 15 zero-[C] rows match.
- Top issues: (1) buyer count 32 not 33, and gkv informatik also unread; (2) stale "MD RLP could apply / open" wording at `pain-industry.md` lines 39 and 224; (3) MD Nordrhein also requires one reference with >= EUR 500k net own development work (omitted), and the "subcontractor" route is inference.
- Not done: unchanged text not re-opened; A18 output does not exist yet; full read of `pain-patients.md` and `pain-professionals.md` after A14 still outstanding.
- Next: researcher A22 (small fixes, can combine with A18).
- Tasks added: A22 (researcher).
- Open questions: none.

### 2026-11-07 — A20 Apply CEO-approved scoring v2 fixes 1–6 (researcher)
- Done: `research/scoring.md` v3: fixes 1–6 applied (K2 evidence rule / 'K2 unproven'; buyer-specific direct-award table; wedge = unit of scoring; K1 'category' and 'in force'; R1 M vs L incl. unknown = 2 L; R4 order and tiers). Fixes 7–10 not applied (CEO).
  - Thresholds now sourced [A]: § 22 Abs. 2 SVHV €50k since 1 Jul 2026 (BAS circulars Jan + Jun 2026); applies to MDs via § 280 Abs. 3 SGB V + SVHV Eingangsformel; Bavarian university hospitals are outside BayHO purchasing rules (Art. 5 BayUniKlinG), so the €100k BayWiVG limit may not apply to them `[UNVERIFIED]`.
  - Calibration (L06, L07, L21, L03): v2 order L06 78 > L07 75 > L21 70 (L03 out); v3 L21 70 = L06 70 > L07 67 > L03 59 (L03 revived by a § 45 SGB XI wedge). **All four end 'unproven'**, so none can be tier A; B1 will likely fill the top 5 from tier B unless A18 finds named young-vendor customers.
- Not done: municipal hospital GmbH purchasing rules; caery and Gesundheit von Morgen founding years.
- Next: critic fact-check of `research/scoring.md`; researcher A18, then B1.
- Tasks added: none.
- Open questions: '≤5 years' measurement and unnamed-customer claims (see Open questions).

### 2026-11-07 — A21 Apply fact-check fixes to research/longlist.md (researcher)
- Done (all 5 issues in `research/reviews/2026-11-07-longlist.md`): MD RLP AI PoC restated as "accessible when tendered, closed 5 Sep 2025, no award in TED" (Findings, L23 row and details); tender count fixed to 36 notices from 33 buyers, 6 still unread (the review said 9 rows; my recount of the two tables gives 6 notices from 6 buyers after reading MD Nordrhein); L10 "~1m cases" = catalogue scope, WIdO counts added; BR-Drs. 620/26 added (Bundestag 15 Oct 2026, not yet law, Bundesrat 20 Nov); [C] gaps list corrected (15 rows without opened voices); L19 marked one [B] only; €15bn gap now points to `trends.md`.
  - **New:** MD Nordrhein 762721-2026 tender documents read (public download on aumass) [A]: average in-field turnover ≥€600k/yr, ≥4.0 FTE, 2 references for productive AI document software; consortia/subcontracting allowed → not accessible alone. Synced in `payer-processing.md` and the `pain-industry.md` tender table.
- Not done: nothing from the fix list.
- Note: I first started A18 from a stale local `main`; after fetching, A21 (added by the critic) came first under rule 7, so I switched. The A18 research done so far (direct-award limits incl. SVHV/MD and Bavarian university hospitals, buyer counts, 10+ young-vendor examples with named customers) is stored in the A18 task notes with URLs.
- Next: researcher A18; critic optional re-check of the A21 changes.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A8 Critic fact-check run 6 (critic, FACT-CHECK)
- Done: fact-checked `research/longlist.md` (A7) and the A17/A19 changes (hospital-billing-audits, payer-processing, trial-recruitment-de, pain-industry), plus spot checks of the A14 pain-patients/pain-professionals revision -> `research/reviews/2026-11-07-longlist.md`. Verdict: **needs work (minor)**, no critical issues, no fabrication. All 14 A7-opened sources and 8 carried-over ones re-downloaded; numbers match (G-BA colorectal 7.75 % / 12.9 %, ABDA 20.1 h, WIdO hybrid DRG, BMG live-in/rare disease, BARMER, BR-Drs. 620/26 with the 1 % tier, DKG EUR 145k, Clinerion deal pages). App Store ratings and Destatis 17.7m re-run: match.
- Top issues: (1) "only one tender open to a new company (MD RLP AI PoC)" is stale: TED 543912-2025 closed 5 Sep 2025; "34 notices" does not reproduce (tables hold 36; 9 rows have unread thresholds). (2) L10 "~1m hybrid-DRG cases in 2026" is the catalogue scope, not billed cases; the cited BT-Drs. 21/8629 is the committee report (passage shown by BR-Drs. 620/26). (3) [C] counts inconsistent between Gaps and table (L23, L26, L27); L19 has only one [B] item.
- Not done: full read of `pain-patients.md` and `pain-professionals.md` after A14 (spot checks only, no new errors); `scoring.md` not re-checked (red-team scope).
- Next: researcher A21 (fix list, before A18); critic re-check of longlist after A21.
- Tasks added: A21 (researcher, before A18).
- Open questions: none new.

### 2026-11-07 — A19 Apply fact-check fixes to A11/A12/A13 files and pain-industry.md (researcher)
- Done (all items in the four reviews):
  - `research/payer-processing.md`: MD-IT Lot 3 stays **€7m**, now citing change notice 773326-2026 (6 Nov 2026; cn 751925 said €5m). Re-downloaded the DTVP documents myself (01 Angebotsbedingungen V1.2, 04.1, Bieterinformation 1–2) [A]: €5m turnover (averaged since founding if <3 yrs), 25 staff, 2 references confirmed; **correction:** a finished pilot replaces *one of the two* references (not a 3rd); **new:** consortia and capacity borrowing (§ 47 VgV) are allowed, so "blocked as prime" → "blocked alone; possible as subcontractor or consortium member". SBK €2.19m marked as procedure estimate; DAK 427316-2025 marked `pin-only`; TK/QuantCo 3 bids re-confirmed.
  - `research/hospital-billing-audits.md`: "€1.6bn flows back" → "revenue at risk for hospitals"; MD capacity updated to 31 Dec 2025 (2,148.3 physician FTE); two audit counting bases explained (MD-handled vs GKV-SV reported); "plan to buy AI" → "plan to use"; DKI quartile contradiction noted; calliora "not independently verified" added; §6 AI-spend arithmetic marked "not a TAM line".
  - `research/trial-recruitment-de.md`: TriNetX–Clinerion is **now sourced, not removed**: Citeline/Norstella bought Clinerion (Feb 2023), then sold it to TriNetX (Apr 2023) per both deal counsels [B]. Netherlands (55) added; Munich "about 300"; 69.7 % = 46 of 66 RCTs with a budget; 8.5 % discount has no end date (only the exemption is 3 years).
  - `research/pain-industry.md`: "verified in A13" dropped; 33k → 24k participants sourced (vfa Oct 2025 deck p. 7, text-searchable as "33 Tsd."); 5.6m attributed to vdek; PKV "0,001 %" vs computed 0.0098 % noted; MD-IT access wording synced.
- Not done: nothing from the fix list. Pain-patients/pain-professionals A14 edits still await the critic's full check (A8).
- Next: researcher A7 (long list); A17 remainder after ~1 Dec 2026; A20 waits for the CEO. Critic: re-check of these four files is optional (no critical items).
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A17 Refresh hospital audit-quota data (researcher, partly done)
- Done (`research/hospital-billing-audits.md` §1–2, Findings, Gaps, Sources):
  - **1 % tier (≥90 % unobjected) is in the Bundestag-passed text** [A]: BT-Drs. 21/8629 Art. 1b no. 12 (four tiers 1/5/20/40 %, in force 1 Jan 2027, applies to Q1 2027 quotas from Q3 2026 data); BR-Drs. 620/26 contains it verbatim. Bundesrat: TOP 5 on 20 Nov 2026; no consent needed, mediation committee possible [B].
  - **8-quarter re-run (Q3 2024–Q2 2026) incl. the 1 % tier** [A data, my math]: 40 % tier stable at 1,098–1,139 hospital IKs; cap 3.9–4.1× today's (1.30–1.40m invoices/quarter). 1 % tier = 83–127 IKs, mostly tiny audit samples (Q2 2026: 86 of 102 had <20 audits), only 48 % stay next quarter, cap effect ~0.1 %. Q2 2026 reproduces A11 exactly.
  - **§ 17c Abs. 7 KHG joint report: not published**; deadline moved 30 Jun 2025 → 30 Jun 2026; BMG report to the Bundestag due 31 Dec 2026; contract value €145k net (DKG); the 2024 tender had award problems (GKV-SV letter).
- Not done: Q3 2026 statistics (not out; due end of Nov 2026) and the Bundesrat outcome (20 Nov). A17 left open with notes; do not restart before ~1 Dec 2026.
- Side finding for A19: TED change notice 773326-2026 (6 Nov 2026) sets MD-IT Lot 3 to €7m, so the critic's "€5m" fix is outdated (note added to A19).

### 2026-11-07 — A8 Critic fact-check run 5 (critic, FACT-CHECK)
- Done: fact-checked the A15 + A16 changes in `research/reimbursement-routes.md` and `research/munich-ecosystem.md` (plus the one-line sync in `research/trends.md`) → `research/reviews/2026-11-07-A15-A16-reimbursement-routes-munich-ecosystem.md`. Verdict: **pass with minor fixes**, no critical issues. All 27 sources carrying new claims re-downloaded; BAS payouts 2019–2024, DAK figures, § 113e text (cabinet draft), wages, FLÜGGE 2026/1 call, EY (−46 %), EIC dates, UnternehmerTUM "keine Unternehmensanteile" all match.
- Top minor issues: (1) SCE "not rolling" is overstated: the same page says "Dauerhaft für die SCE Incubation bewerben"; next-intake date is inference. (2) FINSOZ's 5.6 FTE is a refinanceable cap on extra posts, not the § 113e corridor; FINSOZ's own conservative case is 2.8 FTE, so the €16–19k per home / €128–151m national figures may be overstated (labelled inference). (3) Uptake math uses 32,054 facilities while DAK's "48 % = 17,500" implies ~36,500; the 37 % vs "knapp 40 %" match is partly coincidence. Also: Länder catch-up rule omitted.
- Not done: no other file is new since its fact-check (scoring, A11–A13 files, pain files unchanged); full A14 re-check of pain-patients/pain-professionals still open; vdek, KHZG, GKV-SV position paper (Aug 2026) not re-opened.
- Next: researcher may fold the five minor fixes into the next edit of these files (no separate task added; none is critical). Critic: A8 continues with A17/A18/A7 outputs when they exist.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A16 Apply fact-check fixes to reimbursement-routes.md and munich-ecosystem.md (researcher)
- Done (all 9 items; 4–5 were done in A15):
  - `research/reimbursement-routes.md`: GKV-SV PM regraded [B]; § 40a Abs. 1a quoted verbatim (excludes work organisation of *outpatient* services and apps "ausschließlich" for benefits advice; carer-relief apps explicitly included, so a hybrid carer-relief app is not excluded, inference); 1.9m = users of *any* insurer-funded prevention measure (vdek quote); KHZG €4.3bn synced from A10 (was `[UNVERIFIED]`).
  - `research/munich-ecosystem.md`: SCE Incubation is **not rolling**: two batches/yr (Mar–Jul, Sep–Jan), last deadline 2 Aug 2026, next (summer 2027) deadline not published. UnternehmerTUM Incubator "wir nehmen keine Unternehmensanteile" now sourced. **FLÜGGE call 2026/1** opened [A]: up to 4 projects (~€500k), sketches via a state Bavarian Hochschule by **18 Dec 2026**, panel 18 Mar 2027, start ~1 Jul 2027. EY: Bayern >€1.1bn = **−46 %** y/y; "B2B workflow AI" trend now labelled as a two-deal anecdote. EIC 2027 batching dates 20 Jan / 17 Mar / 1 Sep / 4 Nov re-checked on the EIC page.
- Not done: SCE summer-2027 deadline (not yet published); no Munich health deal count by segment (Crunchbase/Dealroom blocked).
- Next: A17. Critic: fact-check the A15 + A16 changes.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A15 § 113e Transformationsstellen and § 8 Abs. 8 uptake (researcher)
- Done: `research/reimbursement-routes.md` updated.
  - New §4b + table row for **§ 113e** (bill 21/8869, text identical to the cabinet draft): residential homes only, 2028–2032, ≤10 % of the staffing-corridor posts, valued at care minimum wage × 1,560 h, catalogue-gated (Kompetenzzentrum, from 30 Sep 2027). My estimate: ~€16–19k/yr per 100-resident home (FINSOZ example), ceiling ~€100k (DBfK). Nationally ~€43–151m/yr (inference). GKV-SV wants it replaced by a study until 2031 (only ~1/3 of homes have the needed staffing split); DBfK and ver.di want it struck; FINSOZ wants 50 %.
  - **§ 8 Abs. 8 uptake reframed with official data:** BAS national payouts €143.3m 2019–2024 [A] (€24–32m/yr since 2020, flat) ≈ 37 % of the €384.6m pool; ~65 % of DAK-processed facilities used it; vdek 20–30 % = full amount used. "Weak uptake" and the unsourced "IT capacity, not money" claim are removed.
  - New facts: the PNOG 1st reading happened on 5 Nov 2026 (bill went to the Health Committee); the old €12k grant drops "Entlastung der Pflegekräfte"/workflow items from 2027; the bill's general reasoning still says "ambulanten und teilstationären" for the €1.6bn fund (law text: "ambulanter und stationärer").
  - Also did A16 items 4 and 5 (same paragraphs). Synced the uptake gap line in `research/trends.md`.
- Not done: no AOK or GKV-SV count of facilities using the grant was found; BAS 2025 figure not found; GKV-SV § 113c Abs. 8 report (the "one third" figure) not opened.
- Next: A16 (remaining items 1–3, 6–9). Critic: fact-check the A15 changes in `research/reimbursement-routes.md`.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — Red team v2 of research/scoring.md (critic, RED TEAM)
- Done: reviewed the revised method (K1/K2 + R1–R4, CEO option (b)) → `research/reviews/2026-11-07-redteam-scoring-v2.md`. Verdict: **needs work** (rejected options not re-argued).
- Top issues: (1) K2 only fires if *no* direct-award, private-buyer or channel route exists. Such a route is almost always legally possible, and below-threshold and private purchases are invisible in TED. So K2 lets through S1/S3/S7/S8, where every checked tender is closed. (2) "Inference" is in both M and L, so WTP and achievability get tagged M and R2/R3 never fire. Worked example: an S1-type row scores 78/90 (76 after R4) and reaches the top 5. (3) Tiers A/B/C, the R4 order (−1 before or after the cap) and the score for unknowns are undefined. (4) K1 "category" and "budget line" are undefined (draft-law money, price lists). (5) Insurers' direct-award limit is § 22 Abs. 2 SVHV ≤€50k [A], not BayWiVG.
- Proposed: 10 one-line fixes (1–6 must-fix before B1), for CEO approval. `scoring.md` not edited.
- Tasks added: A20 (researcher, blocked on CEO approval), inserted before A18.
- Not done: no B1 scores computed; whether MDs fall under the SVHV and whether BayWiVG covers university/municipal GmbH hospitals is `[UNVERIFIED]`; BAS circular of 8 Jan 2026 not opened.
- Open questions: CEO approval of fixes 1–10 (see Open questions).

### 2026-11-07 — A8 Critic fact-check run 4 (critic, FACT-CHECK)
- Done: fact-checked `research/hospital-billing-audits.md` (A11), `research/payer-processing.md` (A12), `research/trial-recruitment-de.md` (A13): all **pass with minor fixes**. Also `research/scoring.md` K1/K2 revision (pass; two procurement thresholds supported by search results only) and a sample of the A14 revision of `research/pain-industry.md` (pass, not a full re-check). Reviews in `research/reviews/2026-11-07-*.md`. Re-run counts: CTIS (12,788 trials, 4,653 transitioned, every year/country figure) **match exactly**; ClinicalTrials.gov matches except Munich recruiting (307 in file, 314 today); GKV-SV 2023–2025 national audit statistics and the Q2 2026 per-hospital 2027 simulation (1,100/231/193 hospitals; 532 below 50 %) **match**; 28 TED notices, MD Bund report and DKI survey re-checked.
- Top issues: (1) MD-IT framework Lot 3 value is EUR 5m in TED, not EUR 7m, and the MD-IT eligibility rules rest on DTVP documents I could not re-read. (2) "TriNetX owns Clinerion" is stated as fact in A13 Findings and copied into `pain-industry.md` as "verified in A13", while A13's own Details call it snippet-level and the opened source says Citeline/Norstella bought Clinerion in 2023. (3) Smaller overstatements: Netherlands (55 single-country trials) left out of the "Germany has the most" list; 69.7 % budget overrun is of 66 RCTs, not 93; "most hospitals plan to buy AI" is "plan to use" in DKI; two incompatible MD audit counts and a stale 2023 MD capacity figure in A11.
- Not done: pain-patients.md and pain-professionals.md edits from A14 not read; vfa 2013 position PDF unreadable as text; Probando/Carelane/Ancora not opened (blocked, flagged in the files); DTVP tender documents not re-read; BayWiVG and federal EUR 50k thresholds only seen as search results.
- Next: researcher A19 (fix list, inserted before A7). Critic: remaining A8 items (A14 pain-patients/pain-professionals, A15, A16, A17, A18 outputs, A7 long list).
- Tasks added: A19 (researcher: apply fact-check fixes), inserted before A7. A8 left open (notes updated).
- Open questions: none new.

### 2026-11-07 — A14 Apply critic fixes to the three pain files (researcher)
- Done: `research/pain-industry.md`, `research/pain-professionals.md`, `research/pain-patients.md` revised.
  - Read the eligibility criteria (TED `selection-criterion-description-lot`) of 34 tender notices used as WTP evidence and added a "Tender access check" table to the industry and professionals files. Only one is open to a new company: the MD Rheinland-Pfalz AI PoC (one PoC reference, no turnover minimum). UK Saarland speech recognition has no turnover minimum but needs 2 live hospital references. All others need €250k–€10m turnover, university-hospital/GKV references, ISO 9001/27001 or a KHZG certificate [A].
  - WTP downgraded: I5 and S3 → "high buyer budget, low direct startup access"; S1, S7, S8 → "no direct access". I5 split into scan/intake BPO (5 buyers) vs billing check (3). DAK €890m reworded as claims volume checked.
  - Harzklinikum 492877-2025 re-labelled as clinical decision support; MDR caveat from MDR Annex VIII Rule 11 (EUR-Lex) and MDCG 2019-11 rev. 1 [A]: decision-support features → class IIa+.
  - Sourced or fixed: 92 insurers; 15 MDs (MD Bund report); 1.52m (2014) → 1,431,000 assessments in 2013 (MDS); 19m → 17.7m inpatients 2025 (Destatis); 1.8m nurses → 446,425 + 817,711 care-facility staff (2023); 150,000 → 191,875 contract practitioners.
  - [C] counts split into opened vs titles only (A3); leadership 9/9 → 8/9 (A4); ePA contrast added (main insurer apps 4.5–4.8 vs ePA apps 1.3–2.5); €469 marked as among users, self-estimate; voize study COI checked (first author employed by voize); 91 % AOK figure confirmed.
  - I1 updated from A13 (sponsor vs site view, CTIS share, vendors verified, CTMS line removed).
- Not done: thresholds that sit only in tender documents (DAK, gkv informatik, MD Nordrhein, 5 hospital tenders); I4 counter-source; below-threshold buys are invisible in TED.
- Next: A15. Critic: fact-check the three revised pain files.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A13 Clinical-trial recruitment in Germany (researcher)
- Done: `research/trial-recruitment-de.md`.
  - Own CTIS count of all 12,788 public trials [A]: Germany is in 668 of 1,356 (49.3 %) new commercial EU trials in 2025, second only to Spain. It also has the most single-country commercial trials. But its share of trial participants is ~2.9 % [B]. *Inference:* the gap is patients per site, not trial placement.
  - Sponsors cite "fehlende Patienten" for missed targets (72 % of university sites in oncology miss plan by ≥25 %). Sites themselves (N=169, Jan 2026) rate patient identification as a big hurdle in only 4–9 % of cases; staffing/funding is the big hurdle (50–74 %) [B].
  - EHR "patient-finder" systems at 6 MIRACUM university hospitals showed no significant enrolment effect (npj Digit Med 2026) [A].
  - 5 % rule [A]: the BStabG moved it from the G-BA assessment (deleted) to an exemption from the new 8.5 % discount (§ 130a Abs. 1c) for drugs launched from 2027. The BfArM portal is live. Uptake data: none.
  - The Kapazitätsinitiative 2030 is a lobby proposal (3 funding lines incl. recruitment capacity) with no budget or government commitment [B].
  - Sites are paid for patient identification under the 2025 joint costing recommendations, but euro amounts per patient are not public.
  - Vendors: Clariness (incl. Viomedo) merged with SubjectWell (Jan 2026); TriNetX owns Clinerion; Trialbee and Inato report 6,000+ sites each. **MPIRIQ (Munich, 2024)** already sells practice-based trial pre-screening at €99–329/month.
- Not done / blocked: per-patient site fees and sponsor recruitment budgets (not public; Stage D interviews); 5 % rule uptake; DGPharMed survey original; MPIRIQ funding (snippet only). Blocked: forschen-fuer-gesundheit.de, htgf.de, probando.de, ancora.ai, norstella.com, iduneo.com; the Bundesagentur job API returned no JSON.
- Next: A14 (should also update `pain-industry.md` I1 with this file: barometer published 28 Sep 2026; vendors now verified; the "CTMS 65 products" line is not recruitment competition). Critic: fact-check `research/trial-recruitment-de.md`.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A12 Insurer invoice processing and MD assessment automation (researcher)
- Done: `research/payer-processing.md`. Read the award notices for all payer/MD tenders in TED, plus the public tender documents of the new MD-IT AI framework.
  - § 302 outsourcing [A]: 13 awards, 2024–26. IQVIA Health System Services (formerly DAVASO) won 5; the others went to SPS, GFS, mediakom, AZ Emmendingen, GEOS and QuantCo. Where bids are reported, each tender drew only 1–3. Values: €5.5m–€34.3m per lot. One public-law route (§ 88 SGB X) bypasses tenders entirely. DAK €890m is the claims volume checked, not the contract value.
  - Shift from outsourcing to AI software [A]: DAK explored buying AI billing-check software to bring the work back in-house. TK bought DRG scoring software from QuantCo. BITMARCK builds AI "von Krankenkassen für Krankenkassen" [B].
  - Largest new budget [A]: MD-IT framework, 48 months, €88m max for AI case summaries in hospital billing audits. It is explicitly triggered by the statutory audit quotas; bids are due 2 Dec 2026. A startup cannot bid as prime contractor (needs €5m turnover, 25 staff, 2 references); subcontractors are allowed.
  - Most accessible entry [A]: small MD PoC tenders. MD RLP's GenAI care-assessment PoC drew 40 requests to participate and asks for only one PoC reference. The MDs have 2,148 physician FTE and produce only 3.7 % of opinions externally.
  - Admin cap [A]: § 4 Abs. 5 (from 2027) and Abs. 6 (2026: +8 % vs 2024). PNOG slightly reduces care-assessment volume. There are 92 insurers, not 93.
  - Inference: direct § 302 sales fail K2. Payer/MD audit AI has a real budget, but the realistic way in is as a subcontractor or through a small PoC.
- Not done / blocked: most contract values are withheld; several awards are still pending (DAK, BIG, gkv informatik, AOK Rheinland/Hamburg, MD RLP re-tender). AOK Hessen taking checks back in-house is a search snippet only (aok.de: WebFetch DNS fails, page is JS-rendered). caery customers not found. No [C] buyer voices.
- Next: A13. Critic: review `research/payer-processing.md`. A14 should fix "93 insurers" → 92 and the I5 WTP wording using this file.
- Tasks added: none.
- Open questions: none new. (The MD-IT deadline of 2 Dec 2026 is informational only; any contact with bidders would need CEO approval.)

### 2026-11-07 — CEO decision: scoring method (orchestrator)
- Done: applied the CEO's choice to `research/scoring.md`: option (b) knock-outs K1 (no buyer with proven spend) and K2 (no startup-accessible first sale in ≤12 months), plus ranking by confidence (R1–R4: H/M/L tag per score, L counts ≤3, criterion 3 or 5 at L = "unproven", sensitivity check, tiers instead of exact ranks). The 9 criteria and weights are unchanged (max 90), so `templates/venture-brief.md` needs no change.
- Not done: the other red-team proposals (new criteria/weights, K3–K6, minimum bars) were not adopted.
- Next: B1 uses the revised method. A18 (long-list fields incl. first-sale route) supplies the K1/K2 data.

### 2026-11-07 — Red team of research/scoring.md (critic)
- Done: RED TEAM review of the Stage B method → `research/reviews/2026-11-07-redteam-scoring.md`. Verdict: **fail as is**. Reasoning only; 3 new facts checked for the proposed scheme (Art. 20 BayWiVG direct award ≤€100k; federal ≤€50k from 1 Jul 2026; EU threshold €216k 2026–27).
- Fatal objections: (1) purely additive: a "payer unclear" idea beats a clear-payer idea 68 vs 61; (2) "budget owner" ≠ startup can sell (tenders need €0.25–6m turnover, references, KHZG certificate), and direct-award/private-buyer routes are not rewarded either; (3) founder fit = topic match, not buyer access, domain edge, part-time feasibility or co-founder dependency; (4) a score of 3 needs no evidence, so unknowns hide in the middle, and a free pilot meets "achievable"; (5) "≥€1bn EU" market size is top-down and ignores buyer counts (e.g. 15 MDs).
- Proposed: 6 knock-outs + 8 criteria (weights 4/4/3/3/2/2/1/1, max 100) + H/M/L confidence (L capped at 3) + sensitivity check and tiers. `scoring.md` not edited.
- Tasks added: A18 (researcher: long-list fields signer / budget line / first-sale route / status quo / wedge / buyer count), after A7.
- Not done: no B1 scores computed; worked examples are illustrative only.
- Open questions: CEO decision on the scoring scheme (see Open questions).

### 2026-11-07 — A11 Hospital billing audits & coding: size, rules 2027, incumbents (researcher)
- Done: `research/hospital-billing-audits.md`.
  - Size [A]: 1,138,534 MD audit reports in 2025; 48.9 % led to a reduction (avg €2,219.51). My math: ≈ €1.58bn/yr back to insurers (reductions + pre-audit dialogue + penalties). 27 % of audit reasons are coding; 68 % are medical necessity / length of stay.
  - Rules [A]: the BStabG (law, 1 Jan 2027) raises audit quotas to 5/20/40 % (thresholds 80/65 %), with no cap below 50 %, and a €500 penalty and fee. The "switch to sample audits from 2027" in `pain-professionals.md` S3 was a 2024 KHVVG draft and was never enacted, so A14 should fix S3. A 1 % tier for hospitals ≥90 % is pending (Bundesrat 20 Nov).
  - Static simulation on Q2 2026 data: 1,100 of 1,524 hospitals would land in the 40 % tier, and the legal cap rises ~4×. The MD's capacity (2,135 physician FTE) is the real limit. MD Niedersachsen already outsources 20,000 audits (€2m tender).
  - Budget [B] (DKI, Sep 2026): ~4,000 FTE / €245m/yr on audit handling; 51 % of hospitals plan AI for MD audits (median €40k).
  - Incumbents: Tiplu (LOGEX since Jul 2026; MBEG-Assistent in ~30 hospitals; >130 partner hospitals) and calliora (Munich, $6m pre-seed, double-digit hospitals) target exactly the 2027 pain. Also ID Berlin and Dedalus RICO.
  - Inference: big, budgeted, deadline-driven pain, but a crowded window. A newcomer would need a wedge (the payer/MD side, psychiatry/rehab, small private hospitals).
- Not done / blocked: status of the 1 % tier; Q3 2026 statistics (due ~end Nov); GKV-SV/DKG § 17c Abs. 7 report not found; Solventum/3M PDFs blocked (403/404); identity of UK Frankfurt's winner unconfirmed.
- Next: A12. Critic: review `research/hospital-billing-audits.md`.
- Tasks added: A17 (refresh with Q3 2026 data and the 1 % tier decision), inserted before A7.
- Open questions: none new.

### 2026-11-07 — A8 Critic fact-check run 3 (critic)
- Done: fact-checked every research file changed or new since its last review: `research/reimbursement-routes.md` (pass with fixes), `research/munich-ecosystem.md` (pass with fixes), A10 revisions of `research/trends.md` and `research/sources-map.md` (pass). Re-opened ~45 sources; all key numbers match (Bitkom, BStabG/§ 134, PNOG § 11, KHZG penalty annex, DAK, Destatis, Senate answer). TED recipe (637 / 366 cn / 384 procedures / 232 / 140) and ClinicalTrials.gov (300 / 669) reproduce. Reviews: `research/reviews/2026-11-07-*.md`.
- Top issues: (1) SCE Incubation "rolling basis" is not on the SCE page (fixed deadline 2 Aug 2026, passed), and UnternehmerTUM "no equity" is not sourced: the part-time founder path depends on both. (2) A9 still carries the "weak uptake" framing and an unsourced causal claim ("IT capacity, not money") that A10's DAK data contradict; GKV-SV press release graded [A] should be [B]; PNOG Länder co-funding "must" vs draft "sollen". (3) Munich "capital available / B2B workflow AI trend" rests on two deals and omits Bayern VC volume -46% YoY (EY); FLÜGGE "funded up to six projects" is only a plan.
- Not done: pain-* files not re-checked after A14 (A14 still open); ~19 of 43 A9 URLs and ~10 A6 URLs not opened (listed in the reviews); KHSFV § 19 unreachable (connection reset).
- Tasks added: A16 (researcher: apply fixes, combine with A15), inserted before A7.
- Next: researcher A15 + A16, A11-A14; critic reviews new outputs.
- Open questions: none new.

### 2026-11-06 — A10 Apply critic fixes to trends.md and sources-map.md (researcher)
- Done: revised `research/trends.md` and `research/sources-map.md` per both critic reviews.
  - Counts verified [A]: 32,054 care facilities in Dec 2023 (16,505 nursing homes + 15,549 outpatient services, Destatis) and 1,807 hospitals in 2025 (529 public, 549 non-profit, 729 private; Destatis PM 28 Oct 2026). KHZG €4.3bn verified (BMG); DigitalRadar 33.3 → 55.0 (DKG).
  - Framing fixed: the 8.5% FTE cut is a conditional ("müssten"); PNOG and GeDIG are marked as draft everywhere (GeDIG 2nd/3rd reading planned 13 Nov, PNOG 11 Dec 2026); KIM 40% = "applied for"; Pflegestatistik: 800,000 in homes, the definition explains the rise only "zum Teil", 640,000 Pflegegrad-1 people used no services. The old-age-ratio row was correct (33 → 43/45/47 by 2038); I added a note on the second measure.
  - PNOG updated to the cabinet draft: €1.6bn for outpatient **and residential** care, Länder "sollen" co-fund 25%. New: § 113e "Transformationsstellen" lets nursing homes convert up to 10% of the staffing corridor into a tech budget (2028–2032), but only for systems on an evidence catalogue (from 30 Sep 2027).
  - § 8 Abs. 8 grant uptake: DAK processes 48% of facilities. ~11,300 of its ~17,500 used the grant by mid-2025 (64.6%), but only €81.2m ≈ 40% of the funds was drawn. This softens A9's "weak uptake": facilities apply, but small amounts.
  - TED de-duplicated: 637 notices = 384 procedures (366 contract notices = 232 procedures, 139 buyers). Medical-software CPV contract notices: 140 procedures from 110 buyers. Added coverage limits (public buyers only; 729 private hospitals invisible).
  - Job counts downgraded to [C]; kununu needs ≥3 employers; App Store recipe must report the low-star share.
  - New source sections: Munich/Bavaria (KVB, StMGP Krankenhausplan 2026 PDF, Bavarian statistics office, LGL, BKG, AOK Bayern, München Klinik) and provider directories/filings (G-BA quality reports, InEK, AOK-Pflegenavigator, CGM/NEXUS IR, Bundesanzeiger, gematik dashboard = JS only).
  - ClinicalTrials.gov: "Munich" finds 300 recruiting trials, "Munich OR München" 669. A13 must use both spellings.
- Not done / blocked: national (AOK or GKV-SV) uptake of the § 8 Abs. 8 grant not found; incumbent care-software vendors not checked (`[UNVERIFIED]`). Blocked: pflegelotse.de (reset), pflegeportal.bayern.de and lfstat.bayern.de (502).
- Next: A11. Critic: re-check `research/trends.md` and `research/sources-map.md`.
- Tasks added: A15 (update `research/reimbursement-routes.md` with § 113e and the DAK uptake data), inserted before A7.
- Open questions: none new.

### 2026-11-06 — A9 Reimbursement & funding routes for digital health products in DE (researcher)
- Done: `research/reimbursement-routes.md`. 11 routes, each with who decides, amount, timing, evidence and status, almost all from primary law texts and drafts.
  - DiGA: BStabG (in force 30 Jul 2026) adds volume discounts from 2027 (2 % above 3,000 uses/yr, up to 30 % above 100,000) and mandatory first-year price caps. GKV spent €171m in 2025 (0.05 % of GKV spending).
  - DiPA: still zero listed (BMG, Jun 2026). €53/month. Benefits navigation and admin apps are excluded by law.
  - PNOG fund (cabinet 30 Sep 2026): €1.6bn federal + €0.4bn Länder, now also for residential homes. Payouts from 1 Jul 2027; guideline due 30 Jun 2027. My math: ≈€62k per facility over 5 years. Bundestag vote planned 11 Dec 2026.
  - Precedent: the €12k digitisation grant had been used up by only ~20–30 % of facilities in Berlin/Brandenburg by 2024.
  - Hospitals: the transformation fund is not a software budget. No KHZG successor. The KHZG penalty starts weighting actual use: 20 % of it in 2027, 80 % in 2031.
  - Insurers: § 140a contracts are now bound by contribution stability; admin-cost cap from 2027; Innovationsfonds down to €100m/yr.
  - Inference: B2B sales to providers out of their own budgets come first; DiGA/DiPA are later options.
- Not done / blocked: national uptake of the § 8 Abs. 8 grant (only regional vdek data); the current DiGA count (BfArM directory needs JS); the PNOG Bundestag Drucksache (AOK timetable used instead); prevention-course subsidy amounts; PKV. The task's "§64e" is genome sequencing, so § 140a/§ 68a–b were covered instead.
- Next: A10. Critic: review `research/reimbursement-routes.md`.
- Tasks added: none.
- Open questions: none new. Note for B1: suggest that a willingness-to-pay score of 4–5 requires a first revenue route within 12 months that does not depend on a reimbursement listing (`research/reimbursement-routes.md` §7).

### 2026-11-06 — A6 Munich ecosystem: grants, capital, co-founders (researcher)
- Done: `research/munich-ecosystem.md`. Grants (10 programs, with part-time fit), hubs (11), investors (~17), co-founder channels (9), all with sources.
  - Key: the founder stipends (EXIST €2,500/month, FLÜGGE) are not compatible with a full-time job. EXIST allows no active employment and ≤20 h/month of side work, but a sabbatical is OK; applications are accepted until 31 Dec 2027. FLÜGGE requires membership of a state Bavarian Hochschule.
  - Part-time-compatible now: SCE Incubation (≥10 h/week, rolling, prepares for EXIST), UnternehmerTUM Incubator (free, co-founder matching), BayStartUP business plan competition (phase 1 deadline 13 Jan 2027).
  - After founding: Start?Zuschuss! (50 %, max €36k; round 23 planned 25 Nov 2026–10 Jan 2027). EXIST must be approved before founding a company.
  - EIC Accelerator needs TRL 6+. EIT Health (HQ Munich) programmes are closed for now.
  - Competitor signal for A11: Calliora (Munich, AI for hospital billing) raised a >€5.3M pre-seed in Oct 2026 (BHI, Redalpine).
- Not done / blocked:
  - BayTOU 2026 status, INVEST end date and any 2026 BayDiGuP call are unverified.
  - Not opened: Heal Capital (DNS fail / reset), Peppermint and Redalpine (bot check), eu-startups (403). The Munich Startup Insights investor database has been shut down (410).
  - Not covered: pilot partners (Munich university hospitals, insurer innovation units).
- Next: A9. Critic: review `research/munich-ecosystem.md`.
- Tasks added: none.
- Open questions: CEO: is a sabbatical or leaving the job within ~12 months conceivable? EXIST (≈€30k stipend + €30k materials for a team) depends on it. Optional (outward, needs approval): ask SCE / UnternehmerTUM whether a non-alumnus working full-time can join.

### 2026-11-06 — A8 Critic review of Stage A, run 2 (critic)
- Done: reviewed `research/pain-industry.md` (needs work), `research/pain-professionals.md` (needs work) and `research/pain-patients.md` (pass, minor fixes). Re-opened ~45 sources, 9 TED notices (incl. selection criteria), 4 App Store review feeds and the ClinicalTrials.gov counts; nearly all numbers match, App Store and CT.gov counts reproduce exactly. Reviews in `research/reviews/2026-11-06-pain-*.md`.
- Top issues: (1) tenders used as "High WTP" (I5, S3, S8) exclude startups: AOK Hessen requires EUR 6m annual turnover, MUL Lausitz EUR 1m/yr in-field turnover, Charite 3 university-hospital references, Helios a KHZG certificate; DAK's re-tender ("weiterhin") has an incumbent. They prove buyer budget, not startup access. (2) DAK "EUR 890m" is claims volume processed, not contract value; "9 buyers" mixes scanning BPO with billing checks; "1.52m assessments in 2014" is not in the cited vdek page. (3) Harzklinikum "LLM discharge letter" tender is a clinical decision-support system (likely MDR software, needs primary source); A3 [C] counts mix opened threads with titles; ePA app tally picks the worst-rated standalone ident apps.
- Not done: ~40 sources not re-opened (sample-based); Jones Day (Biotech Act) behind Cloudflare on re-fetch. No venture briefs yet (no pre-mortem).
- Tasks added: A14 (researcher: apply A3-A5 fixes, incl. tender eligibility per WTP item), inserted before A7. A8 left open (notes updated).
- Open questions: none new.

### 2026-11-06 — A5 Pain mining: pharma, clinical research, payers, health admin (researcher)
- Done: `research/pain-industry.md`, with 10 problems (I1–I10), each with who has it, who pays, [A]/[B] backing, [C] counts and purchase evidence.
  - Clinical trials (I1/I2), best founder fit:
    - German sites under-recruit: 72 % of university sites miss their plan by ≥25 % (pharma/CRO barometer, Aug 2026).
    - Germany's share of trial participants fell from 4.5 % to ~3 %. My own ClinicalTrials.gov count: industry trials with a German site fell from 15.4 % of all trials (2015) to 10.5 % (2025).
    - Policy is speeding up approvals (MFG, standard contract clauses, EU Biotech Act). Site staff and patient finding remain the gap.
    - Counter-evidence: sponsors rated digital tools a minor hurdle in 2025, and the tool market is crowded (65 trial-management products on Capterra DE).
  - Payers (I5/I6), clearest willingness to pay so far:
    - 9 statutory insurers tendered outsourced invoice/receipt processing since 2025. AOK Hessen: 19.3m invoices over 4 years. DAK: €890m/yr, 2.0m receipts.
    - The MDs are buying AI-assisted assessments (MD RLP care-level assessment pilot, MD Nordrhein malpractice reviews).
    - From 2027, insurers' admin spending may only grow with insured income (§ 4 Abs. 5 SGB V).
  - Other industry pain:
    - EU HTA joint clinical assessment (JCA) dossiers: resource-heavy, but only ~58 JCAs a year and the space is full of incumbents.
    - MDR/IVDR certification: 19.5–21.8 months; 53 % of DACH manufacturers cut R&D. The EU revision proposal (Dec 2025) may shrink this pain.
  - Weak buyers: public-health offices (the federal ÖGD pact ends in 2026) and pharmacovigilance (flat case volume).
- Not done / blocked:
  - The [C] base is thin. Industry pain is not in open forums: Elsmar Cove returned 403, medi-learn has only old career threads, and the krankenschwester.de search needs a session token. Reddit was not used.
  - Primary EU texts were not opened (eur-lex bot check): HTA Regulation, MDR revision, Biotech Act. Law-firm and trade-press summaries were used instead.
  - Not identified yet: the incumbent outsourcers in the payer tenders and the DACH trial-recruitment vendors (snippet only).
- Next: A6 (Munich ecosystem). Critic: review `research/pain-industry.md`.
- Tasks added: A12 (insurer invoice processing and MD assessment automation: incumbents, contract values, buying route) and A13 (clinical-trial recruitment in DE: site economics, vendors, Kapazitätsinitiative 2030), both inserted before A7.
- Open questions: none new. Interviews in Stage D matter more for B2B buyers (sponsors, insurers), whose pain does not show up in public forums.

### 2026-11-06 — A4 Pain mining: clinicians, nurses, practice & hospital staff (researcher)
- Done: `research/pain-professionals.md`, with 10 problems (S1–S10), each with who has it, who pays, [A]/[B] backing, opened [C] counts and purchase evidence.
  - Strongest pain: documentation load. The hospital association institute DKI puts it at 3 h/day for physicians and 2.8 h for nurses (self-estimate). The only measured German study found 93 min/day (19.4 %).
  - Clearest budget owner: hospital coding and MD-audit work. Charité tendered outsourced coding support, Lausitz tendered AI coding software, and DKI ranks MD queries as the most time-consuming duty.
  - Practices: payer requests cost more than 2m hours/yr (KBV), and more than half of practices have weekly TI outages.
  - Funding is shifting. From 2027 the KHZG penalty (up to 2 % per case) starts counting actual *use* of digital services. Under the BStabG, the 2.5 % nurse-relief top-up is clawed back from 2027, and Pflegebudget overruns are no longer refinanced.
  - Counter-evidence: measured AI-scribe gains are modest (16 min per 8 h in JAMA 2026; 15 min per shift in care homes), voize ($50m, 1,100 facilities) already leads in care homes, AI phone assistants are crowded at €9–229/month, and in employer reviews leadership is a bigger complaint than software.
- Not done / blocked:
  - kununu shows page 1 only (the rest sits behind a sign-up, not bypassed), so only kununu's AI summaries were used.
  - krankenschwester.de and medi-learn are low-traffic: 8 threads opened, the rest are titles only. Reddit was not used.
  - LinkedIn job counts are unreliable (fuzzy matching) and StepStone no longer shows counts, so job ads were not used.
  - Not extracted: MD audit volumes, coding incumbents, uptake of the §8(8) SGB XI care-digitisation subsidy.
- Next: A5 (pain mining: industry/payers). Critic: review `research/pain-professionals.md`.
- Tasks added: A11 (hospital billing audits & coding: size, 2027 rule changes, incumbents), inserted before A7.
- Open questions: none new. A Reddit API key would help most for r/medizin and r/Pflege voices.

### 2026-11-06 — A3 Pain mining: patients & caregivers (researcher)
- Done: `research/pain-patients.md`. 11 problems (P1–P11), each with who has it, who pays, [A]/[B] backing, opened [C] signal counts and willingness-to-pay evidence. Strongest: P1 navigating home-care benefits (counselling used by 3% of those entitled, GKV-SV 2026; only 38.4% of Pflegegeld recipients use the relief budget); P2 finding care capacity (91% of home-care services refused new clients, DEVAP 2023); P3 carer overload (WIdO 2026: 46.9% of employed carers highly burdened, €469/month out of pocket); P4 specialist access (25% wait >30 days, GKV-SV 2025). Also: ePA onboarding friction (App Store: 271 of 300 recent reviews of DAK ePA, BARMER eCare and TK-Ident are ≤2 stars), medication shortages, discharge gaps, cancer orientation, rare-disease odyssey (4.7 years, EJHG 2024). Counter-evidence recorded: WIdO finds non-use of care benefits is mainly "no need" or preference, not missing information; the Innovation Fund navigator review found mostly no effect.
- Not done / blocked: [C] base is thin. Reddit was not used; alzheimer-forum.de (403), pflege-forum.org (502), demenz-portal/treffpunkt-pflege (TLS) and patient.info (empty) were unreachable, so P2 and P5 have no opened forum items. ME/CFS, rural GP access and 24-h care figures are snippet-only `[UNVERIFIED]`. Several key data points are >3 years old (flagged in the file).
- Next: A4 (pain mining: professionals). Critic: review `research/pain-patients.md`.
- Tasks added: none.
- Open questions: Reddit API key would mainly help P2, P3, P5 (caregiver and psychotherapy voices).

### 2026-11-06 — A8 Critic review of Stage A (critic)
- Done: reviewed `research/sources-map.md` (pass, minor fixes), `research/trends.md` (pass, minor fixes), `research/scoring.md` (needs work before B1). Re-opened 21 trends sources and re-ran 10 source-map access tests; nearly all numbers match. Reviews in `research/reviews/2026-11-06-*.md`.
- Top issues: (1) the PNOG €1.6bn "budget for a startup" inference ignores the existing §8 Abs. 8 SGB XI care-digitisation grant (max €12k/facility since 2019), whose uptake is the best test of whether grant money becomes purchases; per-facility rules only come with GKV-SV guidelines due 30 Jun 2027. (2) The TED "637 notices" are not de-duplicated (30 of the first 50 are award notices) and half the titles are generic IT; they show public-hospital IT demand, not startup willingness to pay. (3) scoring.md is purely additive (no knock-out for "unclear who pays"), lists DiGA as a 5-level payer example, and has no evidence-confidence dimension.
- Not done: ~19 trends sources not re-opened (sample-based); no venture briefs exist yet (no pre-mortem).
- Tasks added: A10 (researcher: apply trends/sources-map fixes), inserted before A7. A8 left open (notes updated).
- Open questions: CEO: should `research/scoring.md` get knock-out rules (willingness to pay ≤2 or achievability ≤2 → not top 5), a confidence tag per score, and a non-DiGA example for criterion 3 before B1? (Stage B tasks can't be added from Stage A.)

### 2026-11-06 — A2 Source map (nightly researcher)
- Done: `research/sources-map.md`. About 200 URLs across 9 source types were access-tested (curl/WebFetch/WebSearch), each with signal type, grade, access result and recipe. Works: German forums (krankenschwester.de, krebs-kompass, rheuma-online, diabetes forums, onmeda, medi-learn), kununu (incl. review text), App Store API/RSS + Google Play, LinkedIn Jobs/StepStone counts, TED tender API (637 DE hospital IT notices since 2025), G-BA Innovationsfonds (861 projects), CORDIS/EU F&T APIs, BMG/G-BA/Bundestag/insurers, Destatis/Eurostat/OECD SDMX, PubMed E-utilities, Europe PMC REST, ClinicalTrials.gov API, most trade press. Per-task recipes for A3–A6/A9 are included.
- Not done / blocked: Reddit (bot challenge, 0 reddit.com hits in DE `site:` searches; third-party mirrors not used, and the sandbox denied testing them); Facebook/LinkedIn posts (login wall); Google Trends (429); Trustpilot, Indeed, Glassdoor, Crunchbase, Dealroom, OECD web, europepmc.org web, gutefrage, allnurses, Tagesspiegel Background, Ärzte Zeitung, Springer Medizin (bot checks); BA Jobsuche API, Förderkatalog, foerderdatenbank, BAS, SVDGV, Medical Valley EMN (403/502/reset). WebFetch DNS fails for nearly all hosts.
- Next: A3 (pain mining: patients & caregivers). Critic: review `research/sources-map.md`.
- Tasks added: none.
- Open questions: Reddit API key (see Open questions, now more important).

### 2026-11-06 — A1 Trends & policy scan (DE/EU) (nightly researcher)
- Done: `research/trends.md`. Ageing (Destatis 16. kBV), care demand and workforce gap, physicians, chronic disease, hospital reform (KHVVG/KHAG, €50bn fund), digitisation (ePA, GeDIG, FDZ, DiGA, Notfallreform, EHDS, AI Act Omnibus) and cost pressure (GKV/SPV, FinanzKommission, BStabG), each with figures, who is affected and who pays. ~40 sources opened, graded [A]/[B]. Key inference: payers are cutting costs, while new public digitisation money is flowing to providers (PNOG €1.6bn for outpatient care 2027–31, hospital transformation fund). Treat this as input for A7, not as a conclusion.
- Not done / blocked: primary Destatis releases for health spending 2024 and causes of death 2025 (used [B] reports instead); RKI/GBE prevalence data; PNOG cabinet version (used the 5 Jun 2026 draft). WebFetch DNS-blocked destatis.de, bundesgesundheitsministerium.de and vdek.com, so all were fetched via curl. eur-lex.europa.eu returns 202/empty (bot check), oecd.org returns 403, gesetze-im-internet.de does not connect.
- Next: A2 (source map). Critic: review `research/trends.md`.
- Tasks added: A9 (reimbursement and funding routes for digital health products), inserted before A7 because the long list and B1 criterion 3 need it.
- Open questions: none new. (Optional: allowlist eur-lex.europa.eu and oecd.org for primary EU texts.)

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher, run 2)
- Done: verified GLOBOCAN 2024 world/Portugal/Germany figures, CDC colorectal 45–75 gap (B), CDC MMWR lung screening 2017 (A, >3 yrs old); added founder-fit ranking per updated task description; recommendation changed A → C (inference). Rewrote `research/problem-statement.md`.
- Not done / blocked: C, D, E core numbers and A's 2022 national figure still `[UNVERIFIED]` (PubMed/PMC bot check; frontiersin.org and uspreventiveservicestaskforce.org DNS-blocked; ascopubs 403). V1 left open.
- Next: verify C first (it is now the top pick); V10.
- Tasks added: V10 (EU/PT/DACH evidence for C and A).
- Open questions: host allowlist (updated list above); does the CEO agree founder fit should outweigh verified-gap size?

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher)
- Done: drafted `research/problem-statement.md` — 5 candidate problem spaces (A lung screening uptake, B colorectal screening 45–49, C trial enrollment, D financial toxicity, E time-to-treatment), each with problem, who has it, likely payer, key assumptions; provisional recommendation A, runner-up C.
- Not done / blocked: no source could be opened (hosts blocked by network allowlist: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com). All numbers come from WebSearch summaries and are marked `[UNVERIFIED]`. V1 left open with notes.
- Next: verify leads once hosts are allowed; add IARC/EU data.
- Tasks added: none.
- Open questions: host allowlist; US vs EU vs global focus (see Open questions).

### 2026-11-06 — Setup
- Done: created workspace structure.
- Not done: no research yet (by design).
- Next: V1.
