# Fact-check: research/payer-processing.md (A12)
Date: 2026-11-07 | Verdict: pass (minor fixes) | Sources checked: 45 of ~58 (all 37 TED notices spot-queried for 28; 12 of 17 web sources opened; DTVP documents not re-read)

Method: re-queried the TED v3 API per publication number (winner, value, bids, deadlines, selection criteria), re-opened MD Bund report, buzer laws, PNOG PDF, GKV-SV list, vendor/insurer pages.

## Critical issues (must fix)
None. No fabricated items found.

## Issues to fix (non-critical)
1. **MD-IT Lot 3 value is wrong.** §3 table: "est. €88m / €26m / €7m". TED 751925-2026 field `BT-27-Lot` = 88,000,000 / 26,000,000 / **5,000,000**. Lot 1 (€88m) and Lot 2 (€26m) are correct.
2. **SBK €2,186,760 is an estimate, not an award value.** TED 705454-2026: `BT-27-Procedure` = 2,186,760 (estimated procedure value); the award value is withheld (-1). The table column is "Value" for winners. Mark as "est." as done for BAHN-BKK/Pronova.
3. **MD-IT eligibility (€5m turnover, ≥25 staff, 2 references) and pricing basis rest on DTVP documents** that I could not re-read (page is a Wicket app; no document download tested). TED only says "Siehe Vergabeunterlagen Anlagen 04.1-3". Mark as "read by researcher, not re-verified". The €88m / 2 Dec 2026 deadline themselves are supported.
4. **"13 award notices ... each tender drew 1–3 bids"** is right for all that report bids; the AOK BW notice also lists 8 participation requests, which the table mentions. TK QuantCo bids (3) not re-confirmed (TED API returned no submission field for 546608-2026).
5. **Quote attribution.** DAK "künftig wieder eigenständig erbracht werden" and "KI-basierte Rechnungsprüfungssoftware" come from the procedure description of 427316-2025 (a `pin-only` market exploration), correct, but the file calls it a "market exploration" in prose and "[A]" in the grade. Fine; note it is a prior-information notice, not a tender.
6. **Hospital-side overlap.** The A12 table row "MD Niedersachsen ~20,000 outsourced DRG audits ... €2m" is not re-read here; it is checked in the A11 review (criteria text only).

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 13 awards; IQVIA/DAVASO 5; other winners as listed | TED (re-queried 13 notices) | supported | counts per notice: DAVASO in 366472, 500755, 572311, 32477 (2 lots), 247921 |
| AOK BW €6,480,000, 3 bids, 8 requests, IQVIA HSS | TED 366472-2026 (`result-value-lot`) | supported | |
| AOK Hessen: SPS, 3 bids, 19,257,000 invoices / 4 yrs | TED 213218-2026 | supported | |
| BAHN-BKK est. €8,295,000, 2 bids, €423,836,651.42/yr, DAVASO | TED 500755-2025 / 269243-2025 | supported | 0.49 % math checks |
| Pronova €5,482,000, 1 bid | TED 572311-2024 | supported | |
| IKK classic €5,990,428 + €12,951,709; 2 and 1 bids; €34,313,634, 1 bid, no winner in API | TED 32477-2024, 5516-2024 | supported | |
| AOK Niedersachsen DAVASO 1 bid; AOK PLUS mediakom 1 bid; hkk GFS 3; SBK GFS; BKK mkk AZ Emmendingen 2; vdek GEOS 1 | TED | supported | SBK value = estimate (issue 2) |
| BIG: § 88 SGB X direct award to AZ Emmendingen (143948-2025); BIG cn 189396-2025 €250k turnover + 3 refs | TED | supported | |
| DAK 396194-2026: €890m net volume, ca. 2.0m receipts | TED | supported | volume checked, not contract value: correctly worded |
| AOK NordWest 481787-2026: 3 references | TED | supported | |
| AOK Rheinland/Hamburg 518174-2026: €10m liability cover | TED | supported | est. €10m / 24 months value not re-checked |
| MD-IT 751925/773326-2026: bids due 2 Dec 2026; lots €88m / €26m / €5m | TED | partially | Lot 3 wrong (issue 1) |
| MD Nordrhein 95051-2025 eventus, 9 submissions; 762721-2026 due 3 Dec 2026 | TED | supported | |
| MD RLP 483916-2025: 40 requests, `chan-need`, no award; re-tender 543912-2025 asks for reference list where a finished PoC counts; no turnover in TED fields | TED | supported | |
| MD Bayern 63363/126222-2025: ≥€100,000/yr turnover, 3 references, staff minimum | TED | supported | the lot is an IT-helpdesk chatbot; the table says "Chatbot and AI search", fine |
| MD-IT 94411-2026 4voice €2.5m / 48 months, 2 bids (TED shows 3 submission counts: 2/2/2) | TED | supported | |
| MD-IT 276227-2025 arztkonsultation ak €95,940, 3 bids | TED | supported | |
| MD staff 12,677 / 11,140.6 FTE, 2,148.3 physician, 4,851.7 care, 474.8 coding; 2,812,183 opinions; 1,252,253 hospital; 1,232,119 § 275c; 36 %; external 3.7 % / 3.5 % / 60.4 % dentistry | MD Bund report 2024–2025 | supported | |
| § 4 Abs. 5 and 6 SGB V (8 % over 2024 for 2026; IT-security exempt) | buzer § 4 | supported | |
| § 197b "wirtschaftlicher" | buzer | supported | |
| 92 insurers (Stand 07.11.2026) | GKV-SV list | supported | |
| PNOG: "knapp 12 Prozent" / "etwa 22 Prozent", 3,000–60,000 uses, "knapp 70 Millionen" | BMG PNOG PDF | supported | the "12/22 %" figures are in the MD-assessment reasoning; the file words them as recognition drop, matching the source |
| DAVASO: ~1,350 staff, 230,000 providers, ~€25bn billing volume, part of IQVIA since 2021; 55,000 direct billers (2024) | DAVASO PR (Jun 2025), IKK classic PDF | supported | |
| TK: IQVIA HSS central intake | tk.de | supported | |
| DAK uses GFS for § 300 | dak.de | supported | |
| BITMARCK KI-Marktplatz, "von Krankenkassen für Krankenkassen" | Annual report 2025 | supported | "KI-Life-cycle" and DAK "KI-Partnerschaft" wording not individually located |
| bitDetect 2022 pilot, "DRG-Prüfung: Scores" | BITMARCK slides 2022 | supported | |
| caery / Telekom, "Leistungsprüfung, Abrechnung und Auszahlung" (29 Sep 2026) | Telekom | supported | |
| gkv informatik JV incl. Barmer, HEK (old) | cio.de | supported | |
| EU threshold €216,000 | IHK table | supported | |
| DAVASO kununu 3.2, 361 reviews, 50 % recommend, "Viel Leistungsdruck" | kununu | supported | page also shows 52 % in a different filter |
| AOK Hessen insourcing from 1 Aug 2026; GFS hedge-fund owner; eventus Munich HQ; os-care = AOK Systems | snippets | unverifiable | correctly flagged `[UNVERIFIED]` |

## [UNVERIFIED] items
- Listed in Gaps: AOK Hessen insourcing, eventus HQ, GFS owner, os-care link. None is used in a finding that decides anything. **Watch:** §3 inference "A Munich assessment firm is thus already the incumbent partner for MD AI" builds on the unverified eventus HQ; the sentence carries the flag, keep it.
- DTVP-based eligibility (issue 3) is in effect unverified by this review.

## Other checks
- Grades: TED notices [A] (official register), MD Bund [A], vendor/insurer sites [B], kununu [C]. Correct.
- Stale: BITMARCK 2022 slides and cio.de article marked >3 years old. Fine.
- Overreach: "MD-IT framework locks in up to 3 vendors for 4 years from ~2027" is a reading of the tender text (3 best bidders), not a fact about awards; labelled implicitly as inference in §7. Fine.
