# Fact-check: research/shortlist.md (B1)
Date: 2026-11-08 | Verdict: **needs work (minor)** | Sources checked: 24 of 41 listed (all 11 "opened in B1" sources; 13 of 29 carried-over sources, picked from the ones the top 5 rests on)

Scope: only `research/shortlist.md` is new since the last fact-check (`2026-11-08-longlist-scoring-fields-A23-A25.md`). The inputs (`scoring.md`, `longlist-scoring-fields.md`) were reviewed there and not re-opened except where B1 relies on them. No fabrication found: every quote I opened is verbatim. Not judged here: the business idea (red team B2).

**Arithmetic: reproduces in full.** All 10 base totals, all 10 R4 totals, the R2 caps, the tier table, the "if decided the other way" totals in C1 (L07 66/64), C2 (L13 4th, L29 5th), C6 (L07 61), the L01 K2-fallback (63/56), the L03 pain-3 case (56) and the six ceiling figures re-derive from the table and weights (3/2/3/2/2/1/2/2/1; max 90). The top 5 (L01, L07, L06, L03, L13) is the correct base-total order under `scoring.md` as written, and the 59/59 tie does not matter (L29 is 57). Counts: 17 knocked out + 10 survivors = 27 rows; the other 3 of 30 (L10, L19, L30) are merged/excluded in A23. **The top 5 does not change on mechanical grounds.**

## Critical issues (must fix)
None that is a fabrication or a wrong number. One issue could change the top 5 and is turned into a fix task (B4), under rule 14:

1. **L01 K1 is passed on a standard that the same file uses to fail other rows.** K1 (shortlist reading table): "A tender, contract or named purchase by the wedge's signer type **for the same job**" (G2: "Job: opex without an observed purchase = K1 not shown", used to knock out L12, L20, L24, L09). L01's K1 evidence is [e1]-[e4]. I opened all four:
   - pme: "Mehr als 1400 Unternehmen vertrauen auf usere [sic] EAP-Lösungen" and a menu item "Homecare-Eldercare". 1,400 is the **EAP** customer count, not eldercare.
   - heycare: customers "Daimler Truck, Douglas, Vaillant and VW Retail" **"According to the company"**; the platform "provides care solutions for children, elderly relatives and pets" plus mental-health training. This is a bundled EAP; eldercare spend is not isolated. (The same article says "already profitable", which the shortlist does not use.)
   - Aon: an offering page ("Individuelles Pflege-Case Management"), no buyer.
   - AOK PLUS: a free Kasse programme in **Thüringen** ("Projektes der AOK PLUS in Thüringen"), i.e. a substitute, not a purchase.
   None is a dated, named employer purchase of an eldercare service. The shortlist itself lists exactly that as its first open check ("One dated, named employer contract with a price for eldercare") and admits "no observed stand-alone eldercare price", yet the table shows "Pass". K2 rests on the same vendor claim, which the file does flag ("L01 = 63 / 56"), but K1 is not flagged. If K1 is "not shown" (same rule as L12/L20), L01 is out and the top 5 becomes L07, L06, L03, L13, L29, and the Recommendation ("deep-dive L01") changes. Fix: B4.

