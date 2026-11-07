# Fact-check: research/hospital-billing-audits.md (A11)
Date: 2026-11-07 | Verdict: pass (minor fixes) | Sources checked: 28 of 45 listed (all numeric critical-path sources re-run; trade press and ~12 vendor/law pages not opened)

Method: downloaded the three GKV-SV annual XLSX files and the Q2 2026 XLSX and re-computed the tables and the 2027 simulation; re-read DKI, MD "Zahlen Daten Fakten 2024", BStabG text, Tiplu/LOGEX/calliora pages, TED notices.

## Critical issues (must fix)
None. All key numbers reproduce.

## Issues to fix (non-critical)
1. **Two different "audit counts" are used without explanation.** §1 table: 1,192,500 MD reports in 2024 (GKV-SV). §1 MD-capacity bullet: "1,313,000 hospital billing audits in 2024" (MD Zahlen Daten Fakten). `payer-processing.md` (A12) uses MD Bund's 1,232,119 § 275c audits in 2025 against GKV-SV's 1,138,534 reports in 2025. These are different counting units. Add one sentence saying so, otherwise the "4× cap vs. capacity" inference mixes bases.
2. **Stale capacity figure.** "MD capacity: 12,480 staff ... 2,135 physician FTE ... as of 31 Dec 2023" is used in the Findings inference ("MD's capacity (2,135 physician FTE) is the real ceiling"). A12 already reads the 31 Dec 2025 data (12,677 people, 2,148.3 physician FTE, 474.8 coding FTE). Update to avoid two figures for the same ceiling (changes nothing material).
3. **"Hospitals ... most plan to buy AI" overreaches.** DKI: 9 % use AI, 51 % plan "eine Nutzung", 40 % neither. "Nutzung" is not purchase. The total (60 %) is plausible, but "plan to buy" is not what the survey asks.
4. **DKI AI-cost quartiles contradict inside the source.** DKI prose says "von 40.000 € (unteres Quartil) bis 95.000 € (oberes Quartil)"; its table says median 40,000, lower quartile 17,500. The file quotes the table ("quartiles €17,500–95,000"), which is the better reading; add a note. The rough market ceiling in §6 (1,038 × 60 % × €40k–68k) is the researcher's own arithmetic on a self-estimate and the file says "whether the stated cost is annual is unclear". Keep it out of any TAM line.
5. **"Penalties flow back to insurers" / "~€1.6bn".** €183,094,800 is the penalty column (457,737 invoices); the file adds it to reductions. Correct as arithmetic; but the Finding title "~€1.6bn flows back" sums reductions that are the hospital's loss and penalties that go to insurers. Label it "revenue at risk for hospitals", which is how §6 uses it.
6. **A11's correction of A4 is right**: the KHVVG draft sample-audit plan is in the opened vdek release; "Stichproben" text confirmed.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 2025 national: 1,138,534 reports; 582,044 not reduced; 556,490 reduced (48.9 %); avg €2,219.51; penalties €183,094,800 | GKV-SV 2025 XLSX (re-opened) | **supported, exact** | |
| 2024: 1,192,500 / 620,270 / 572,230 / €2,090.00; 2023: 1,262,013 / 651,920 / 610,093 / €1,971.77 | GKV-SV XLSX | **supported, exact** | |
| Pre-audit dialogue 331,543 / 131,458 / €1,251.83 (2025); 348,132 / 148,481 / €996.94; 382,785 / 161,501 / €918.62 | XLSX | supported, exact | |
| Erörterungen 126,655 (11 %), 99,871 (9 %), 72,828 (6 %) | XLSX | supported, exact | |
| Audit reasons 2025 (414,987 / 890,365 / 523,868 / 61,711 / 25,423; 550,055 multi-reason audits) | XLSX | supported, exact | |
| 2024 penalty columns look inconsistent (806,858) | XLSX | supported | good catch |
| €1.24bn + €0.16bn + €0.18bn ≈ €1.58bn | recomputed | supported | |
| Q2 2026: 1,603 IKs; 1,100 at 40 %, 231 at 20 %, 193 at 5 %, 79 without result; 532 below 50 %; 3,497,255 invoices; max auditable Q4 441,834 | Q2 2026 XLSX (re-run) | **supported** | I get 441,833 (rounding) |
| 2027 tiers (≥80 / 65–80 / <65 → 5 / 20 / 40 %), €500 penalty, fee 300 → 500 €, in force 1 Jan 2027, promulgated 29 Jul 2026 | buzer BStabG Art. 1 no. 66, Art. 8 | supported | "No cap <50 %" and "today <20 %" not individually re-read |
| Draft: 5/15/25 %; "Minderausgaben von rund 1,6 Milliarden Euro pro Jahr" from 2027 | BT-Drs. 21/6130 | supported (quote); page "p. 141" not checked | |
| DKI: 306 of 1,038; 3.9 / 2.5 FTE; €236,016 / €150,000; ~4,000 FTE; ~€245m; 98 %; 53 %; 2.3 FTE / €178,128; 9 % / 51 % / 40 %; AI cost mean €68,147, median €40,000 | DKI flash survey | supported | see issues 3 and 4 |
| Tiplu: "knapp 7 von 10 Kliniken ... mindestens 40 %"; MBEG-Assistent "rund 30 Krankenhäusern"; Kodieragent for 2027; LOGEX sole owner (8 Jul 2026); >130 hospitals in ML network; ~400 LOGEX customers in DE | tiplu.de | supported | |
| calliora: $6m pre-seed, BHI + redalpine, Munich, founded 2023, double-digit hospitals, five states, "not independently verified" | Trending Topics (6 Oct 2026) | supported | article itself says figures not independently verified: add to the file |
| ID: ">1.400 Einrichtungen" | job ad PDF | supported | |
| MD ZDF 2024: 12,480 staff / 11,020 FTE; 2,513 / 2,135 physicians; 1,313,000 audits; 14,372,000 GKV hospital cases; 50.6 % not correct | MD Zahlen Daten Fakten 2024 | supported | staff is as of 31 Dec 2023 (stated) |
| MD Niedersachsen 383478-2026: DRG external audits, selection on turnover + references | TED | supported (criteria text); "20,000 orders / 4 months / 4 × €500k" not re-read | |
| TED awards: Charité framework → Health Data Exchange (352020-2025, value withheld); UK Frankfurt 557531-2024 Dr. Baller 4 bids; 402898-2024 "Medical AI Analytics & Information GmbH" €181,800, 5 bids | TED | supported | €360,000 for the Frankfurt framework not in the fields I queried |
| GKV-SV deputy CEO "eine Milliarde Euro" | GKV-SV press release | supported | |
| vdek: KHVVG replacing targeted checks with "wahllose Stichproben" | vdek release | supported | |
| MD Bund / DKG / BWKG / Ärzteblatt / medi-learn quotes, Dedalus, Solventum, Parallel, Recare, Sqior | — | not opened this run | Solventum flagged `[UNVERIFIED]` in the file |

## [UNVERIFIED] items
- Listed: Solventum customer count (snippet), MIA ↔ Medical AI Analytics link, 1 % tier passage, joint GKV-SV/DKG report. None feeds a conclusion. Good.

## Other checks
- Grades: GKV-SV statutory statistics [A]; DKI, vendors, trade press [B]; medi-learn [C] (3 threads, labelled weak). Correct.
- Stale: MD capacity (2023), ID undated profile; flagged. Customer counts of Tiplu/calliora/ID are vendor claims, stated.
- Re-run counts: GKV-SV and Q2 2026 simulation **match**.
