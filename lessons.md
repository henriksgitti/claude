# Lessons

Things learned about the work and how to do it better — mistakes, dead ends, sources that proved (un)reliable, process fixes. Any agent or the CEO can append.

Format: `- YYYY-MM-DD — <lesson> (context: <task id or link>)`

<!-- Newest first -->
- 2026-11-06 — For patient pain, the App Store review RSS (100 reviews via page=1,2) gives countable, dated [C] signals fast; forum discovery via WebSearch rarely returns thread URLs. Browse forum index pages directly instead (rheuma-online is at forum.rheuma-online.de; krebs-kompass `forumdisplay.php?f=<id>`). Payer surveys (GKV-SV, WIdO) can contradict advocacy figures (VdK), so always look for the counter-source. (context: A3)
- 2026-11-06 — Tender/job counts need de-duplication and a reliability note: a TED query mixes contract and award notices for the same procurement, and LinkedIn "N+ Open Roles" changed from 6,000+ to 4,000+ within one day for the same URL. Use same-day snapshots and notice-type filters before comparing. (context: A8 review of sources-map.md)
- 2026-11-06 — `site:reddit.com` web search returns almost no reddit.com hits for German queries (0 in 3 tries); English queries return mostly third-party mirror snapshots. Do not use mirrors to get around Reddit's block. Plan pain mining on DE forums, kununu, app-store review APIs, job counts and TED tenders instead. (context: A2)
- 2026-11-06 — Prefer official APIs over web front ends: TED v3 search (POST, no key), Europe PMC REST, PubMed E-utilities, ClinicalTrials.gov v2, OECD SDMX, App Store search/RSS and CORDIS `format=json` all work, while several of the matching websites are behind bot checks. (context: A2)
- 2026-11-06 — WebFetch can fail DNS for hosts that `curl` via the agent proxy reaches fine (destatis.de, bundesgesundheitsministerium.de, vdek.com). Fetch with curl to the scratchpad and convert with pdftotext or a small HTML-to-text script. Check with a quick curl status loop before declaring a host blocked. (context: A1)
- 2026-11-06 — WebFetch can reach hosts that curl cannot (cdc.gov 403 via curl, fine via WebFetch); GCO PDF fact sheets are unreadable as text but the saved PDF can be opened with Read. PubMed/PMC show a bot check — do not try to bypass it. (context: V1 run 2)
- 2026-11-06 — The session network allowlist blocks most medical sources (PubMed, PMC, cancer.org, IARC); WebSearch works but its summaries are not opened sources. Check host access first and mark everything from search summaries `[UNVERIFIED]`. (context: V1)
