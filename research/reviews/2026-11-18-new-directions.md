# Fact-check: research/new-directions.md (C15, task C17 fact-check half)
Date 2026-11-18 | Verdict: **needs work (minor)** | Sources checked: 29 of 29 cited URLs attempted, 27 read in full (GTAI bot-blocked; Pharmazeutische Zeitung timed out / HTTP 502); § 63a AMG read via the buzer.de mirror because gesetze-im-internet.de reset the connection; PRWeb read via WebFetch (curl 403). Plus TED API re-runs (342013-2026, 374640-2025, occupational-health count) and the repo cross-references (CTIS counts, AOK Hessen, § 393, Art. 18 HKaG).

Scope: only file in `research/` or `ventures/` changed since its latest fact-check (commit 2026-11-18). Business judgement (is direction 1 a good venture, is the spin-out route a career move) is left to the red-team half of C17.

**What holds.** No fabrication. The legal core of direction 1 holds word for word: Art. 37 CTR duty to file a results summary plus a lay summary, in-system alerts, "direct email notifications", per-Member-State monitoring, and the end-2026 ACT EU reporting (EMA letter, 2 Jul 2026). The compliance gap (116 of 234 on time, 20 late, 98 missing, 47 incomplete, >8,400 trials) matches TranspariMED and is correctly flagged as a preprint. EMWA €82.2/h median and 223 respondents, Yseop (Novartis dRx, Eli Lilly, 150 trials, 10,000+ reports), TrialAssure (est. 2009, ~50,000 documents, LINK), EXIST one-pager (4 FTE, business seat, €250k materials, 18 months, Phase II €180k / 75 %, cut-offs 31 Mar / 31 Aug / 30 Nov, Hochschule applies), EFT report (175 applications, >€55m, average >€1m since 2023, Phase II 71/58, 50 % AI), UK Leipzig ≥€2m turnover, ~35 coders, >60,000 inpatient cases, DMRZ 1.30 % + €25, Lisbon wages, € 920 / €13.90 / €14.60 minimum wages, § 63a AMG, 84 % SMEs, EMA 400 substance groups, KfW 1.2× (median 0.6×) and >6 % closure plans, search-fund EBITDA range, DiGA 74/58 and ~€400m, BÄK 1,000 entities, NIS2 6 Dec 2025, drweb €15 / €125, vdek €243m / 1.8m, course caps €75–150, Regensburg €1,450,800 + €549,200: all reproduce. Arithmetic in K3 (72/200, 36/100, 4.5–9.0 %), €243m/1.8m ≈ €135, €13.90 × 40 × 52 / 12 ≈ €2,409, 68–79 % all reproduce.

