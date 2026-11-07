# Fact-check: research/scoring.md (v3, A20) and the A22 changes to longlist.md, pain-industry.md, pain-professionals.md, payer-processing.md
Date: 2026-11-07 | Verdict: **pass with minor fixes** (no fabrication; all legal thresholds and quotes reproduce; one table/math gap, three overstated inferences) | Sources checked: 19 of 19 scoring.md URLs (all opened; PDFs read as text), plus 7 TED notices via API and 2 DTVP links for A22. Version checked: origin/main at 657aa9a.

Scope: `scoring.md` changed in A20 (8392f82) after its last fact-check (2026-11-07-scoring.md covered v2 K1/K2). The four A22 files changed after the A21 re-check. Other research files are unchanged since their last review. `longlist.md` on origin/main only (A18 edits in progress not checked).

## Critical issues (must fix)
None.

## Issues (should fix before B1 uses the calibration)
1. **L03 row cannot be reproduced from the table (scoring.md, "Scores" table).** The L03 pain cell holds the note "v2: out at K1" instead of a score, but the math line (`12+4+9+8+6+5+6+4+5 = 59`) uses pain = 4 (12 points). The pain score and its H/M/L tag are missing. Also check: the rest of the row is 8 scores for 9 columns plus the note, so the row looks shifted. Add "4 M/H" (with evidence) to the pain cell. All other rows reproduce (L06 78/70/63, L07 75/67/62, L21 70/70/68, L03 59/52 recomputed: match, given pain = 4).
2. **L03 K1 "Pass (new)" is only partly sourced.** K1 requires that the signer type "pays today for the same job, sourced". What is supported: § 45 SGB XI text ("haben ... unentgeltlich Schulungskurse durchzuführen", "sollen auch digitale Pflegekurse anbieten", Abs. 2 "geeignete andere Einrichtungen mit der Durchführung beauftragen") [A]. Mobil Krankenkasse press release of 07.05.2026 confirms a "Kooperation" with Gesundheit von Morgen GmbH (PflegeBetreuer) and that the courses are "kostenfrei" for insured people. Neither it nor pflege.de ("Kostenfrei dank Übernahme durch Ihre Pflegekasse", advertising copy) says that a Kasse pays the vendor, or how much. So "a Kasse commissions third parties" is supported; "a Kasse pays for this job" is an inference. The file already notes "the release does not state a fee" in the K2 column; K1 should say the same.
3. **L21 K2 "Pass, weakly (channel clause)" overstates the Telekom source.** The Telekom release (29.09.2026) says only that TechBoost gives young firms "Zugang zu Vertriebs- und Partnernetzwerken" and that Telekom and caery will jointly "die Digitalisierung ... vorantreiben". It names no insurer, no sale and no resale agreement. Fix 1 requires "a named channel/prime partner" with a sourced example for this signer type; a programme description is not an example of the route in use. By the file's own rule ("only legally possible = K2 unproven") this is closer to "unproven". The file does hedge ("weakly", "no caery customer is named"), so this is a labelling issue, not a misquote. Same for the § 97a Abs. 5 GWB point: the BAS circular confirms the clause ("Interessen kleiner und mittlerer Unternehmen bei der Vergabe von Unteraufträgen besonders zu berücksichtigen") but says buyers *can* oblige contractors; no use shown.
4. **UKL-GPT does not show discharge-letter work (L06 K2 column).** The Ärzteblatt article (9 Mar 2026) describes document search over ~8,700 internal documents plus an assistant for "E-Mails, Berichten oder Zusammenfassungen"; planned extensions are anamnesis support and applications. "Arztbrief" does not appear. It is a counter-signal for in-house LLMs generally, not for discharge letters. UKE "Argo" does support discharge letters (UKE subsidiary IDM, 22 Aug 2024): supported.
5. **Direct-award table, insurers row: "before: €15,000 under a temporary rule" is narrower than written.** The BAS circular of 7 Jan 2026 is addressed to the *bundesunmittelbare* Sozialversicherungsträger (federal-level bodies) and concerns the UVgO derogation (€15,000, BAnz 29 Dec 2025). The table applies it to "all social-insurance bodies". The new €50,000 in § 22 Abs. 2 SVHV itself applies to all SVHV addressees (§ 78 SGB IV: all Sozialversicherungsträger except the BA): supported. Reword "before" to "for federal-level bodies".
6. **L06 K2 builds on an [UNVERIFIED] item.** "Bavarian university hospitals are outside BayHO purchasing rules (table above), so a pilot is legally possible". Art. 5 Abs. 1 BayUniKlinG quote is exact ("... finden mit Ausnahme der Art. 88 bis 104 und 111 keine Anwendung") [A]. But the table row says the applicable below-threshold limit is `[UNVERIFIED]`, so "legally possible" is not established; the hospitals' own purchasing rules were not found. Rephrase as "possible, rules unverified".
7. **voize facts have no source in the repo.** "voize (founded 2020, named customer BruderhausDiakonie, A18 notes)" points to `tasks.json` notes of A18, not to a URL; `longlist.md` has no founding year or customer name for voize (only "1,100 facilities", "$50m"). The quote is used to decide the "≤5 years" question for L05. Needs a URL in the research file before it is relied on.
8. **EU threshold €216,000 is cited to a review, "not re-opened".** Correct: IHK Hannover (cited in `payer-processing.md` line 96) and a web search I ran (Cosinex, Berlin Vergabeservice, Sonntag & Partner snippets) give €216,000 for sub-central supplies/services in 2026-27 [B]. Cite the IHK page directly. Note the federal supreme authorities' limit is €140,000, not €216,000 (snippet only; not relevant to the hospital row).

