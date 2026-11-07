# Red team: research/scoring.md (v2, after the CEO decision of 2026-11-07)
Date: 2026-11-07 | Mode: RED TEAM (reasoning, not sources) | Verdict: **needs work. Do not run B1 until fixes 1–6 are approved (each is a one-line edit).**

Scope: the revised `research/scoring.md` (knock-outs K1/K2 + confidence rules R1–R4; 9 criteria and weights unchanged, max 90). The CEO chose this as option (b). The rejected proposals (new criteria/weights, K3–K6, minimum bars) are **not** re-argued here. Data checked against: A18 (task text), the "Tender access check" tables in `research/pain-industry.md` and `research/pain-professionals.md` (A14), `research/payer-processing.md`, `research/hospital-billing-audits.md`, `lessons.md`.

## Summary
- **K1 works.** It removes "payer unclear" rows (the 68 vs 61 case in the first review). Its open edges are what counts as the "category" and whether a draft-law budget counts (fix 4).
- **K2 hardly ever fires as written.** It only knocks out a row when *no* direct-award, private-buyer or channel route exists. Some such route almost always exists in law, and the routes are invisible in the data (below-threshold and private purchases are not in TED). So K2 tests whether a route is legally possible, not whether a startup has ever sold that way (fatal 1).
- **R1–R4 mostly work as intended.** Four gaps remain: "inference" is listed under both M and L, unknowns still sit at 3, the order of R2 and R4 is not stated, and **tiers have no definition**.
- **A weak idea can still reach the top 5.** Route: K2 passes because a route is possible, and the WTP and achievability scores are tagged M ("inference from [A]"). Then R2 and R3 never fire. Worked example below.

## Fatal or near-fatal objections

**N1. K2 passes whenever a route is legally possible, so it barely filters.** K2 fires only if "Every known buyer route needs turnover, references or certificates a new company lacks, **and there is no** direct-award-sized pilot (≤€100k …), private buyer, or channel/subcontract route."
- *Private buyer:* 729 of 1,807 hospitals are private (`trends.md`), as are most care operators and all pharma companies and CROs. So the clause is met for almost every provider or industry row.
- *Direct award:* this is a legal option for every public buyer. Whether it is ever used for this product cannot be seen in the data. Both pain files say so: "Below-threshold hospital purchases are invisible in TED" (`pain-professionals.md`, Gaps); "Tenders below the EU threshold are invisible in TED" (`pain-industry.md`, Gaps).
- *Subcontract:* MD-IT allows it ("**No as prime; yes as subcontractor**", `pain-industry.md` tender table), but no prime is named.
- The researcher's own text already gives the escape route for the four hospital rows where **every** checked tender is "No", "Hard" or "Unknown" (S1, S3, S7, S8): "Realistic first sales: below-threshold purchases …, private hospital groups that buy outside TED, or co-selling with a KIS vendor" (`pain-professionals.md`, inference under the tender table). Under K2 as written, all four pass.
- So the A14 tender checks, the only hard access data in the repo, cannot knock anything out. A buyer would say: "We don't buy from companies without references." An investor would ask: "Name one hospital that bought from a startup like you."
- **The data to test K2 properly exists**, in the form of young vendors with paying customers in the same buyer type:
  - MPIRIQ (Munich, 2024; sells to practices, €99–329/month; `trial-recruitment-de.md`)
  - calliora (Munich, founded 2023; "double-digit" number of hospitals, vendor claim; `hospital-billing-audits.md`)
  - voize (1,100 care facilities; `pain-professionals.md`)
  - caery via Telekom (a channel to insurers; `pain-industry.md`)
  - MD RLP PoC (open to a new company with one AI PoC reference; `pain-industry.md`)
- **Fix 1:** reverse the burden of proof. Without such evidence, the row is marked "K2 unproven" rather than knocked out. This avoids killing rows only because the data is invisible.

**N2. Rows tagged M escape R2/R3, so "unproven" rarely triggers.**
- R1 says "M = indirect [B] or **inference** from [A]. L = [C] only, snippet only, **or inference**." The same word is in both tags. The researcher will tag most judgement calls M, and M has no consequence.
- Criterion 5 (achievability) is always a forecast. Criterion 4 (founder fit) has no graded source at all (`founder-brief.md` is not [A]/[B]/[C]). Read strictly, both are always L: R3 then marks *every* row "unproven" and stops telling rows apart. Read loosely, they are always M: R3 never fires. Both readings defeat R3.
- **Worked example: an S1-type row (AI discharge letters for hospitals) under v2.** Plausible B1 scores:

  | Criterion | Score | Tag | Basis |
  |---|---|---|---|
  | Pain | 5 | H | DKI, DMW |
  | Market | 5 | M | ~176,800 physician FTE, top-down |
  | WTP | 5 | M | 8 hospital buyers in TED + "private groups buy outside TED" |
  | Founder fit | 4 | M | |
  | Achievability | 4 | M | "direct award ≤€100k" |
  | Regulatory | 3 | H | Rule 11 IIa risk for decision-support features |
  | Fundability | 4 | M | |
  | Competition | 3 | L | incumbents not mapped |
  | Future | 5 | H | |

  - Total **78/90**; R4 takes off 2 → 76. K1 passes, K2 passes (N1), and R3 does not fire.
  - So the row lands in the top 5, even though every one of the 8 observed hospital tenders is closed to a startup and no startup sale to a hospital is documented for this product.
  - Fixes 1 and 6 together put WTP and achievability at L (capped at 3, total ≈ 70) and mark the row "unproven". It can then enter the top 5 only with a named test. That is the intended behaviour.

