# Fact-check: A21 changes to research/longlist.md, research/pain-industry.md, research/payer-processing.md
Date: 2026-11-07 | Verdict: **pass with minor fixes** (all five issues of the earlier longlist review are fixed; new A21 claims reproduce from primary documents; two small count/staleness slips) | Sources checked: 6 of 6 new A21 sources (TED API x3 notices, aumass tender package downloaded and read: eligibility xlsx, Angebotsbedingungen.pdf; BR-Drs. 620/26 already confirmed in the previous run), plus recount of both tender tables and the [C] column. Unchanged parts of the files were not re-opened (covered by reviews 2026-11-07-longlist, -payer-processing, -A14).

## Critical issues (must fix)
None. No fabrication; every new number traces to an opened document.

## Issues (should fix before A18/B1 cite them)
1. **"36 notice numbers from 33 buyers" is 32 buyers (longlist Findings, bullet 3).** Recount of the two "Tender access check" tables: `pain-industry.md` 16 notice numbers / 13 buyers (incl. MD-IT as one buyer); `pain-professionals.md` 20 notice numbers / 19 buyers (Charité has two notices; the three "Unknown" S1 rows are 3 buyers; Münster and Bremerhaven 2). 13 + 19 = **32**. The 36 notice count and the 16/20 split match.
2. **"Thresholds of 6 notices from 6 buyers are still unread" is incomplete.** Unread: 5 hospital "Unknown" rows (Mittweida, Dietrich-Bonhoeffer, KRH, UK Münster, Bremerhaven) + DAK 396194-2026 = 6, matches. But `pain-industry.md` ("Tender documents not read") still names gkv informatik 481787-2026 as unread (amount not in TED), so the true unread-threshold count is 7 notices/7 buyers, or the gkv informatik row should be counted as "No on reference count alone". State which.
3. **Remaining stale present-tense wording on MD RLP.**
   - `pain-industry.md` line 39: "so a startup with one finished PoC could apply" with no mention that it closed 5 Sep 2025 (fixed only at line 184).
   - `pain-industry.md` line 224 (Inference under the tender table): "only small PoC tenders (MD RLP type) and subcontracting are open to a new company". MD RLP is closed; MD Nordrhein is not open to a newcomer alone. Reword to "were open" / "route existed".
   - `pain-professionals.md` line 175 says "One notice per buyer", but Charité has two notices (186365-2025 / 213191-2026). Cosmetic.
4. **MD Nordrhein: material requirement omitted.** The eligibility sheet (item 6.2 R6) also requires that at least one submitted reference shows own development work of **at least EUR 500,000 net order value** ("reine Lizenz-, Hosting- und Supportentgelte zählen nicht"). This is a stronger barrier than the 600k turnover and is not in longlist, pain-industry or payer-processing. It matters for K2 and for the "possible inside a consortium" inference.
5. **"yes as consortium member or subcontractor" (pain-industry table, MD Nordrhein) is only half supported.** Angebotsbedingungen § 4 allows consortia whose eligibility is shown jointly (supported). § 5 allows subcontractors, but project lead and overall responsibility for architecture and information security must stay with the bidder or a consortium member; subcontractors count only via Eignungsleihe (§ 47 VgV). A startup as plain subcontractor does not satisfy eligibility itself. "Consortium member" is supported; "subcontractor" is an inference and should be labelled so.
6. **"No checked notice is both open today and startup-accessible"**: true for what was checked, but deadlines were re-checked only for MD RLP and MD Nordrhein. For the 'No' rows this is moot (not accessible anyway); for UK Saarland (508395-2025, "Hard") and MD Bayern ("Hard") the deadlines were not verified. Low priority.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| MD Nordrhein open procedure, deadline 3 Dec 2026, AI malpractice-review software (762721-2026) | TED API | supported | deadline-receipt-request 2026-12-03T14:00+01:00; title "KI-gestützte Gutachtenerstellung ... Behandlungsfehler" |
| MD RLP re-tender 543912-2025 request deadline 5 Sep 2025, published 20 Aug 2025 | TED API | supported | deadline 2025-09-05T10:00+02:00 |
| MD RLP first procedure 483916-2025 ended without award, "change of need" | TED API | partially re-checked | Notice exists as can-standard (24 Jul 2025); reason text/40 requests carried from earlier review (confirmed there) |
| "No award notice as of 7 Nov 2026" for the re-tender | TED | not independently re-run | Plausible; searched only by publication number here |
| Average in-field turnover >= EUR 600,000 net over last 3 years; younger firms: available years | Fragebogen_Eignung_MD_Nordrhein.xlsx | supported | Quote matches ("mindestens 600.000 EUR netto"; "Bei kürzerem Bestehen ... genügen die verfügbaren Geschäftsjahre") |
| >= 4.0 FTE besides project lead and deputy | same | supported | "neben Projektleitung und Stellvertretung ... mindestens 4,0 VZÄ" |
| Two references for productively used AI document software; >= 12 months operation (R5) | same | supported | Also: at least 2, at most 4 references; R1 for each; R2-R6 jointly; research projects/demonstrators/pure OCR/chatbots excluded |
| Consortia allowed; project lead, architecture and information security stay with bidder or consortium member | Angebotsbedingungen.pdf §§ 4-5 | supported | See issue 5 on subcontractors |
| Not required: MD reference, malpractice-specific reference | same | supported (omitted in files) | Useful counterpoint; files only list barriers |
| Hybrid DRG: Bundestag 15 Oct 2026, Fristablauf 20 Nov, "§ 115f wird gestrichen", 2028 Kurzzeitfallpauschale | BR-Drs. 620/26 | supported | Verified in previous run; only wording changed |
| L10: catalogue scope ~270k to ~1m, WIdO 363k + 986k cases | Ärzteblatt, WIdO | supported | Wording now correct |
| Payers ~EUR 15bn gap 2027, cited to trends.md | trends.md | supported (internal) | Fixed pointer |
| 36 notices / 33 buyers / 16 + 20 | own tables | notice count supported; buyer count **32** | Issue 1 |
| 15 rows without opened online voices (L02, L03, L04, L10, L11, L13, L15, L17, L18, L22, L24, L25, L28, L29, L30) | longlist evidence column | supported | Recount matches; L23 and L27 have 1; L12 and L14 also have 1 |
| L19 "one [B] item only" | longlist | supported | Fix from previous review applied |

## Re-run counts
- TED: 762721-2026, 543912-2025, 483916-2025 retrieved via API (match). Tender-table recount: 36 notices (match), 32 buyers (mismatch with "33").
- App Store / CT.gov: not applicable to this change.

## [UNVERIFIED] items
- None new. Earlier flagged items (L25 "~375 local health offices", L17 outreach payer, L04/L11 recruiter fees) remain flagged and unused as facts.

## Unsourced claims
- None new.