## Source check (scoring.md)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| Direct award ≤ €100,000 (Bavarian state and municipal), text valid from 1 May 2026 | gesetze-bayern.de BayWiVG Art. 20 | supported | Quote matches; also Abs. 4 extension to Art. 105 Abs. 2 BayHO entities, Abs. 3 no splitting |
| Art. 105 BayHO state-supervised legal persons | gesetze-bayern.de BayHO-105 | supported | Text valid from 1 Aug 2025 |
| Six university hospitals as Anstalten (Art. 1); Art. 5 Abs. 1 BayHO not applicable except Art. 88-104, 111 | gesetze-bayern.de BayUniKlinG | supported | Art. 1 lists Augsburg, Erlangen, LMU, ... ; Art. 5 Abs. 1 wording matches |
| § 22 Abs. 2 SVHV: ≤ €50,000, "Der Auftraggeber soll zwischen den beauftragten Unternehmen wechseln" | gesetze-im-internet SVHV § 22 | supported | Current text |
| SVHV last changed by Art. 14 of the law of 12 May 2026 (BGBl. 2026 I Nr. 137); issued under § 78 SGB IV | SVHV page | supported | Eingangsformel "Auf Grund des § 78 des Vierten Buches" |
| § 78 SGB IV covers all social-insurance bodies except the BA | gesetze-im-internet | supported | |
| § 280 Abs. 3 SGB V applies "die auf Grund des § 78 des Vierten Buches erlassenen Rechtsverordnungen entsprechend" | gesetze-im-internet | supported | Labelled inference for MDs: fair |
| Law published 18 May 2026, in force 1 Jul 2026; Art. 14 → €50,000; new § 97a Abs. 5 GWB | BAS circular 1 Jun 2026 | supported | PDF file name says 20260603; letter dated 1 Jun |
| €15,000 until new law, for supplies and services below EU threshold | BAS circular 7 Jan 2026 | partially | Addressed to federal-level bodies only (issue 5) |
| Federal direct awards ≤ €50,000 from 1 Jul 2026 | IHK Schwerin, Vergabeblog | supported | Both [B]; IHK: "Direktaufträge bis 50.000 Euro im Bundesbereich" |
| § 45 SGB XI quotes | gesetze-im-internet | supported | All three quotes verbatim |
| Mobil KK × Gesundheit von Morgen GmbH (PflegeBetreuer), 7 May 2026 | mobil-krankenkasse.de | supported | Fee not stated (issue 2) |
| curendo "Kostenfrei dank Übernahme durch Ihre Pflegekasse" | pflege.de | supported as ad copy | Does not show who pays the vendor |
| calliora founded 2023; "privaten, öffentlichen und kirchlichen Krankenhäusern in fünf Bundesländern" per company | munich-startup.de | supported | "nach Angaben von Calliora" |
| calliora interview 6 Oct 2026, no named customer | startupvalley.news | supported | Page date list shows 6 Oct 2026; no customer named |
| caery TechBoost partner, "Zugang zu Vertriebs- und Partnernetzwerken" | telekom.com 29.09.2026 | supported (quote); channel inference weak | Issue 3 |
| UKE Argo, in-house via subsidiary IDM, 22 Aug 2024 | Ärzteblatt | supported | >2 years old: correct |
| Leipzig UKL-GPT in own data centre, 9 Mar 2026 | Ärzteblatt | supported for date and data centre | No discharge-letter use (issue 4) |
| EU threshold €216,000 2026-27 | review only | supported externally | Issue 8 |
| DKI median planned AI spend €40k; Charité/Lausitz tenders; 8 speech-recognition buyers | internal (`pain-professionals.md`, `hospital-billing-audits.md`) | supported internally | DKI: median €40,000 per chart (checked in the earlier reviews); not re-opened here |

