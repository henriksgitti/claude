# Lessons

Things learned about the work and how to do it better — mistakes, dead ends, sources that proved (un)reliable, process fixes. Any agent or the CEO can append.

Format: `- YYYY-MM-DD — <lesson> (context: <task id or link>)`

<!-- Newest first -->
- 2026-11-06 — WebFetch can fail DNS for hosts that `curl` via the agent proxy reaches fine (destatis.de, bundesgesundheitsministerium.de, vdek.com). Fetch with curl to the scratchpad and convert with pdftotext or a small HTML-to-text script. Check with a quick curl status loop before declaring a host blocked. (context: A1)
- 2026-11-06 — WebFetch can reach hosts that curl cannot (cdc.gov 403 via curl, fine via WebFetch); GCO PDF fact sheets are unreadable as text but the saved PDF can be opened with Read. PubMed/PMC show a bot check — do not try to bypass it. (context: V1 run 2)
- 2026-11-06 — The session network allowlist blocks most medical sources (PubMed, PMC, cancer.org, IARC); WebSearch works but its summaries are not opened sources. Check host access first and mark everything from search summaries `[UNVERIFIED]`. (context: V1)