## Other issues (caveats for the CEO; no new tasks, rule 14)
2. **L26 K1 evidence is outside the file's own date rule and stale.** The reading table requires "dated 2024+". The Clariness × Boehringer Ingelheim release has `datePublished` 2021-11-29 and the Servier release 2022-04-12 (Q1 2022 recruitment start). Both are >3 years old (rule 4). By the file's own reading L26 should be K1 "not shown". Rank 8, no top-5 effect.
3. **L07 market score and ceiling use the wrong buyer base.** The wedge is "private hospital <300 beds". The score uses "1,603 IKs × DKI €40k ≈ €64m" and the ceiling 1,807 × €20-40k. Destatis (opened): 729 of 1,807 hospitals are privately owned, and they are the smaller ones. 729 × €20-40k = €15-29m. `hospital-billing-audits.md` itself computes €25-42m for the whole market. Also the DKI €40k is the median "Sachkosten für **Anschaffung und laufende Kosten**" of an AI solution (DKI PDF, chart: median 40,000, mean 68,147, quartiles 17,500-95,000), not an annual price; the source file already says "whether the stated cost is annual is unclear". The sketch prices "€20-40k/yr". Re-based, market 3→2 gives L07 61, below L06 (62): slots 2 and 3 swap, top 5 unchanged (−2 is not >2).
4. **L06 pain "5 H" breaks R1.** H needs "no counter-source". The 93.1 min/day study (opened via Europe PMC: 9 physicians, one hospital, 216 h) is called a "Counter-measure" to the 3 h/day figure in `pain-professionals.md`, and both measure all documentation, not discharge letters. Tag should be M (no score change; R2/R4 penalise only L). Whether 5 is justified without any online voice (criterion 1 text: "many independent online signals") is a judgement for the red team; the same applies to L07 and L22.
5. **L01 buyer count is legal units.** 18,632 is the Destatis column "250 und mehr" under "Rechtliche Einheiten" (2024; employees 17,289,712 in that class) - verified. Legal units of one group count several times, so independent HR buyers are fewer; the €93-373m ceiling is an upper bound.
6. **L13 K1 and ceiling.** Quotes verified (Ärzteblatt, issue 7/2024, a "Blickwinkel" opinion column; one practice satisfied, one cancelling). But (a) the "half of staff cost" quote gives no price or vendor, so it shows a purchase, not a price; (b) 7/2024 is ~2.7 years old in a fast market; (c) the €9-229/month range is per vendor and the Doctolib €229 is "pro Behandler" incl. VAT, while the ceiling uses €100-200 per practice. Fine as L-grade inference; do not read the ceiling as sourced.
7. **L06 K1 is inconsistent with L08.** L08 is knocked out because discharge-platform buys "used one-off KHZG money (G1)" and `longlist-scoring-fields.md` says "KHZG money has ended". L06 passes on one KHZG-funded tender (Harzklinikum, TED 492877-2025: re-queried, published 2025-07-28, deadline 2025-08-25, only the contract notice under the procedure, 1 notice, no award - reproduces). The tender is a CDSS bundle that needs a German full-implementation reference (`pain-professionals.md`), and the buyer is a public hospital while the wedge says "small private hospital". The file does flag L06 K1 as weak and shows "L06 out, L29 in", so this is disclosed; the inconsistent treatment of KHZG money is not.
8. **L29 K1/K2 evidence is about large firms.** Flinn's named customers (Carl Zeiss, Philips, Paul Hartmann) are large; the wedge is "device SME with 20-250 staff". Quote and $20m verified; founded 2022 verified (tech.eu: "formed earlier this year", 20 Dec 2022). Slot 6; matters only if it enters.
9. **L23 K1/K2 rests on a procedure that was cancelled.** `payer-processing.md` lists MD RLP under "Cancellations (change of need)". The shortlist says "closed 5 Sep 2025, no winner"; it should say cancelled/re-tendered (543912-2025, no award). Rank 7.
10. **Unreproducible numbers.** C1 gives the L05 voice-documentation wedge "64 today, 67 at the sale", but that wedge has no row or scores in the file. Treat as unverifiable.
11. **Table does not meet the "evidence link per cell" output rule** of `scoring.md` for ~half of the cells (Fit, Reg, Achiev., many WTP and Comp cells carry no [eN]). Tags are given; links are not.
12. **Threshold used as price.** L03 (92 × "≤€50k") and L23 (15 × "≤€50k") ceilings multiply the direct-award cap, not an observed fee. Labelled "≤", L-grade; fine, but the €4.6m / €0.75m are caps, not estimates.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| pme: "Homecare-Eldercare"; ">1400 Unternehmen vertrauen auf unsere EAP-Lösungen" [e1] | familienservice.de | Supported (partly) | Site text reads "usere" (typo); 1,400 = EAP customers, "Homecare-Eldercare" is only a menu item |
| heycare Munich, 2022, "elderly relatives", €4m, named customers "according to the company" [e2] | munich-startup.de (18 Mar 2026) | Supported | Founded 2022 as Heynanny; bundle incl. children, pets, mental health; "already profitable" (not used) |
| Aon "betriebliche Pflegelösung" with "Individuelles Pflege-Case Management" [e3] | aon.com | Supported | Offering only |
| AOK PLUS trains in-company Pflegelotsen "for free" [e4] | aok.de | Partially | "Teilnahme ... kostenfrei", but a Thüringen project; geography omitted |
| § 106b SGB XI: monthly TI-Pauschale for TI equipment and running costs of care facilities [e37] | gesetze-im-internet.de | Supported | Amount in force from 30 Jun 2023, renegotiated every 2 years; it reimburses the facility's TI costs, it is not a purchase of onboarding services |
| Practice: "Die Kosten für den VoiceBot entsprechen dabei der Hälfte der ansonsten anfallenden Personalkosten" [e24] | Ärzteblatt 7/2024 | Supported | Opinion column, 2024 |
| Practice cancelling: "konnten im Schnitt zwei" of ten callers | same | Supported | |
| Clariness × BI "multi-year partnership ... Boehringer Ingelheim Pharma & Co" in Germany [e34] | clinicaltrialsarena.com | Supported, **stale** | Published 2021-11-29 |
| Clariness recruits for Servier's German subsidiary, Q1 2022 | clinicaltrialsarena.com | Supported, **stale** | Published 2022-04-12 |
| DORA covers insurers, applies from 17 Jan 2025 (Art. 2(1)(n), Art. 64) | EUR-Lex 32022R2554 | Supported | |
| TED 492877-2025 Harzklinikum, deadline 25 Aug 2025, no award [e14] | TED API | Supported (re-run) | 1 notice under procedure 7e725667-...; published 2025-07-28 |
| 3 % use counselling [e5] | GKV-SV §7a report | Supported | "3 Prozent der Anspruchsberechtigten" |
| 46.9 % "hoch belastet"; 45.2 % cut hours [e6] | WIdO PM | Supported | 46.9 % = of in-work carers; 45.2 % = of **part-time** working carers only (shortlist says "46.9 % of employed carers" correctly; L03 pain text "45 % cut hours" elsewhere is a part-time subset) |
| 18,632 legal units ≥250 staff [e7] | Destatis | Supported | Legal units, not enterprises |
| 1,807 hospitals; 729 private [e17] | Destatis PM 2026 | Supported | Private = 729 (21 % of beds) |
| DKI median €40k AI cost [e10] | DKG/DKI flash survey | Supported | Acquisition **and** running costs; not annual |
| Tiplu MBEG-Assistent "in rund 30 Krankenhäusern" [e13] | tiplu.de | Supported | |
| ~98,000 practices + ~4,900 MVZ [e26] | Hartmannbund | Supported | |
| 10 vendors, €9-229/month [e25] | medizinio.de | Supported | Doctolib €229 per Behandler incl. VAT |
| Doctolib bought aaron.ai [e27] | Ärzteblatt | Not opened | Carried over; checked in earlier reviews |
| Flinn $20m, Hartmann quote [e28] | lisavienna.at (19 Feb 2026) | Supported | Customers named: Zeiss, Philips, Hartmann (large) |
| Flinn formed 2022 [e29] | tech.eu/2022/12/20/n26/ | Supported | URL slug is odd ("n26") but page is the Flinn article |
| 1,480 firms >20 staff [e31] | BVMed | Supported | "1.480 Betrieben mit mehr als 20 Beschäftigten" |
| calliora €5.3m, 2023 [e11] | munich-startup.de | Supported (headline) | Not re-read in full |
| 92 Kassen; ≤€50k direct award, "soll ... wechseln" [e22] | GKV-SV list; § 22 SVHV | Supported | List shows "92 Ergebnisse (Stand: 08.11.2026)" |
| 93.1 min/day [e16] | Europe PMC 38977000 | Supported | 9 physicians, 1 hospital, all documentation |
| Others carried over (e8, e9, e12, e15, e18-e21, e23, e30, e32, e33, e35, e36, e38-e40) | repo files / earlier reviews | Not re-opened | Covered by earlier fact-checks of their source files |