Arithmetic: all four calibration rows recomputed; match except the missing L03 pain cell (issue 1).

## A22 changes (longlist.md, pain-industry.md, pain-professionals.md, payer-processing.md)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| DAK 396194-2026 deadline 14 Jul 2026 | TED API | supported | 2026-07-14T12:00+02:00 |
| gkv informatik 481787-2026 deadline 10 Aug 2026 | TED API | supported | 2026-08-10T12:00+02:00 |
| UK Saarland 508395-2025 deadline 1 Sep 2025 | TED API | supported | |
| MD Bayern 63363-2025 / 126222-2025 deadline 28 Feb 2025 | TED API | supported | Both notices carry the same deadline |
| MD RLP 543912-2025 deadline 5 Sep 2025; MD Nordrhein 762721-2026 deadline 3 Dec 2026 | TED API | supported | |
| DTVP document links return HTTP 404 | curl, 7 Nov 2026 | supported | Both links 404 |
| MD Nordrhein R6 ≥ €500,000 own-development reference; Eignungsleihe | aumass package | supported | Confirmed in A21 re-check (item 6.2); not re-downloaded now |
| 36 notices / 32 buyers; 7 unread thresholds | own tables | supported | Matches the A21 recount (13 + 19 = 32; 5 hospital + DAK + gkv informatik = 7) |
| "No checked notice is open today and startup-accessible" | TED deadlines | supported for the 7 notices re-checked; the "No" rows are inaccessible regardless | |
| MD RLP wording changed to past tense, Charité two notices | text | fixed | A21 issues 1-6 all closed |

Remaining wording nit: `longlist.md` says "DAK ... 'Unlikely'" among unread thresholds and then also states the deadline passed; consistent. No new problems.

## [UNVERIFIED] items
- Scoring.md: purchasing limits of the six Bavarian university hospitals and of municipal hospital GmbHs (marked correctly). Issue 6: the L06 calibration text partly treats the university-hospital case as open ("legally possible").
- Not marked but unsourced in the file: voize founding year and customer (issue 7); caery's and Gesundheit von Morgen's founding years (listed under Gaps: fine).
- No later text treats a marked [UNVERIFIED] item as fact, except the L06 phrase above.

## Unsourced claims and grades
- "Absence in search is not proof of absence" and the L06 "no ≤5-year-old vendor with a named paying hospital found (2 searches)": own search result, disclosed; fine.
- Grades: statutes and regulator circulars [A], IHK/Vergabeblog/press releases [B]: correct. No score rests on [C]. Calibration scores are marked illustrative.
- Stale data: UKE article is >2 years old and is labelled so. All other sources 2025-2026.

## Re-run counts
- TED: 7 notices retrieved via API (deadlines match). Tender-table recount not repeated (done in A21; A22 only changed wording).
- App Store / CT.gov: not applicable.
