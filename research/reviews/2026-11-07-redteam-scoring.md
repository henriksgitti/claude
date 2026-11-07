# Red team: research/scoring.md (Stage B method)
Date: 2026-11-07 | Mode: RED TEAM (attacks the reasoning, not the sources) | Verdict: **fail as is: do not run B1 with it**

Viewpoint: (a) the person at the buyer who must sign the order, (b) a Munich pre-seed/seed investor reading the shortlist. Context used: `founder-brief.md`, `research/trends.md`, `research/reimbursement-routes.md`, `research/pain-*.md`, `research/munich-ecosystem.md`, all reviews incl. `2026-11-06-scoring.md`.

The 2026-11-06 review already asked for knock-outs, a confidence tag, a non-DiGA example for criterion 3, a bottom-up market method and separate user/buyer/budget fields. **None of these is in `scoring.md` yet** (it is unchanged since then, and the CEO has not decided). This review does not repeat those points. It shows why they are fatal, adds the problems they miss, and proposes a full replacement scheme for the CEO to approve.

## Fatal objections (any one makes the ranking unreliable)

**F1. A no-payer idea can beat a clear-payer idea, and this is likely to happen on the actual long list.** The scores are added with no gate, so "Unclear who pays" (criterion 3 = 1) costs only 6 of 90 points against a 3. Illustration with plausible scores for pain-patients **P3** (carer overload, table: "payer unclear") vs. a modest B2B idea with a proven budget:

| Criterion (weight) | P3-type: "carer app, payer unclear" | Modest B2B, clear payer |
|---|---|---|
| Pain (3) | 5 → 15 (WIdO data + 104 threads) | 3 → 9 |
| Market (2) | 5 → 10 (3.1m families, top-down) | 3 → 6 |
| WTP (3) | **1 → 3** | **5 → 15** |
| Founder fit (2) | 4 → 8 (care coordination = "sweet spot") | 3 → 6 |
| Achievability (2) | 4 → 8 (a free pilot counts, see F4) | 3 → 6 |
| Regulatory (1) | 5 → 5 | 4 → 4 |
| Fundability (2) | 4 → 8 (EXIST, BayDiGuP care call) | 3 → 6 |
| Competition (2) | 3 → 6 | 3 → 6 |
| Future (1) | 5 → 5 | 3 → 3 |
| **Total** | **68** | **61** |

The idea with no buyer wins by 7 points. In general, an idea with criterion 3 = 1 can still reach 78/90. A buyer would never sign it and an investor would stop reading at "who pays?". **Cheapest fix:** knock-out K1 below (one line in `scoring.md`).

**F2. "Who pays" is scored, but "can a 1–2-person startup sell to them" is not.** Criterion 3 gives a 5 for a "clear budget owner (payer, hospital, pharma, employer)". The research already shows that budget owners with proven spend lock out a new company:
- AOK Hessen § 302 tender: minimum turnover **€6m/yr**; BIG: €250k turnover + **3 comparable references**; DAK: re-tender with an incumbent (`research/reviews/2026-11-06-pain-industry.md`, issue 1).
- MUL Lausitz AI coding: **≥€1m/yr turnover in the field** for 3 years; Helios discharge platform: **KHZG certificate + hospital-group reference** (`research/reviews/2026-11-06-pain-professionals.md`, issue 1).
- `lessons.md` 2026-11-06 already says it: "A tender proves a buyer budget, not startup access."

