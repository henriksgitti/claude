# Review: research/trends.md and research/sources-map.md (A10 revision, commit 5351969)
Date: 2026-11-07 | Mode: fact-check | Verdict: pass (both). Earlier critic points on these files are resolved; only minor notes remain.

Method: re-downloaded DAK, Destatis PM 376/2026, Destatis Presseportal (Pflegestatistik), Destatis PD24_033, BMG KHZG page, Berlin Senate answer S19/25964 (PDF), § 8 SGB XI, DKG PDF, AOK G+G Rating Report article, AOK PNOG and GeDIG trackers, BMG Notfallreform page, PNOG cabinet PDF (§ 11, § 113e). Re-ran the TED recipe and both ClinicalTrials.gov counts.

## Critical issues (must fix)
None. All earlier critical points (conditional 8.5 % FTE cut, PNOG as draft, KIM "applied for", facility and hospital counts, TED de-duplication) are fixed and match the sources.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 1,807 hospitals 2025 (529 public, 549 non-profit, 729 private), 468,803 beds, 17.7m patients | Destatis PM 376, 28 Oct 2026 | supported | |
| 16,505 nursing homes + 15,549 outpatient services = 32,054 (Dec 2023) | Destatis table | supported | "Stand 18 Dec 2024" |
| 5.7m care recipients, +730,000 (+15 %), "geht zum Teil auf den weiter gefassten Pflegebegriff zurück", demographic ~100,000; 86 %/4.9m at home, 3.1m Pflegegeld only; 800,000 in homes; 640,000 Pflegegrad 1 without services | Destatis via Presseportal | supported | |
| Nurse gap 280,000-690,000 by 2049; 90,000-350,000 by 2034 | Destatis PD24_033 | supported | 2024 projection on 2019 base (stale, flagged by researcher); "worst-case variant" 350,000 / 690,000 is the unfavourable scenario, not the central one - wording "will be short" is stronger than "280,000-690,000 range" |
| PNOG fund €1.6bn, 2027-31, ambulant + stationär, Länder "sollen" 25 % = €400m, from 1 Jul 2027, guideline by 30 Jun 2027 | PNOG cabinet PDF § 11 | supported | |
| § 113e Transformationsstellenanteile (up to 10 % of corridor, 2028-2032, catalogue from 30 Sep 2027) | PNOG cabinet PDF | partially checked | § 113e exists (art. 1 no. 73) and 10 % wording present at line ~3280; dates not individually checked |
| DAK: ~11,300 of ~17,500 facilities used the grant by mid-2025; €81.2m drawn = "knapp 40 Prozent"; DAK handles 48 % of facilities | DAK PM 1 Sep 2025 | supported | |
| DAK: ~70 % of ~32,000 facilities not on TI; 63 % applied for SMC-B | DAK PM | supported | |
| Nationwide 27 Apr 2026: 83 % applied SMC-B, 50 % activated, 40 % applied KIM | Berlin Senate answer | supported | "Vergleich Bund"; [A] OK (parliamentary answer quoting gematik) |
| KHZG "bis zu 4,3 Milliarden Euro" | BMG KHZG page | supported | |
| DigitalRadar 33.3 → 55.0, +12.6 vs 2024; penalties "nicht mehr braucht" | DKG PM 17 Jun 2026 | supported | interest group, [B] correct |
| Rating Report: 555 accounts of 864 hospitals; 60 % deficit 2027; "müssten" cut ~8.5 % non-nursing FTE by 2030; 400 sites at risk medium-term; 22 % of municipal hospitals | AOK G+G | supported | |
| GeDIG: 2nd/3rd reading 13 Nov 2026; e-referral duty from 1 Sep 2029 ("sollen"); ~€448m/yr relief | AOK GeDIG tracker | supported | still a draft; date will pass in days |
| PNOG timetable 5 Nov / 11 Dec | AOK PNOG tracker | supported | |
| Emergency reform: 116117 split into appointment and acute-care service | BMG | partially checked | passed-on-15-Oct date not re-confirmed on the snippet I read |
| TED: 637 notices = 366 cn + 216 can + 39 VEAT + 18 other; 384 procedures; 232 procedures from 139 buyers (cn); medical-software CPVs 214 cn = 140 procedures, 110 buyers | TED API v3 | reproduced | my re-run: 637 / 366 / 216 / 39 / 18 (10 pin-only + 2 pin-cfc + 2 pmc + 1 can-desg + 1 can-social); 384 procedures; 232 procedures; buyers 142 vs 139 and 111 vs 110 - small difference from how buyer-name lists are de-duplicated, immaterial |
| ClinicalTrials.gov recruiting "Munich" = 300; "Munich OR München" = 669 | CT.gov v2 | reproduced | exactly 300 and 669 on 2026-11-07 |
| BMG: GKV hospital spending +9.6 % (+€9.7bn) 2025; KHVVG/KHAG; Destatis 16. kBV; Krankenhaus Rating; Berlin/other items | various | not sampled | |

## [UNVERIFIED] items
Remaining items in trends.md (primary-care law, MFA shortage, Critical Medicines Act, TI cost refunds, e-billing mandate from 1 Dec 2026) are marked and not used as facts. The care-software incumbents (Vivendi, MediFox, DAN, Snap) are `[UNVERIFIED]` and are a gap for any care-documentation idea.

## Missing evidence
- Incumbents in care documentation and hospital billing: no market share or pricing. B1 cannot score competition for these areas from the files.
- DAK's grant-uptake figure covers 48 % of facilities and is a payer press release with an advocacy goal (DAK demands an "Unterstützungsoffensive"): [B], correctly graded, but treat as favourable to the "uptake is real" reading as well as the "money unspent" reading.

## Assumptions to challenge
- trends.md still sizes "per facility €62,400 over 5 years" at 100 % participation.
- A9 (`reimbursement-routes.md`) still contains the superseded "weak uptake" and "KHZG €4.3bn [UNVERIFIED]" statements; A15 is open to sync them.

## sources-map.md
Recipes work as documented: TED query with `fields` returned the stated counts, CT.gov both counts exact. Grades are correct ([A] documents, [C] for kununu/LinkedIn). The Munich/Bavaria and filings sections (A10 additions, ~25 hosts) were not re-tested for access; they carry an "access tested" statement without a log (the file itself says no log was kept).