**N3. "Tiers (A/B/C)" have no definition, and R4 does not say what "top 5" is.** R4 says: "Report a row as top 5 only if it stays in the top 7. Present tiers (A/B/C), not exact ranks." It is not defined:
- what puts a row in tier A, B or C;
- whether "top 7" is counted among all rows or only K1/K2 survivors;
- what happens if fewer than 5 rows pass R4;
- whether an "unproven" row can be tier A.

B1 will make this up during scoring, after the totals are known. **Fix 5.**

## Other issues (B1 will trip over these)

| # | Issue (quote) | Why it matters | Fix |
|---|---|---|---|
| I1 | K1: "observed paid purchase **in the category**"; "budget line" | "Category" is undefined. Does a speech-recognition tender prove spend on AI discharge letters? Does § 302 scanning BPO prove spend on AI billing checks? Do families paying for 24-h live-in care (P11) prove a payer for a carer app? A vendor price list proves a price, not a buyer. A "budget line" in a draft law (PNOG, until the planned 11 Dec 2026 vote) is not proven spend, but K1 does not say so | Fix 4 |
| I2 | K1/K2 test "the category" / "buyer route"; the scores are per "problem" | A18 adds a one-line **wedge** (product, first customer, price), but `scoring.md` never says to score the wedge. One problem can have a closed route (I5 direct) and an open one (I5 via subcontract). Without a rule, B1 will mix the best K2 route with the biggest WTP budget from *different* buyers | Fix 3 |
| I3 | K2 cites only "Art. 20 BayWiVG for Bavarian public buyers, ≤€50k federal" | Statutory insurers and other social-insurance bodies have their own rule. **§ 22 Abs. 2 SVHV:** "Leistungen bis zu einem voraussichtlichen Auftragswert von 50 000 Euro ohne Umsatzsteuer können … ohne die Durchführung eines Vergabeverfahrens beschafft werden (Direktauftrag). Der Auftraggeber soll zwischen den beauftragten Unternehmen wechseln." ([gesetze-im-internet.de](https://www.gesetze-im-internet.de/svhv/__22.html), opened 2026-11-07) [A]. Still `[UNVERIFIED]`: whether the 15 MDs fall under the SVHV, and whether Art. 20 BayWiVG covers Bavarian university hospitals and municipal hospital GmbHs (e.g. München Klinik). B1 will otherwise apply €100k to every public buyer | Fix 2 |
| I4 | K2: "Every **known** buyer route needs …" | Tender rows marked "Unknown" (thresholds only in the tender documents: DAK, gkv informatik, MD Nordrhein, 5 hospital tenders) are not "known closed", so they keep K2 open. `lessons.md` (A14) already says: mark them "unknown", do not assume they are open | Fix 2 |
| I5 | R2: "An L score counts as at most 3 … Unknown = L = no bonus" | It is not clear what score an unknown gets. In practice it gets 3, which is the problem the first review raised in F4 ("Unknown ≠ average"). A row with no evidence on a criterion ties with one that has H evidence of an average result | Fix 6 (last clause) |
| I6 | R4: "re-rank with every L score −1" | Does the −1 come before or after the R2 cap? If before, an L-5 becomes 4, is capped to 3, and R4 changes nothing for exactly the scores it should test. Floor at 1? Ranked among which rows? | Fix 5 |
| I7 | R3: "a named cheap test to run before Stage C" | Most tests of WTP or achievability need buyer contact. That is an outward action (rule 5), and CLAUDE.md puts interviews in Stage D. The rule cannot be met as written unless the test is desk-only or the CEO approves the contact | Fix 7 |
| I8 | Criterion 2: "≥€1bn addressable in EU; state the buyer count" | A18 supplies a bottom-up DACH buyer count. The anchor rewards a top-down EU figure. B1 will use whichever number is higher. A top-down report figure is "inference" and should be L | Fix 8 |
| I9 | Additive compensation remains for founder fit = 1 and regulatory = 1 | The CEO accepted this, so it is not re-argued here. But a row with a score of 1 on these criteria can still total ~78 and the reader would not see it. Showing it costs nothing | Fix 9 (display only) |

## Are K1/K2 testable with the long-list data?
| Test | Data A7/A18 will have | Testable? |
|---|---|---|
| K1 | A7 "who pays"; A18 signer + budget line; TED awards (A11–A14); price lists | **Yes**, once "category" and "in force" are defined (fix 4) |
| K2: closed direction | A14 tender tables (TED, above-threshold, public buyers only) | Only for public buyers above the threshold. Private and below-threshold purchases are invisible, so K2 can **never** be shown closed for rows that have them |
| K2: open direction | Young-vendor customer evidence (MPIRIQ, calliora, voize, caery, MD RLP PoC) | **Yes**, if A18 records one sourced example per route. A18 currently asks for "first-sale route with evidence" but not for a named example of a young vendor (≤5 years old) with a paying customer. Fix 10 |

## Proposed one-line fixes (for CEO approval; `scoring.md` not edited)
Must-fix before B1: 1–6. Should-fix: 7–10.

1. **K2 evidence** (add to K2 "Test"): "A route counts only with a sourced example for this signer type: a company ≤5 years old with a named paying customer, a published direct-award/PoC call open to new companies, or a named channel/prime partner. A route that is only legally possible = **'K2 unproven'**: criteria 3 and 5 are tagged L (R2 cap, R3 'unproven')."
2. **Thresholds and unknowns** (replace the K2 parenthesis): "Direct award: Bavarian state/municipal ≤€100k (Art. 20 BayWiVG); federal ≤€50k; statutory insurers ≤€50k (§ 22 Abs. 2 SVHV); state which applies per buyer, `[UNVERIFIED]` if unclear. Tender rows with thresholds 'unknown' count as closed."
3. **Unit of scoring** (add under Step 1): "K1, K2 and all scores apply to the row's A18 wedge (one signer + one product); if a problem has several wedges, score each as its own row."
4. **K1 category** (add to K1 "Test"): "'Category' = the wedge's signer type pays today for the same job, sourced [A]/[B]; a price list counts only with a named paying customer; a budget line counts only if in force today."
5. **Tiers** (replace the last sentence of R4): "Apply −1 after the R2 cap (floor 1), ranking only K1/K2 survivors. Tier A = top 5 in base **and** top 7 in R4 **and** not 'unproven'; Tier B = top 7 in either run, or 'unproven'; Tier C = rest. Top 5 = tier A, filled from tier B by base total."
6. **M vs L** (replace R1's M/L definitions): "M = an [A]/[B] item about the same signer type in Germany, applied by inference; L = [C] only, snippet only, or inference without such an item. Criterion 5 is M/H only with a sourced comparable (a young company, same buyer type, paid within ≤12 months) or an open accessible procurement. Criterion 4 is M (source: `founder-brief.md`) unless the CEO has answered the founder-access question (H). No evidence at all = score 2, tag L."
7. **R3 test** (add to R3): "The test must need no outward action (desk research or the CEO's own knowledge); a test that needs buyer contact goes to 'Open questions' for CEO approval, and the row stays 'unproven'."
8. **Market** (add to criterion 2 "5 ="): "4–5 only from bottom-up buyer count × price (A18); a top-down report figure alone = L."
9. **Display** (add to Output): "Mark every score of 1 as a red flag in the tier table."
10. **A18 data** (append to the A18 description; CEO edits the task or approves a new one): "Per first-sale route, one sourced example of a young vendor with a named paying customer in this signer type, or 'none found'."

## Cheapest tests
- **Of the fixes (researcher, ≤1 run, desk only):** score S1, S3, I5 and P3 under the current text and under fixes 1–6. Expected result: P3 is out at K1 under both; S1, S3 and I5 pass K2 under the current text but are "K2 unproven" under fix 1 unless a young-vendor example is found. calliora would supply one for S3; caery/Telekom would support I5 only as a channel. If ranks do not move, the fixes are not needed.
- **Of K2 itself (CEO, 10 minutes, no outreach):** for each A18 signer type, does the CEO know one person who has bought from a company less than 3 years old? This is the same founder-access question as in the first review. It also moves criterion 4 from M to H (fix 6).

## Sources opened in this review
- § 22 SVHV (direct award ≤€50k for social-insurance bodies): https://www.gesetze-im-internet.de/svhv/__22.html [A], accessed 2026-11-07
- Search only, not opened: BAS circular "Vereinfachte Vergabe" of 8 Jan 2026 (https://www.bundesamtsozialesicherung.de/fileadmin/redaktion/Vergabe/20260108_Vereinfachte_Vergabe.pdf). It may change the SVHV practice: `[UNVERIFIED]`.
