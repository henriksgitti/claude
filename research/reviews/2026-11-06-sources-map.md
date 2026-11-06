# Review: research/sources-map.md (A2)
Date: 2026-11-06 | Verdict: pass (minor fixes)

The map is honest about blocks, does not bypass bot checks, and the sample of access claims I re-ran holds up. The problems are about how future tasks will *read* the signals, not about the access tests.

## Critical issues (must fix)
None blocking. Three should-fix items (task A10):
1. **TED count is overstated as "hard willingness-to-pay data" (Findings bullet 2, §4).** "637 German notices" are notices, not distinct procurements or budgets. I re-ran the exact query (POST, 2026-11-06): `totalNoticeCount` = 637, but of the first 50, **30 are contract award notices (`can-standard`), 18 contract notices (`cn-standard`), 2 prior information notices**. One procurement often appears as CN plus CAN, so the count double-counts. `FT~"Krankenhaus"` matches full text, so it also catches non-clinical IT (servers, firewalls, NAC, HR software, licences: 6 of the first 12 titles). Fix: say "notices (incl. award notices; not de-duplicated)" and give a recipe to de-duplicate by procedure ID and to filter by notice type and CPV 48180000/48814000 (medical/clinical software).
2. **Tenders only show above-threshold public buyers.** EU tender notices cover public/public-law buyers above EU thresholds. Private chains (Helios, Asklepios, Korian), most outpatient care services and practices, the PNOG target group, do not appear. Also part of the 2025 volume may be KHZG-funded projects (an expiring programme; KHZG status is `[UNVERIFIED]` in trends.md). The recipe should warn: "TED = public hospital IT demand, likely KHZG-inflated; not a proxy for care-service or practice demand".
3. **Job-count grading.** §3 grades counts [B]. LinkedIn keyword counts are noisy keyword matches and unstable: the same URL showed "6,000+" in A2 and **"4,000+ Open Roles"** when I re-ran it today. Fix: grade [C] (or "[B] source, low reliability"), require same-day snapshots when comparing roles, and never use them for sizing.

## Source check (sample re-run 2026-11-06 via curl/API)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| TED: 637 DE notices, CPV 48000000/72000000, FT "Krankenhaus", since 2025-01-01 | api.ted.europa.eu/v3/notices/search | supported | Count reproduced; titles "Patientenportal… Freudenstadt" and "digitale Pflege- und Behandlungsdokumentation… Geomed" present. See issue 1 on interpretation |
| G-BA Innovationsfonds "861 Ergebnisse" | innovationsfonds.g-ba.de/projekte/ | supported | |
| kununu Helios 2855 reviews, 3.1 | kununu.com/de/helios-kliniken/kommentare | supported | 48% recommendation also on page |
| kununu Korian 2017 reviews | kununu.com/de/korian-deutschland/kommentare | supported | |
| LinkedIn "Medizinische Dokumentation… 6,000+" | linkedin.com/jobs/search… | partially | Today: "4,000+". Volatile (issue 3) |
| StepStone 326 MFA jobs München | stepstone.de | supported | |
| Europe PMC hitCount 392 | ebi.ac.uk REST | supported | |
| ClinicalTrials.gov Munich recruiting 300 | CT.gov v2 API | supported | 300 with `query.locn=Munich` may include "Munich, ND" (US); check country filter |
| CORDIS "nursing" 164 | cordis JSON | supported | |
| App Store search API works (somnio, Oviva counts) | itunes.apple.com/search | supported (access) | Rating numbers not re-checked |
| gesetze-im-internet.de "works (home); deep links need retesting" | — | supported, now stronger | Deep link `gesetze-im-internet.de/sgb_11/__8.html` returned 200 with full text today |
| ~200 URLs tested; "raw log not kept" | — | unverifiable | ~180 access statuses have no evidence trail. Acceptable for a map, but keep a status log next time |

## [UNVERIFIED] items
- Trustpilot KKH "906" reviews (snippet only): correctly marked; not built on.
- Reddit mirror snippets: correctly not used.
- No [UNVERIFIED] item is treated as fact downstream.

## Missing evidence / gaps in the map
- **Munich/Bavaria-specific sources are missing**, although the founder brief makes Munich the base: KVB (Kassenärztliche Vereinigung Bayerns), Bavarian hospital plan (StMGP Krankenhausplan), LGL Bayern, Bayerische Krankenhausgesellschaft, AOK Bayern, Bavarian Pflege statistics (Bayerisches Landesamt für Statistik).
- **Provider directories and quality data** (to size and segment buyers): G-BA Qualitätsberichte der Krankenhäuser, Deutsches Krankenhausverzeichnis, AOK Pflege-Navigator / vdek Pflegelotse (care-service counts per region), InEK data browser. These would close the unverified "~32,000 facilities" and "~1,700 hospitals" counts in trends.md.
- **Competitor financials:** annual reports of listed vendors (CompuGroup Medical, Nexus AG; [A] filings) for pricing/market-share signals.
- **gematik TI dashboard** (connection status of care facilities) as an [A] alternative to the Berlin Senate answer.
- **Existing care-digitisation subsidy uptake** (§8 Abs. 8 SGB XI, €12,000/facility since 2019): where GKV-SV/BAS report uptake. Needed to test the PNOG inference (see trends review).

## Assumptions to challenge
- "Strongest new signal type" (Findings 2): a tender proves a public buyer had a budget for a category; it does not show willingness to pay a startup. Award notices list winners. Use them for **competitor mapping** (who wins), which is arguably more valuable.
- kununu ratings are self-selected employee reviews [C]. Comparing a chain's score "below industry average" says little about a specific workflow pain. Recipe should require theme counts across ≥3 employers, not one chain's score.
- App-store recipe pulls "1–2-star reviews per competitor": that biases towards complaints by design. Report the share of low-star reviews along with the excerpts.
