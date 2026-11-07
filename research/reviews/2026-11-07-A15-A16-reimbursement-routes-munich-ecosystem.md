# Fact-check: research/reimbursement-routes.md (A15 + A16 changes) and research/munich-ecosystem.md (A16 changes)
Date: 2026-11-07 (run 5) | Verdict: **pass with minor fixes** (both files) | Sources checked: 27 of 27 sources that carry the new or changed claims (all re-downloaded and text-searched with curl and pdftotext); unchanged parts of both files and the one-line sync in `research/trends.md` were not re-checked (they were covered in the run-3 reviews).

Scope: diff of the two files since the run-3 review (commit 674ff92), i.e. commits fbc18d0 (A15) and c7955cd (A16). `research/trends.md` changed by one line (uptake sync); it matches the reimbursement file. No other research file is new since its last fact-check (`scoring.md`, `hospital-billing-audits.md`, `payer-processing.md`, `trial-recruitment-de.md`, pain files all unchanged since their reviews).

## Critical issues (must fix)
None. No invented figures, quotes or sources. Every number I searched is on the cited page. No [UNVERIFIED] item is used as fact.

## Minor fixes (for the next revision, not blockers for B1)
1. **SCE "not rolling" is stronger than the page.** `munich-ecosystem.md` (Programs bullet and table row) says intake is "twice a year, not rolling". The page does show "Sommer-Batch (März - Juli) und Winter-Batch (September - Januar)" and "Deadline: 2. August 2026". But the same page also says "**Dauerhaft** für die SCE Incubation bewerben." That sentence can be read as continuous applications. "Next intake is the summer batch from March 2027" is the researcher's inference, not on the page. Fix: say "batches Mar–Jul / Sep–Jan; page shows a passed deadline of 2 Aug 2026 but also 'Dauerhaft … bewerben'; whether applications are open now is unclear; ask SCE". The recommendation "SCE (summer batch from March 2027)" in the next-steps line rests on this reading.
2. **FINSOZ example is stretched.** `reimbursement-routes.md` §4b: "FINSOZ puts the corridor for a 100-resident home at ~5.6 FTE". The statement says the § 113c limits allow refinancing "40 % dieses Mehrbedarfs, das wären 5,6 VZÄ" of the 14-FTE extra need, and then (its "sehr konservative Rechnung") assumes about half of that is unfilled, i.e. 2.8 FTE, and at its proposed 50 % share 1.4 FTE. So 5.6 FTE is the cap on refinanceable extra posts, not the minimum-to-maximum corridor of § 113e Abs. 2 as the file defines it. The €16–19k per 100-resident home and €128–151m national figures rest on 10 % × 5.6. They are labelled "inference" and "one industry example", which is honest, but the attribution "FINSOZ puts the corridor at" should be "FINSOZ computes a 5.6-FTE refinanceable cap; the 10 % is applied by me". Direction of the error: the file may overstate (FINSOZ's own conservative case is 2.8 FTE before any percentage).
3. **Facility count inconsistency in the uptake math.** The "37 % of pool" uses 32,054 facilities (Destatis 2023). DAK says it processes 48 % of facilities = about 17,500, which implies about 36,500 facilities nationwide. The two denominators differ by about 14 %. The 37 % vs DAK "knapp 40 %" agreement is therefore partly coincidental. Say so in one line, or use DAK's implied base as a sensitivity.
4. **PNOG timetable.** "2nd/3rd reading 11 Dec 2026, in force 1 Jan 2027" is from the AOK tracker [B] and is correct as quoted (also "Anhörung 11. oder 25. November", "Bundesrat 18. Dezember"). Fine, but the file calls the bill "Drucksache 21/8869" and the Bundestag page lists it "Status: 02.11.2026"; consistent. No fix; noted because the CEO should treat all PNOG items as bill status.
5. **Länder co-funding omits the catch-up rule.** File: "the €2.0bn total holds only if every Land takes part". The draft text (§ 11 Abs. 4, p. 26–27) also allows a Land that misses the deadline to catch up by 1 Jan of the next year (money then flows for both years). Add half a sentence.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| § 8 Abs. 8 payouts 2019–2024: 5,187,883 / 26,639,280 / 31,641,717 / 27,590,391 / 28,072,975 / 24,164,292 € | BAS two PDFs | supported | exact, row "Förderung digitaler Anwendungen in Pflegeeinrichtungen § 8 Abs. 8 SGB XI"; sum 143,296,538 € is correct (my recomputation) |
| DAK: 48 % of facilities, ~21,000 applications (+28 %), 93 % approved, ~11,300 of ~17,500, €81.2m "knapp 40 Prozent", "+ fast zwölf Prozent", "Abrufquote … eher niedrig", other facilities "überwiegend die AOK" | DAK press release 1 Sep 2025 | supported | all quotes verbatim |
| 37 % and 65 % and €7,200 | own math | arithmetic correct | see minor fix 3 on the denominator |
| vdek Berlin ~30 %, Brandenburg ~20 % = full amount | vdek | not re-opened this run | checked in run 3 (A10/A16 text unchanged) |
| 1st reading 5 Nov 2026, referred to committees, Gesundheitsausschuss leads, coalition announces changes for family carers | Bundestag text archive | supported | the page also names the document 21/8869 (status 02.11.2026) |
| 2nd/3rd reading 11 Dec 2026, in force 1 Jan 2027 | AOK tracker, updated 27.10.2026 | supported | |
| § 113e: only vollstationäre; 1 Jan 2028–31 Dec 2032; up to 10 %; Pflegesatzvereinbarung; § 82 Abs. 2 not applicable; min. wage cap; catalogue 30 Sep 2027, quarterly; evaluation 30 Jun 2030 / 30 Jun 2033; first GKV-SV report 1 Jul 2028; Abs. 6 quality/safety | Cabinet draft p. 59–60 | supported | verbatim in the law text; 1,560 h and "keine Sozialversicherungsbeiträge" are in the reasoning (p. 232 area), not in the law text. The file says the cap is "× 1,560 h"; correct only as the reasoning's assumption |
| "text identical in bill 21/8869" | Bundestag PDF | supported (not diffed line by line) | § 113e appears 11 times in the bill; uptake of the same wording not compared character by character |
| Minimum wages €16.52 / 17.80 / 21.03 from 1 Jul 2026, valid to 30 Sep 2028; €16.95 / 18.26 / 21.58 from 1 Jul 2027 | Bundesregierung; BMG PM 25.11.25 | supported | |
| FINSOZ: 14 FTE extra need, 40 % = 5.6, asks 50 % | FINSOZ statement | partially | see minor fix 2 |
| DBfK: 25.46 FTE, ~2.55 FTE max scenario; "zu streichen oder grundlegend zu überarbeiten" | DBfK PDFs | supported | 0.884 / 1.663 split not re-derived |
| GKV-SV: "nicht pauschal als Ersatz", ~one third have a staffing agreement by qualification group (report § 113c Abs. 8), replace by catalogue/method until 30 Sep 2031, "Wirtschaftlichkeitsnachweis mit bezifferbaren Effizienzgewinnen", § 115 Abs. 3 | GKV-SV statement 10 Jun 2026 | supported | the file correctly says the underlying report was not opened |
| ver.di: "in dreifacher Hinsicht" | ver.di statement | supported | |
| 800,000 in full residential care, Dec 2023 | Destatis via Presseportal | supported | "Ein Siebtel … (14 % beziehungsweise 800 000)" |
| § 40a Abs. 1a exclusions incl. "ausschließlich auf Auskunft oder Beratung …" | gesetze-im-internet | supported | the inference about hybrid carer-relief apps is flagged as inference |
| PNOG: Länder "sollen" co-fund €400m, Königsteiner key, 30 Jun 2027 / 30 Nov, 2024–26 average | Cabinet draft p. 26–27 | supported | see minor fix 5 |
| PNOG: bill reasoning "ambulanten und teilstationären", law text "ambulanter und stationärer" | bill 21/8869 | supported | both strings found |
| Old grant narrows (AI training, GKV-SV guidelines by 31 Mar 2027) | Cabinet draft | supported | |
| GKV-SV position paper 27 Aug 2026: grant every three years, no uptake figure | PDF | not individually re-checked | only opened to confirm it downloads; the "no uptake figure" claim is an absence claim |
| FLÜGGE 2026/1: up to 4 projects, ~€500,000, sketches 2 Nov–18 Dec 2026 via Hochschule (Ausschlussfrist), panel 18 Mar 2027, application 28 Apr 2027, start from 1 Jul 2027, €2,500/month, must belong to the Hochschule | call PDF 2026 | supported | exact |
| SCE: Sommer/Winter-Batch, "mindestens 10 Stunden pro Woche", "Deadline: 2. August 2026", "über 30.000 €" free | sce.de | partially | see minor fix 1 |
| UnternehmerTUM Incubator: Berufstätige in target group, kostenfrei, "wir nehmen keine Unternehmensanteile", start "2 Mal pro Jahr (März und September)" | unternehmertum.de | supported | resolves the run-3 finding |
| EY: Bayern > €1.1bn "(minus 46 Prozent)", rank 3; 93 rounds (+21 %), rank 2; Health rank 4/5 > €450m | EY Startup-Barometer Jul 2026 | supported | |
| EIC 2027 batching dates 20/01, 17/03, 01/09, 04/11 (5pm Brussels); Open budget €428m | EIC page | supported | |
| KHZG €4.3bn "bis zu" | BMG page | not re-opened | verified in run 3 |

## [UNVERIFIED] items
- `reimbursement-routes.md`: 4 occurrences (prevention-course subsidy amounts per insurer; PKV/Beihilfe reimbursement of DiGA; one table cell; the section heading). None is used as a premise later in the text. The KHZG €4.3bn item is now resolved (matches my run-3 finding).
- `munich-ecosystem.md`: 5 occurrences, unchanged by A16 apart from the removed FLÜGGE caveat; not re-examined here beyond confirming no A16 text builds on them.
- Gaps the researcher states honestly and I confirm are open: § 113c Abs. 8 GKV-SV report not opened; no AOK or national facility count; BAS 2025 figures; Bundesrat Drucksache; no catalogue method yet published.

## Unsourced claims
None found among the new text. Paragraphs marked "My math" or "Inference" carry their inputs with URLs.

## Evidence grades
- A15 table of BAS payouts [A]: correct (official administrative statistics).
- DAK, vdek, DBfK, ver.di, FINSOZ, GKV-SV positions are [B] interest-group documents: correctly graded [B]. The § 113e text from the cabinet draft/bill is [A] as a legal text, but it is a draft: the file says so repeatedly.
- National § 113e sizing (€128–151m, €43–50m) rests on one [B] industry example plus inference; the file states this. Nothing here should be copied into scoring as a market size without that caveat (the red team may want to know: the "one third" factor comes from a payer-side statement whose source report was not opened).
- Data age: all new sources are 2024–2026; vdek Hamburg 2021 figure is flagged in the file as older than 3 years.

## Fabrication check
No quotes, interviews or feedback without a URL. All verbatim German quotes I searched were found on the cited page.

## Re-run counts
No recipe applies to these two files (no App Store, ClinicalTrials.gov or TED counts). Arithmetic re-done: BAS sum, 143.3/384.6 = 37.3 %, 11,300/17,500 = 64.6 %, 1,560 × 18.26 = 28,486, 1,560 × 21.58 = 33,665, 0.56 × 28,486–33,665 = 15,952–18,852: all match the file.