## [UNVERIFIED] items
- MIA = UK Frankfurt winner; Gesundheit von Morgen and Recare founding years; private/municipal hospital purchasing rules. All correctly marked; C1 builds a "what if" (L07 66/64) on the MIA match, labelled as such. OK.
- L11 fees `[UNVERIFIED]`, L18 spend `[UNVERIFIED]`: used to knock rows out, not to rank. OK.
- No `[UNVERIFIED]` item is treated as fact in the ranking.

## Evidence grades
- Tags [A]/[B] on the opened sources are right (statutes, Destatis, TED, GKV-SV = A; vendor pages, press, Ärzteblatt, DKI/BVMed = B).
- Criterion-1 scores of 4-5 rest on [A]/[B] only; no [C] items at all (Reddit blocked, disclosed in "Gaps").
- Stale data: Clariness (2021/2022), UKE (Aug 2024 in the scoring file), Hallesche FEELcare (08/21, correctly used only as a pointer).
- Sizes: no market size rests on [C]; all six ceilings are inference and tagged L.

## Unsourced claims
- L01 sketch slogan ("Pflegefall in 48 h organised") and product design are sketch, not claims. OK.
- "Practices pay ... AI agents are the founder's daily work" (L13): the second half is from `founder-brief.md`, not cited. Minor.

## Fabrication check
No quote, interview or feedback without a URL. All quotes opened (pme, heycare, Ärzteblatt x2, DKI, SVHV) are verbatim except the pme typo "usere" being silently corrected.

## Re-run counts
TED 492877-2025: match (1 notice, no award). GKV-SV Kassen count 92: match. No App Store / CT.gov recipe applies.
