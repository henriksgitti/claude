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

## CEO decision 2026-11-11
- **Deep dive on idea 1 only: eldercare navigator as an employee benefit (L01).** Stage C started; C1 unblocked. Other shortlist ideas are parked, not killed.

## Next steps
- (2026-11-11) Critic: C2 fact-check and pre-mortem of the L01 brief. CEO: C3 (go to Stage D / revise / drop). Researcher: no open unblocked task after C1 (A17 waits for 2026-12-01; A24/A26 deferred). The numbered list below is from Stage B.
0. **CEO: B3 — pick 2–3 ideas for deep dive** from `research/shortlist.md` (recommendation: L01 + L03 as one 'carer support' brief, plus L07). Critic: B2 review of the shortlist.
1. Researcher: B4 done 2026-11-08. No open unblocked task (A17 waits for 2026-12-01; A24/A26 deferred; C1 waits for B3). Critic: B2 red team (B4 done).
2. After B3: C1 venture briefs for the picked ideas.

## Open questions
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