Under the current scheme S3 (hospital coding) and I5 (§ 302 processing) get WTP = 5 and keep it. A buyer reading the score would say: "I'm not allowed to buy from you." The scheme also misses the routes that **do** work for a startup, so it cannot reward them either:
- **Direct award without a tender:** Bavarian state and municipal buyers up to **€100,000 net** for supplies and services ([Art. 20 BayWiVG](https://www.gesetze-bayern.de/Content/Document/BayZustWiG-20), opened: "ein Direktauftrag ist bis zu einer Wertgrenze von einschließlich 100 000 € ohne Umsatzsteuer zulässig") [A]. Federal buyers up to €50,000 since 1 Jul 2026 ([IHK Schwerin on the Vergabebeschleunigungsgesetz](https://www.ihk.de/schwerin/recht/aktuelles/vergabebeschleunigungsgesetz-ab-01-07-2026-7060088)) [B]. The EU tender threshold for most public buyers is **€216,000** for 2026–27 ([IHK Hannover](https://www.ihk.de/hannover/hauptnavigation/unternehmensfoerderung/oeffentliches-auftragswesen/aktuell-auftragswesen/neue-schwellenwerte-fuer-eu-ausschreibungen-fuer-2026-und-2027-6927176)) [B].
- **Private buyers:** 729 of 1,807 hospitals are private (`trends.md`, Destatis), as are most care operators and all pharma/CROs. As private companies they are generally not bound by public procurement law (`[UNVERIFIED]` in this review; exceptions such as publicly funded projects are not checked). They still run vendor qualification: IT security, GDPR data-processing agreements, and GxP/CSV audits in pharma.
- **Channel or subcontract:** e.g. caery selling via Telekom (`2026-11-06-pain-industry.md`).

**Cheapest fix:** split criterion 3 into "budget proven" and "startup-accessible first sale" (C2/C3 below), and add knock-out K2.

**F3. Founder fit is scored as topic match, not as the ability of *this* founder to win the first customer.** Criterion 4 asks whether the idea "matches `founder-brief.md` strengths (health innovation, AI/automation, German market)". Almost every admin-automation idea gets a 4–5 on this, so the criterion does not tell ideas apart. What the founder brief actually implies, and the criterion ignores:
- **Buyer access:** the brief lists no German healthcare buyer network. The CEO's work is in asset management in Lisbon (~1.5 years). Can he get a meeting with a hospital CFO, a care-home operator or a CRO head of feasibility? This differs a lot by idea and is the first thing an investor asks.
- **Domain edge:** the CEO's stated interest is drug development and clinical research (brief, "Interests"), but he has no work experience there. A "fit" score that treats interest as an edge will over-score I1/I2.
- **Part-time feasibility:** enterprise and hospital sales happen in working hours, with on-site meetings and procurement paperwork. A product sold self-serve to many small buyers, or validated through remote interviews, suits ~10 h/week. One sold via months of committee meetings does not. SCE Incubation alone needs ≥10 h/week (`munich-ecosystem.md`).
- **Co-founder dependency:** the brief says to avoid ideas whose core needs skills the CEO lacks "unless the co-founder profile solves it". The scheme does not say *which* co-founder each idea needs, or whether that person is findable in Munich.
- **Investor view:** a part-time, solo, non-technical first-time founder is not fundable at pre-seed until a co-founder joins and there are first buyer signals. The competitor bar is visible: Calliora (hospital billing AI, Munich) raised >€5.3m pre-seed (`munich-ecosystem.md`).

**Cheapest fix:** replace criterion 4 with the four sub-questions in C4 below. Before B1, the CEO answers three yes/no questions per buyer type (see "Cheapest tests" 1).

**F4. The 1–5 scale lets unknowns hide in the middle and lets "achievable" be met for free.**
- "Show evidence links for every score ≥4 or ≤2" means a **3 needs no evidence**. Any criterion the research has not answered (incumbents in care documentation and hospital billing are explicitly `[UNVERIFIED]`, see `2026-11-07-trends-and-sources-map-A10-revision.md`) will default to 3 with no trace. Unknown ≠ average.
- Criterion 5: "**Pilot** or first customer in ≤12 months." A free pilot satisfies this. Buyers hand out free pilots easily and rarely convert them. Investors discount them to zero.
- "Flag any score based only on [C] evidence" is a flag with no consequence for the total.

**Cheapest fix:** evidence and confidence for *every* score, a cap on low-confidence scores, and "paid pilot or LOI with a named budget" as the bar (rules R1–R3 below).

**F5. The market-size criterion rewards the wrong number for this founder.** "≥€1bn addressable in EU" has no method (already raised) and **points the wrong way for a seed case.** A Munich seed investor wants (i) a bottom-up count of reachable buyers in DACH × a realistic price and (ii) a believable path to venture scale. A top-down "€1bn EU" passes for almost any healthcare theme. Meanwhile the real constraint can be buyer count, which the research already shows:
- I6 MD assessment: **15** buyers (all MDs). Even at €300k/yr each, the German SAM is €4.5m. This is too small for venture funding however "high" the pain.
- I5 § 302: **93** statutory insurers, concentrated, with tenders requiring €0.25–6m turnover.
- S2-type care software: **32,054** facilities (Destatis) × a few €k/yr. This is a large count but a low price, and voize already has 1,100 facilities (`pain-professionals.md`).

**Cheapest fix:** C5 below (buyers × ACV with sources, DACH first) plus knock-out K4 for small markets.

## Other weaknesses (with the cheapest fix)

| # | Weakness (quote / criterion) | Why it distorts the ranking | Cheapest fix |
|---|---|---|---|
| W1 | Ease is counted four times: "Achievability" (2), "Regulatory burden" (1), "Fundability" (2), "Founder fit" (2) all reward "low-regulation software" | 7 of 18 weight points go to the same trait, so an admin-software idea can start up to ~20 points ahead (7 weights × 3 score steps) whatever the buyer | Merge into one gated set: regulation becomes a knock-out (K3), fundability becomes a note, fit is redefined (C4) |
| W2 | Ageing is counted three times: "Pain" ("cost/harm"), "Market size & **growth**", "Future relevance" | Care and ageing themes get a structural bonus three times | Keep the trend in one criterion only (C8, weight 1) |
| W3 | Criterion 1 "Pain intensity": "people already pay **or hack workarounds**" | This mixes user pain (forum hacks) with buyer pain (money). It repeats the who-pays vs who-uses error | Score the **signer's** pain: cost, revenue at risk, legal duty, deadline (C1) |
| W4 | Criterion 7 "Fits EXIST, Bavarian programs, EU grants" | EXIST and Start?Zuschuss! do not depend on topic. Their binding constraint is the founder's employment status (`munich-ecosystem.md`: no stipend while employed). Every idea scores the same, so the criterion only adds noise | Drop it as a score. Keep a required "funding route" note; only BayDiGuP-type topic calls differ by idea |
| W5 | Criterion 6 "Regulatory burden", weight 1 | A class IIa device needs an ISO 13485 QMS and a notified body (avg. 19.5 + 21.8 months, `pain-industry.md` I4). The founder brief says to avoid it. With weight 1 it costs at most 4 points. AI admin tools also drift into clinical decision support (the Harzklinikum "discharge" tender was CDS, `2026-11-06-pain-professionals.md` issue 2) | Knock-out K3 for MDR IIa+/IVDR B+ before first revenue. Add a required "intended-purpose risk" flag |
| W6 | Criterion 8 "No strong incumbent in DACH; clear wedge" | (a) Ignores the status quo (Excel, paper, outsourced BPO, overtime, doing nothing), which is the most common competitor in healthcare. (b) Ignores incumbent suites (hospital IT system, PVS, care-software vendors) adding the feature. (c) "No incumbent" can mean "no market" | C6: score switching cost from the status quo and whether an incumbent can copy the feature within 12 months |
| W7 | Scoring a **problem**, not a problem + wedge | Achievability, regulation, competition and price depend on the product, not the problem. P1 as a Pflegekasse service and P1 as a family app score very differently | Required field: a one-line wedge (product, buyer, price) per scored row. Several wedges per problem are allowed |
| W8 | Ranking by exact total | With 9 criteria and ±1 noise on each, totals a few points apart are a tie. A strict top 5 will look more precise than it is | Use tiers (A/B/C) plus a sensitivity check (R4) |
| W9 | No "why now" trigger | Buyers sign when a deadline or penalty forces them to (e.g. KHZG penalty weighting use from 2027, the 2027 audit rules in A11). Without a trigger, "nice to have" ideas look as good as forced purchases | Part of C1 (urgency) |
| W10 | Draft-law money is treated like real money | PNOG (draft until the planned 11 Dec 2026 vote; payouts from 1 Jul 2027) and DiPA (0 listed) can make WTP look like a 5 | Knock-out K5: revenue cannot depend only on a rule not yet in force or on an empty route |
| W11 | `templates/venture-brief.md` shows "Score: <x>/90" | It will be wrong after any change of weights | CEO updates the template with the scheme (CEO-owned file) |

## Proposed revised scheme (for CEO approval; `scoring.md` not edited)

### Step 0: required fields per row (no score without them)
User · **signer** (role + organisation type) · budget line · wedge (one line: product, first customer type, price/ACV guess) · status quo today · trigger (why now) · first-sale route (direct award ≤€100k BY / ≤€50k federal, private buyer, channel, tender) · co-founder needed.

### Step 1: knock-outs (any one → "parked" with the reason; not eligible for the top 5)
| # | Knock-out | Test |
|---|---|---|
| K1 | No buyer with proven spend | No tender, contract, budget line, price list or observed paid purchase in the category. "Payer unclear" = out |
| K2 | No startup-accessible first sale in ≤12 months | Every known buyer route needs turnover, references or certificates a new company lacks, and there is no direct-award-sized pilot (≤€100k), private buyer or channel/subcontract route |
| K3 | Core needs MDR IIa+ / IVDR B+, a drug, or a clinical trial before first revenue | Per founder brief "avoid". A non-device wedge of the same problem may be scored instead |
| K4 | Too small | Bottom-up DACH SAM < €50m/yr **and** no sourced EU expansion path (threshold is a CEO parameter) |
| K5 | Revenue only via a rule not in force or an empty route | Draft law, DiPA (0 listed), unpassed fund; OK only if a payer exists today without it |
| K6 | Not a product problem | Root cause is headcount, leadership or national infrastructure (e.g. S6 TI, S9 leadership) |

### Step 2: scored criteria (1–5; anchors for 1/3/5; evidence link + confidence for **every** score). Weights sum to 20, so max = 100
| # | Criterion | W | 5 = | 3 = | 1 = |
|---|---|---|---|---|---|
| C1 | **Signer's pain and urgency** | 4 | Cost/revenue/legal duty quantified [A]/[B] + dated trigger (deadline, penalty) | Cost known, no deadline | Only user pain, no buyer cost |
| C2 | **Startup access to the signer** | 4 | Private or direct-award-sized buyers, many of them, short cycle (<6 months), no references needed | Mix: some accessible buyers or a channel partner | Only tenders with turnover/reference thresholds; ≤20 buyers |
| C3 | **Proven willingness to pay** | 3 | Buyers pay today for this category; price points known (tenders, price lists) | Adjacent spend exists | Only inferred |
| C4 | **Founder–idea fit** | 3 | CEO can reach signers via his own network, has a real edge, first test feasible at ~10 h/week, co-founder profile clear and findable in Munich | 2 of 4 | Needs full-time on-site selling + an unfindable specialist |
| C5 | **Market size, bottom-up** | 2 | DACH buyers × ACV ≥ €250m, EU path sourced | €50–250m | <€50m (= K4) |
| C6 | **Status quo and incumbents** | 2 | Status quo is costly and painful; no incumbent suite can add it within 12 months | Point competitors exist, differentiation plausible | Funded leader (e.g. voize, Calliora) or suite feature |
| C7 | **Cheap testability** | 1 | Riskiest assumption testable in ≤4 weeks of desk work + ≤10 interviews | Needs a pilot | Needs a build + clinical data |
| C8 | **Structural tailwind** | 1 | Grows with ageing/workforce/law in force | Flat | Shrinking or policy reversing |

### Step 3: confidence rules
- **R1** Tag every score H/M/L. H = ≥1 [A]/[B] item directly on point and no counter-source. M = indirect [B] or inference from [A]. L = [C] only, snippet only, or inference.
- **R2** An **L** score counts as **at most 3** in the total. Unknown = L = no bonus.
- **R3** C2 or C3 at L → row marked "unproven". It may enter the top 5 only with a named cheap test to run before Stage C.
- **R4** Sensitivity: re-rank with every L score −1. Report a row as top 5 only if it stays in the top 7. Present tiers, not exact ranks.

### Step 4: minimum bars
C2 ≥ 3 and C3 ≥ 3 and C4 ≥ 3 for the top 5 (beyond the knock-outs). Max 2 top-5 rows per buyer type, so the CEO gets a real choice.

### Illustration (not B1 scores)
- P3-type carer app: out at **K1** (no payer). Under the old scheme it scored 68/90.
- S3 hospital coding: passes K1. K2 depends on whether private hospital groups or ≤€100k Bavarian direct awards are a real route (A11 must check). C6 is low (Calliora, €5.3m pre-seed, Munich; Tiplu/LOGEX per `research/hospital-billing-audits.md`, A11, merged during this review and not reviewed here). C4 is low (no coding domain edge, no hospital network). Likely tier B: it falls for stated reasons, not hidden ones.
- I6 MD assessment: out at **K4** (15 buyers).

## Cheapest tests (before or during B1; none is an outward action)
1. **CEO, 10 minutes:** for each buyer type (hospital admin/CFO, care operator, practice, insurer, pharma/CRO, families): "Could I get a 30-minute call with a signer via my own network within 2 weeks? yes/no". Plus hours/week available and own validation budget (still TBD in the brief). This feeds C4 directly. Nothing else in the repo can answer it.
2. **Researcher, 1 run:** calibrate the new scheme on three known rows (P1, S2, S3) under both schemes, and show where the ranks differ and why. This is cheap and shows whether the change matters before 20–30 rows are scored.
3. **Researcher, in A7:** for every long-list row, fill the Step 0 fields. The first-sale route comes from TED `selection-criterion` texts and the private/public split of buyers. This is the data K1/K2/C2 need. It is added as task A18.
4. **B1 itself:** run the R4 sensitivity check and publish it next to the ranking.

## Assumptions to challenge
- That a high "pain" score predicts a sale. In this repo the biggest pains (P2 capacity, S7 staffing, S9 leadership) have root causes software cannot fix.
- That "fits the AI/automation sweet spot" is an advantage. It is the most crowded seed category in Munich (`munich-ecosystem.md`: the "B2B workflow AI" trend rests on two deals, and both are competitors).
- That the top 5 from desk research needs no buyer contact. Rule 5 forbids outreach without CEO approval, but test 1 only uses the CEO's own knowledge.
