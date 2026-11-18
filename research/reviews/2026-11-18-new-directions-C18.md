# Fact-check: research/new-directions.md after the C18 fixes (task C17, fact-check re-check)
Date 2026-11-18 | Verdict: **pass (caveats)** | Sources checked: 8 of 8 new or changed sources (all read in full), plus the TED re-run of the two recorded queries and notice 226625-2025

Scope: only file in `research/` or `ventures/` changed since its latest fact-check (`research/reviews/2026-11-18-new-directions.md`, commit c31940c); diff c31940c..c3abbf5. Sources that were unchanged and already checked in the first review were not re-opened. Business judgement is left to the C17 red-team half. This was the one fix round (rule 14): remaining points are caveats, not tasks.

**What holds.** All 5 critical issues and all 8 minor issues from the first review are fixed. No leftover "direction 4", "spun out", "plain language summaries", "fewer than 55", "every tender" or "pool of buyers" wording in the file. Every new quote was found verbatim in its source. No fabrication.

## Critical issues (must fix)
None.

## Caveats for the CEO (rule 14, no new task)
1. **"About one application in four" for EXIST-Forschungstransfer is a lower bound.** The 27.8 % (634 of 2,280) is cumulative since the programme started, and the report says "Skizzen, die vor April 2023 eingereicht wurden, werden dabei als Anträge gewertet" ([EFT report 2025](https://exist.de/wp-content/uploads/2026/04/EFT_Monitoringbericht_2025_Nr.3.pdf), section 3). Before April 2023 applicants first sent a short outline; counting outlines as applications pulls the rate down. The odds for a full application today may be higher; the report gives no 2025-only rate. Findings, Details §2 and K3 present 27.8 % as "about one in four" without this note.
2. **The 2017 Commission recommendation was worded more strongly than the 2021 guidance.** The 2017 text (mirror, §9) says the summary "is expected to be provided in the local language of each of the EU countries"; the 2021 GLSP says "the EU CTR does not request translations". The file's reading (law = one lay summary; translations = recommended) is correct for the law. Sponsors may still treat the expert-group text as a de facto expectation; whether they pay for it is untested (the file says so).
3. **"a Munich GbR of two occupational physicians" (Details §8)** is read from the winner name "Dres. Dietlmeier & Hohmann GbR" (buyer: TUM, 226625-2025). The two doctors' specialty is not in the TED fields read; minor, not built on.
4. **Task C16 text was written before C18** and does not carry the 27.8 % rate or "translations recommended, not required". The researcher's C18 log entry in `progress.md` tells the CEO both points; the critic may not edit C16.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| "the EU CTR does not request translations"; "as a minimum … local language(s) of each of the countries where the trial took place, matching the languages employed in the PIS/ICF"; English "where resources allow" | [GLSP, EudraLex Vol. 10, adopted 9 Jul 2021](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf), p. 49 (also p. 14) | supported | Verbatim on printed p. 49; adoption date on p. 1 |
| "While one version must be uploaded … no time frame for additional translated LS is defined"; "may consider engaging with a language service provider" | GLSP p. 49 | supported | Verbatim |
| "most funding bodies do not foresee budget allocation for LS preparation"; "it may be impossible to secure funds for LS" (§2.3, p. 22) | GLSP p. 22, §2.3 Cost Implications | supported | Verbatim, section and page match |
| 2017 expert-group recommendation, §9 Language: same local-language rule | [gmp-compliance.org mirror](https://gmp-compliance.org/files/guidemgr/2017_01_26_summaries_of_ct_results_for_laypersons.pdf) | supported | §9: "As a minimum, the summary is expected to be provided in the local language…"; English "not mandatory". [A, mirror] fair (caveat 2) |
| 634 of 2,280 approved, "Förderquote (gesamt) 27,8 %" | EFT report 2025 | supported | Verbatim; includes pre-April-2023 outlines as applications (caveat 1) |
| "Im Jahr 2025 haben Forschende, Studierende sowie Absolventinnen und Absolventen … 115 Start-ups gegründet" | [TUM, 26 Jun 2026](https://www.tum.de/aktuelles/alle-meldungen/pressemitteilungen/details/presidential-award-fuer-raumfahrt-start-up) | supported | Verbatim; wording now "researchers, students and alumni" [B] |
| Peer AI customers include "top 20 pharmaceutical firms and emerging biotechs"; protocols and CSRs; lay summaries not named | [eeNews Europe](https://www.eenewseurope.com/en/peer-ai-raises-12-1m-to-speed-up-drug-approvals-with-agentic-ai) | supported | Verbatim; 0 hits for "lay summar" / "plain language" |
| DDReg sells "Retainer services for QPPV Services" and PV outsourcing in Germany | [DDReg](https://www.ddregpharma.com/pharmacovigilance-services-in-germany) | supported | Verbatim; vendor page [B] fair |
| TK: 80 % (max €150) for external courses; TK courses "in voller Höhe" | [TK](https://www.tk.de/techniker/leistungen-und-mitgliedschaft/informationen-versicherte/leistungen/weitere-leistungen/praevention/gesundheitskurse-2000912) | supported | Verbatim; the earlier "(search result only)" tag correctly removed |
| UK Leipzig bars: references from ≥3 maximum-care/university hospitals, ≥24 months, ISO 9001, ≥2 employed coding physicians | TED 342013-2026 | supported | Matches first review's read of `selection-criterion-description-lot` |
| Lisbon ad with full bonus ≈ €2,328 = ~97 % of €2,409 | Blu Selection (checked in first review) | supported | 1,905.92 + 1,267/3 = 2,328.25; / 2,409.33 = 96.6 % |
| AbD 2 laufend / 2 eingeleitet / 10 eingestellt / 5 nicht durchgeführt / 1 ruhend | G-BA (checked in first review) | match | Same as first review's count |

## Re-run counts
| Recipe (recorded in Details §8) | File | Re-run 2026-11-18 | Result |
|---|---|---|---|
| `classification-cpv=85147000 AND buyer-country=DEU AND notice-type=can-standard AND publication-date>=20240101` | 125 | 125 | match |
| same `AND FT~"betriebsärztliche"` | 36 | 36 | match |
| 226625-2025 winner | Munich GbR | buyer TUM, tenderer "Dres. Dietlmeier & Hohmann GbR" | match |

## [UNVERIFIED] items
| Item | Treated as fact or built on? |
|---|---|
| Per-trial package price €5–10k | Labelled assumption; unchanged (red-team question) |
| No national German rule requiring a German results lay summary (2 searches) | Not built on; recommendation now conditional |
| Max-Planck-Innovation co-founder role (snippet) | Now tagged; counted as snippet, not as an opened signal |
| Redstone 38 researcher-founded TUM start-ups (snippet) | Not built on |
| GTAI free substitute; NIS2 "crowded"; large CROs in RWE; PV incumbents other than DDReg | Now tagged; all on dropped/parked rows |
| EHDS 2029; EudraCT split; Citeline panel price; PV €2k/month; €40k per seat | Unchanged, labelled, not on the critical path |
| Lay-summary language rule | **Resolved**: now sourced [A] and correctly read as guidance, not law |