## Critical issues (must fix)
1. **Direction numbering is inconsistent in the part the CEO reads.** Findings call the Lisbon admin team "direction 4" twice ("(direction 4)"; "Keep direction 4 as the delivery model for direction 1"), but the ranked table and Details number it **3**; direction **4** in the table is pharmacovigilance. Task C16 option (d) says "3 Lisbon admin team". A reader following the recommendation lands on the wrong row. Fix: "direction 3" in both Findings lines.
2. **An `[UNVERIFIED]` item carries the recommendation.** The rule that lay summaries must be in "the official local language or languages" is marked snippet-only `[UNVERIFIED]` (Details §1, Gaps), yet three statements build on it: K5 "German, English and Portuguese cover three CTIS languages"; first idea (b) "lay-summary translation … for CROs"; and the Recommendation "Keep direction 4 [3] as the delivery model for direction 1 (multilingual lay summaries: DE/PT/EN)". Art. 26 CTR leaves dossier language to each Member State concerned; I did not find the lay-summary language rule in an opened primary source either. Fix: cite the primary rule (CTR Annex V / Art. 37(4), the Commission CTR Q&A, or the EudraLex Vol. 10 lay-summary guidance) or rewrite these three statements as conditional on it.
3. **TUM "115 start-ups" is cited to a page that does not contain it, and is overstated as "spun out".** The cited URL (`…/erstmals-mehr-als-100-neue-start-ups-in-einem-jahr`, 28 Mar 2025) says **103 start-ups in 2024**. The 115 figure is in the TUM press release of 26 Jun 2026 ([TUM](https://www.tum.de/aktuelles/alle-meldungen/pressemitteilungen/details/presidential-award-fuer-raumfahrt-start-up)): "Forschende, Studierende sowie Absolventinnen und Absolventen … 115 Start-ups gegründet". These are mostly student/alumni start-ups, not research spin-outs; a search result (Redstone index, snippet only, not opened) gives 38 researcher-founded TUM start-ups in 2025. Findings: "TUM alone spun out **115** start-ups in 2025" → fix the URL and the wording ("115 start-ups by researchers, students and alumni").
4. **A quoted phrase is not in its source.** Details §1: Peer AI "automates protocols, CSRs and \"plain language summaries\"" cited to eeNews Europe. The article mentions CSRs and protocols, not plain-language or lay summaries (grep: zero hits). Peer AI's site did not return text to check. Fix: drop the quote or cite a page that says it. Note the same article says Peer AI's customers include "top 20 pharmaceutical firms and emerging biotechs": relevant to the file's inference that small biotechs are the open segment.
5. **EXIST arithmetic is invalid and a key number from the same report is missing.** Details §2: "*My math:* >€55m / >€1m ≈ fewer than 55 Phase I projects a year". Dividing two lower bounds gives no upper bound (e.g. €60m / €1.05m = 57). The same report states the cumulative approval rate: **634 of 2,280 applications, "Förderquote (gesamt) 27,8 %"** ([EFT report](https://exist.de/wp-content/uploads/2026/04/EFT_Monitoringbericht_2025_Nr.3.pdf), dashboard "Förderstatistik"). The inference "Phase I pays the CEO's salary from Sep 2027 if he joins a team" should carry that roughly one-in-four odds. Fix: delete the "fewer than 55" sentence or take the 2025 approval count from the report; add the 27.8 % rate.

## Minor issues (fix in the same pass if cheap)
- **G-BA AbD count mismatch** (Details §10): file "3 laufend, 3 eingeleitet, 11 eingestellt". The page's filter menu contains each label once; excluding it, the 25 listed procedures show **2 laufend, 2 eingeleitet, 10 eingestellt**, plus 5 "Datenerhebung wird nicht durchgeführt" and 1 "ruhend". The direction-10 verdict is unchanged; Findings "~3 running AbD data collections" → "2".
- **"Big incumbents win every tender"** (Findings, direction 8) is stronger than the evidence. The Details say "and a few local practices"; my TED pull (CPV 85147000, DEU, award notices since 2024: 125 notices, incl. company fitness) shows winners such as Medical Airport Service, Medservio, Arbeitsschutz Borch, Praeamed and "Dres. Dietlmeier & Hohmann GbR" (226625-2025, "Betriebsarzt München"). Write "mostly incumbents". Verdict (drop: needs physicians) unchanged.
- **The "34 award notices" count cannot be reproduced**: the query is not recorded. CPV 85147000 gives 125; CPV 85147000 + FT "betriebsärztliche" gives 36. Record the query string (sources-map recipe).
- **Lisbon wage comparison leaves out the bonus.** The ad pays "+ bonus up to 1.267,00€ gross per quarter" (≈ €422/month) and the €1,633.89 option includes free accommodation. With the full bonus the no-accommodation option is ≈ €2,328 = 97 % of the German minimum, not 79 %. This strengthens the file's own reading ("cost gap alone is modest").
- **UK Leipzig bar is higher than stated**: besides ≥€2m turnover, the notice asks for references from ≥3 maximum-care or university hospitals over ≥24 months, ISO 9001 and ≥2 employed physicians with ≥5 years of coding experience (TED 342013-2026 `selection-criterion-description-lot`).
- **DiGA "shrinking pool of buyers"**: the directory shrank (74 admitted, 58 left), but the same report says use rose 63 % on the previous year. Write "shrinking list of DiGA", not "shrinking pool of buyers".
- **Unsourced in this file** (no URL, no `[UNVERIFIED]`): PV incumbents PharmaLex, Freyr, ProductLife and "biologit (directory listing)"; "GTAI (federal, free)" as a market-entry substitute; NIS2 "crowded (ISMS tools, IT service firms)"; "Kassen run free online courses" (direction 9 K4); "IQVIA-type CROs"; Max-Planck-Innovation co-founder role (snippet, labelled but graded [B] without a URL). None is critical-path; add URLs or `[UNVERIFIED]`.
- **Stale data**: EMWA 2023 (flagged), EMA 2015 (flagged), Yseop Dec 2023 and TrialAssure Oct 2023 (3 years, not flagged; vendor claims only).

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| Art. 37 CTR duty: results summary + lay summary; alerts, email notifications, per-MS monitoring; end-2026 ACT EU reports | EMA letter 2 Jul 2026 | supported | Quotes verbatim |
| 116/234 on time, 20 late, 98 missing, 47 incomplete, >8,400 trials; no sponsor split | TranspariMED | supported | Preprint, [B] fair; no sponsor-type split confirmed |
| €82.2/h median, 223 respondents (2023) | EMWA | supported | 3 years old (flagged) |
| Peer AI $12.1m, San Francisco; "plain language summaries" | eeNews Europe 7 Oct 2025 | partially | Funding yes; quote not in article (issue 4) |
| Yseop: Novartis (dRx), Eli Lilly, 150 trials, 10,000+ reports | Yseop 5 Dec 2023 | supported | |
| TrialAssure est. 2009, ~50,000 PLS, LINK | PRWeb 18 Oct 2023 | supported | curl 403; read via WebFetch |
| EFT: ≤4 FTE incl. business seat; €250k; 18 months; Phase II €180k/75 %; cut-offs; AI model project | BMWE one-pager | supported | |
| 175 applications, >€55m, >€1m avg since 2023; Phase II 58 approvals, 50 % AI; biotech/software/medtech lead | EFT report 2025 | supported | 27.8 % approval rate omitted; "<55 projects" maths invalid (issue 5) |
| TUM 115 start-ups 2025 | TUM 28 Mar 2025 page | not supported | Page says 103 (2024); 115 is in the 26 Jun 2026 release, incl. students/alumni (issue 3) |
| KIARA (Fraunhofer HHI) seeks commercial co-founder | LMU IEC | supported | |
| DMRZ "ab 1,30 %", €25/month | DMRZ brochure | supported | €25 applies to Heil-/Hilfsmittel, midwives, rehab sport, transport |
| Lisbon €1,633.89–1,905.92 gross, expired | Blu Selection | supported | Bonus up to €1,267/quarter omitted from the % comparison |
| PT minimum wage €920 (DL 139/2025) | APCMC | supported | Page opened fine |
| DE minimum wage €13.90 (2026), €14.60 (2027) | Bundesregierung | supported | |
| UK Leipzig external coding revision, ≥€2m turnover, ~35 coders, >60,000 inpatient cases | TED 342013-2026 | supported | More bars than stated (references, ISO 9001, physicians) |
| Stufenplanbeauftragter duty; "Andere Personen … nicht ausüben" | § 63a AMG | supported | Read via buzer.de mirror |
| >650 pharma companies | GTAI | unverifiable | Radware bot block |
| 84 % SMEs | Apotheke Adhoc | supported | |
| EMA screens 400 substance groups | EMA 2015 news | supported | Old, flagged |
| KfW asking price 1.2× (median 0.6×); >6 % closure plans to end-2026 | KfW Fokus 526 | supported | |
| 6,444 listings on nexxt-change | nexxt-change | match | 6,440 today (live count) |
| Search-fund EBITDA €1–5m; "Handvoll" investors | Unternehmeredition | supported | |
| 74 DiGA admitted, 58 left end-2025, ~€400m total | GKV-SV DiGA report 2025 | supported | "Shrinking pool of buyers" overstated; use +63 % |
| 1,000 extra health entities (800 MVZ, 200 BAG) | BÄK statement 4 Jul 2025 | supported | On the draft bill (stated) |
| NIS2UmsuCG in force 6 Dec 2025 | usd.de | supported | |
| Betriebsarzt from €15/employee, €125/h, as of 3 Oct 2026 | drweb | supported | |
| 34 occupational-health award notices; Regensburg €1,450,800 + €549,200 (ias, B·A·D) | TED API | partially | Regensburg reproduces; 34 not reproducible (no query); "every tender" overstated |
| €243m (2025), >1.8m participants | vdek | supported | |
| 80–100 %, capped €75–150 per course | krankenkasseninfo | supported | |
| AbD: 3 laufend, 3 eingeleitet, 11 eingestellt | G-BA | mismatch | 2 / 2 / 10 excluding the filter menu |
| FDZ: 82 institutions, 53 applications | Pharmazeutische Zeitung | unverifiable | Timeout and HTTP 502 today |
| CTIS 1,356 commercial + 876 non-commercial (2025); DE 668 / 109 | repo `research/trial-recruitment-de.md` | supported | Matches repo; recipe reproduced in run 4 |

## [UNVERIFIED] items
| Item | Treated as fact or built on? |
|---|---|
| Per-trial package price €5–10k | Labelled assumption; drives K3 and the "Top 1" rank, and C16 repeats it as "assumed". Acceptable as labelled; the red team should judge the ranking |
| Lay summaries "in the official local language(s)" | **Built on** (issue 2): K5 language edge, idea (b), direction-3 delivery model |
| EudraCT 23.6 % vs 77.2 % split | Not built on |
| Citeline $3,000–3,500 patient panel | Not built on |
| Per-seat €40k (direction 3) | Labelled assumption in K3; not built on beyond that |
| PV €2k a month; "~670" pharma firms (snippet) → 563 SMEs | Labelled; minor |
| EHDS secondary use from 26 Mar 2029 | Drives the "Watch (EHDS 2029)" verdict; minor |
| DACH market-entry consultants paid | Labelled; direction dropped |
