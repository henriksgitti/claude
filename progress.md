# Progress

## Current state
- Project: **Healthcare Venture** (scope opened from cancer to healthcare on 2026-11-06, see `decisions/2026-11-06-scope-pipeline.md`).
- Stage: **A — Scan** (in progress). A1 trends scan drafted (`research/trends.md`); A2 source map drafted (`research/sources-map.md`); A3 patient/caregiver pain drafted (`research/pain-patients.md`, 11 problems); A4 professional pain drafted (`research/pain-professionals.md`, 10 problems). A5 industry/payer pain drafted (`research/pain-industry.md`, 10 problems). A6 Munich ecosystem drafted (`research/munich-ecosystem.md`). A9 reimbursement/funding routes drafted (`research/reimbursement-routes.md`). A10 applied the critic fixes to `research/trends.md` and `research/sources-map.md`. A11 drafted `research/hospital-billing-audits.md` (MD audits, 2027 rules, incumbents). A12 drafted `research/payer-processing.md` (insurer § 302 outsourcing, MD AI tenders, buying routes). A13 drafted `research/trial-recruitment-de.md` (CTIS count, 5 % rule, Kapazitätsinitiative, vendors). A14 applied the critic fixes to the three pain files (tender access tables; WTP downgraded where startups cannot bid). A15 added the § 113e Transformationsstellen route and official § 8 Abs. 8 uptake data to `research/reimbursement-routes.md`. A16 applied the fact-check fixes to `research/reimbursement-routes.md` and `research/munich-ecosystem.md`. A17 (partly) confirmed the 1 % audit tier in the Bundestag-passed text and added an 8-quarter 2027 quota simulation to `research/hospital-billing-audits.md`; the Q3 2026 data and Bundesrat vote are still to come. A19 applied the fact-check fixes to the A11–A13 files and `pain-industry.md` (MD-IT: consortia/capacity borrowing allowed; TriNetX–Clinerion now sourced). **A7 long list drafted (`research/longlist.md`): 30 problems L01–L30** (fact-check fixes applied in A21), 6 raw items excluded/merged; new DE data on cancer screening, hybrid-DRG abolition 2028, pharmacy shortage workload, live-in care. Cancer-only work archived in `archive/`; its V1 draft feeds A7.
- Infrastructure: worker session on environment `healthcare-venture`. WebFetch fails DNS for many hosts (destatis.de, bundesgesundheitsministerium.de, vdek.com), but `curl` through the proxy reaches them: fetch with curl + local text extraction. Reddit is effectively unusable: direct fetch is bot-checked and `site:reddit.com` search returns almost no reddit.com hits (A2). Working alternatives and recipes are listed in `research/sources-map.md`.
- No interviews (by design until Stage D). Decisions: see `decisions/`.

## Next steps
1. Researcher: A18 (scoring fields per long-list row; head start in its task notes); A20 (now unblocked) first; A17 blocked until 2026-12-01 (external data). Critic: optional re-check of `research/longlist.md` after A21.
2. Then B1 (score, top 5) → CEO picks 2–3.

## Open questions
- **Reddit API key (now more important):** A2 found Reddit unreachable (bot challenge; search returns almost no reddit.com hits). A free Reddit app/API key created by the CEO is the only clean route. Without it, A3–A5 rely on German forums, reviews, job ads and tenders.
- Optional allowlist / network change: WebFetch fails DNS for most hosts; curl is blocked by bot checks at trustpilot.com, indeed.com, glassdoor, crunchbase.com, dealroom.co, oecd.org (web), europepmc.org (web), gutefrage.net, aerztezeitung.de, springermedizin.de, background.tagesspiegel.de. Not bypassed.
- ~~CEO: own budget, no-go areas, target date~~ Answered 2026-11-07: €10k own money, no no-go areas, full-time from September 2027 (`founder-brief.md`).
- ~~CEO decision before B1: replace the scoring method?~~ **Decided 2026-11-07 (chat): option (b) + confidence ranking.** `research/scoring.md` now has knock-outs K1/K2 and confidence rules R1–R4 (H/M/L per score, L capped at 3, tiers + sensitivity check). Still useful for founder fit: the 10-minute founder-access check in the red-team review ("Cheapest tests" 1).
- **CEO decision before B1: approve the scoring v2 fixes?** `research/reviews/2026-11-07-redteam-scoring-v2.md` lists 10 one-line edits to `research/scoring.md` (must-fix 1–6: K2 needs a sourced example of the route in use, else 'K2 unproven'; buyer-specific direct-award limits incl. § 22 Abs. 2 SVHV ≤€50k for insurers; score per A18 wedge; define K1 'category' and 'in force'; define tiers and the R4 order; separate M from L). Recommendation: approve 1–6 now; 7–10 optional. **Decided 2026-11-07 (chat): only fixes 1–6 approved; 7–10 not applied.** A20 unblocked.

---

## Log
<!-- Newest first. Format:
### 2026-11-07 — A7 Long list of 20–30 problems (researcher)
- Done: `research/longlist.md`: 30 problems (L01–L30) merged from P1–P11, S1–S10, I1–I10 and cancer A–E; each with one-line statement, who has it, who pays (proven / budget / plausible / unclear), evidence count and grades, links. Excluded/merged: S6, S9, I10, cancer D; cancer A/B replaced by German data (L17); P7+S8 → L08; I6 split into L22 (hospital-audit work, MD-IT) and L23 (care assessments).
  - New sourced items: colorectal screening participation 7.75 % vs EU minimum 45 %, documented follow-up after positive stool test 12.9 % (G-BA report, Mar 2026) [A]; lung LDCT screening GKV benefit since Apr 2026 [A]; § 115f (hybrid DRG) deleted, short-stay flat rates from 2028 (BT-Drs. 21/8629) [A] → new row L10; pharmacies 20.1 h/week on shortages (ABDA) [B]; live-in care 100k–210k carers/day (BMG report 2024) [A]; ~4m rare-disease patients (BMG 2026) [A]; BARMER runs cancer navigators in-house [B].
  - All rows have ≥2 evidence items with ≥1 [A]/[B]; proven spend in 15 rows, but direct startup access is rare (A14 tender check).
- Not done: scoring fields (signer, budget line, wedge, first-sale route, buyer count) = A18. L10 has no purchase or [C] evidence yet; [C] layer thin overall (Reddit blocked).
- Next: researcher A18; critic A8 review of `research/longlist.md`.
- Tasks added: none.
- Open questions: none new (Reddit API key still open).

### YYYY-MM-DD — <task id> <task title>
- Done:
- Not done / blocked:
- Next:
- Open questions:
-->

### 2026-11-07 — A8 Critic fact-check run 7 (critic, FACT-CHECK)
- Done: re-checked the A21 changes in `research/longlist.md`, `research/pain-industry.md`, `research/payer-processing.md` (review: `research/reviews/2026-11-07-A21-longlist-payer-pain-industry-recheck.md`). Verdict: pass with minor fixes. MD Nordrhein terms (EUR 600k average in-field turnover, 4.0 FTE, 2 productive AI references, consortia) reproduce from the downloaded aumass tender package; MD RLP re-tender deadline 5 Sep 2025 and MD Nordrhein 3 Dec 2026 confirmed via TED API; tender tables recount 36 notices (match) but 32 buyers (file says 33); the 15 zero-[C] rows match.
- Top issues: (1) buyer count 32 not 33, and gkv informatik also unread; (2) stale "MD RLP could apply / open" wording at `pain-industry.md` lines 39 and 224; (3) MD Nordrhein also requires one reference with >= EUR 500k net own development work (omitted), and the "subcontractor" route is inference.
- Not done: unchanged text not re-opened; A18 output does not exist yet; full read of `pain-patients.md` and `pain-professionals.md` after A14 still outstanding.
- Next: researcher A22 (small fixes, can combine with A18).
- Tasks added: A22 (researcher).
- Open questions: none.


### 2026-11-07 — A21 Apply fact-check fixes to research/longlist.md (researcher)
- Done (all 5 issues in `research/reviews/2026-11-07-longlist.md`): MD RLP AI PoC restated as "accessible when tendered, closed 5 Sep 2025, no award in TED" (Findings, L23 row and details); tender count fixed to 36 notices from 33 buyers, 6 still unread (the review said 9 rows; my recount of the two tables gives 6 notices from 6 buyers after reading MD Nordrhein); L10 "~1m cases" = catalogue scope, WIdO counts added; BR-Drs. 620/26 added (Bundestag 15 Oct 2026, not yet law, Bundesrat 20 Nov); [C] gaps list corrected (15 rows without opened voices); L19 marked one [B] only; €15bn gap now points to `trends.md`.
  - **New:** MD Nordrhein 762721-2026 tender documents read (public download on aumass) [A]: average in-field turnover ≥€600k/yr, ≥4.0 FTE, 2 references for productive AI document software; consortia/subcontracting allowed → not accessible alone. Synced in `payer-processing.md` and the `pain-industry.md` tender table.
- Not done: nothing from the fix list.
- Note: I first started A18 from a stale local `main`; after fetching, A21 (added by the critic) came first under rule 7, so I switched. The A18 research done so far (direct-award limits incl. SVHV/MD and Bavarian university hospitals, buyer counts, 10+ young-vendor examples with named customers) is stored in the A18 task notes with URLs.
- Next: researcher A18; critic optional re-check of the A21 changes.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A8 Critic fact-check run 6 (critic, FACT-CHECK)
- Done: fact-checked `research/longlist.md` (A7) and the A17/A19 changes (hospital-billing-audits, payer-processing, trial-recruitment-de, pain-industry), plus spot checks of the A14 pain-patients/pain-professionals revision -> `research/reviews/2026-11-07-longlist.md`. Verdict: **needs work (minor)**, no critical issues, no fabrication. All 14 A7-opened sources and 8 carried-over ones re-downloaded; numbers match (G-BA colorectal 7.75 % / 12.9 %, ABDA 20.1 h, WIdO hybrid DRG, BMG live-in/rare disease, BARMER, BR-Drs. 620/26 with the 1 % tier, DKG EUR 145k, Clinerion deal pages). App Store ratings and Destatis 17.7m re-run: match.
- Top issues: (1) "only one tender open to a new company (MD RLP AI PoC)" is stale: TED 543912-2025 closed 5 Sep 2025; "34 notices" does not reproduce (tables hold 36; 9 rows have unread thresholds). (2) L10 "~1m hybrid-DRG cases in 2026" is the catalogue scope, not billed cases; the cited BT-Drs. 21/8629 is the committee report (passage shown by BR-Drs. 620/26). (3) [C] counts inconsistent between Gaps and table (L23, L26, L27); L19 has only one [B] item.
- Not done: full read of `pain-patients.md` and `pain-professionals.md` after A14 (spot checks only, no new errors); `scoring.md` not re-checked (red-team scope).
- Next: researcher A21 (fix list, before A18); critic re-check of longlist after A21.
- Tasks added: A21 (researcher, before A18).
- Open questions: none new.

### 2026-11-07 — A19 Apply fact-check fixes to A11/A12/A13 files and pain-industry.md (researcher)
- Done (all items in the four reviews):
  - `research/payer-processing.md`: MD-IT Lot 3 stays **€7m**, now citing change notice 773326-2026 (6 Nov 2026; cn 751925 said €5m). Re-downloaded the DTVP documents myself (01 Angebotsbedingungen V1.2, 04.1, Bieterinformation 1–2) [A]: €5m turnover (averaged since founding if <3 yrs), 25 staff, 2 references confirmed; **correction:** a finished pilot replaces *one of the two* references (not a 3rd); **new:** consortia and capacity borrowing (§ 47 VgV) are allowed, so "blocked as prime" → "blocked alone; possible as subcontractor or consortium member". SBK €2.19m marked as procedure estimate; DAK 427316-2025 marked `pin-only`; TK/QuantCo 3 bids re-confirmed.
  - `research/hospital-billing-audits.md`: "€1.6bn flows back" → "revenue at risk for hospitals"; MD capacity updated to 31 Dec 2025 (2,148.3 physician FTE); two audit counting bases explained (MD-handled vs GKV-SV reported); "plan to buy AI" → "plan to use"; DKI quartile contradiction noted; calliora "not independently verified" added; §6 AI-spend arithmetic marked "not a TAM line".
  - `research/trial-recruitment-de.md`: TriNetX–Clinerion is **now sourced, not removed**: Citeline/Norstella bought Clinerion (Feb 2023), then sold it to TriNetX (Apr 2023) per both deal counsels [B]. Netherlands (55) added; Munich "about 300"; 69.7 % = 46 of 66 RCTs with a budget; 8.5 % discount has no end date (only the exemption is 3 years).
  - `research/pain-industry.md`: "verified in A13" dropped; 33k → 24k participants sourced (vfa Oct 2025 deck p. 7, text-searchable as "33 Tsd."); 5.6m attributed to vdek; PKV "0,001 %" vs computed 0.0098 % noted; MD-IT access wording synced.
- Not done: nothing from the fix list. Pain-patients/pain-professionals A14 edits still await the critic's full check (A8).
- Next: researcher A7 (long list); A17 remainder after ~1 Dec 2026; A20 waits for the CEO. Critic: re-check of these four files is optional (no critical items).
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A17 Refresh hospital audit-quota data (researcher, partly done)
- Done (`research/hospital-billing-audits.md` §1–2, Findings, Gaps, Sources):
  - **1 % tier (≥90 % unobjected) is in the Bundestag-passed text** [A]: BT-Drs. 21/8629 Art. 1b no. 12 (four tiers 1/5/20/40 %, in force 1 Jan 2027, applies to Q1 2027 quotas from Q3 2026 data); BR-Drs. 620/26 contains it verbatim. Bundesrat: TOP 5 on 20 Nov 2026; no consent needed, mediation committee possible [B].
  - **8-quarter re-run (Q3 2024–Q2 2026) incl. the 1 % tier** [A data, my math]: 40 % tier stable at 1,098–1,139 hospital IKs; cap 3.9–4.1× today's (1.30–1.40m invoices/quarter). 1 % tier = 83–127 IKs, mostly tiny audit samples (Q2 2026: 86 of 102 had <20 audits), only 48 % stay next quarter, cap effect ~0.1 %. Q2 2026 reproduces A11 exactly.
  - **§ 17c Abs. 7 KHG joint report: not published**; deadline moved 30 Jun 2025 → 30 Jun 2026; BMG report to the Bundestag due 31 Dec 2026; contract value €145k net (DKG); the 2024 tender had award problems (GKV-SV letter).
- Not done: Q3 2026 statistics (not out; due end of Nov 2026) and the Bundesrat outcome (20 Nov). A17 left open with notes; do not restart before ~1 Dec 2026.
- Side finding for A19: TED change notice 773326-2026 (6 Nov 2026) sets MD-IT Lot 3 to €7m, so the critic's "€5m" fix is outdated (note added to A19).

### 2026-11-07 — A8 Critic fact-check run 5 (critic, FACT-CHECK)
- Done: fact-checked the A15 + A16 changes in `research/reimbursement-routes.md` and `research/munich-ecosystem.md` (plus the one-line sync in `research/trends.md`) → `research/reviews/2026-11-07-A15-A16-reimbursement-routes-munich-ecosystem.md`. Verdict: **pass with minor fixes**, no critical issues. All 27 sources carrying new claims re-downloaded; BAS payouts 2019–2024, DAK figures, § 113e text (cabinet draft), wages, FLÜGGE 2026/1 call, EY (−46 %), EIC dates, UnternehmerTUM "keine Unternehmensanteile" all match.
- Top minor issues: (1) SCE "not rolling" is overstated: the same page says "Dauerhaft für die SCE Incubation bewerben"; next-intake date is inference. (2) FINSOZ's 5.6 FTE is a refinanceable cap on extra posts, not the § 113e corridor; FINSOZ's own conservative case is 2.8 FTE, so the €16–19k per home / €128–151m national figures may be overstated (labelled inference). (3) Uptake math uses 32,054 facilities while DAK's "48 % = 17,500" implies ~36,500; the 37 % vs "knapp 40 %" match is partly coincidence. Also: Länder catch-up rule omitted.
- Not done: no other file is new since its fact-check (scoring, A11–A13 files, pain files unchanged); full A14 re-check of pain-patients/pain-professionals still open; vdek, KHZG, GKV-SV position paper (Aug 2026) not re-opened.
- Next: researcher may fold the five minor fixes into the next edit of these files (no separate task added; none is critical). Critic: A8 continues with A17/A18/A7 outputs when they exist.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A16 Apply fact-check fixes to reimbursement-routes.md and munich-ecosystem.md (researcher)
- Done (all 9 items; 4–5 were done in A15):
  - `research/reimbursement-routes.md`: GKV-SV PM regraded [B]; § 40a Abs. 1a quoted verbatim (excludes work organisation of *outpatient* services and apps "ausschließlich" for benefits advice; carer-relief apps explicitly included, so a hybrid carer-relief app is not excluded, inference); 1.9m = users of *any* insurer-funded prevention measure (vdek quote); KHZG €4.3bn synced from A10 (was `[UNVERIFIED]`).
  - `research/munich-ecosystem.md`: SCE Incubation is **not rolling**: two batches/yr (Mar–Jul, Sep–Jan), last deadline 2 Aug 2026, next (summer 2027) deadline not published. UnternehmerTUM Incubator "wir nehmen keine Unternehmensanteile" now sourced. **FLÜGGE call 2026/1** opened [A]: up to 4 projects (~€500k), sketches via a state Bavarian Hochschule by **18 Dec 2026**, panel 18 Mar 2027, start ~1 Jul 2027. EY: Bayern >€1.1bn = **−46 %** y/y; "B2B workflow AI" trend now labelled as a two-deal anecdote. EIC 2027 batching dates 20 Jan / 17 Mar / 1 Sep / 4 Nov re-checked on the EIC page.
- Not done: SCE summer-2027 deadline (not yet published); no Munich health deal count by segment (Crunchbase/Dealroom blocked).
- Next: A17. Critic: fact-check the A15 + A16 changes.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A15 § 113e Transformationsstellen and § 8 Abs. 8 uptake (researcher)
- Done: `research/reimbursement-routes.md` updated.
  - New §4b + table row for **§ 113e** (bill 21/8869, text identical to the cabinet draft): residential homes only, 2028–2032, ≤10 % of the staffing-corridor posts, valued at care minimum wage × 1,560 h, catalogue-gated (Kompetenzzentrum, from 30 Sep 2027). My estimate: ~€16–19k/yr per 100-resident home (FINSOZ example), ceiling ~€100k (DBfK). Nationally ~€43–151m/yr (inference). GKV-SV wants it replaced by a study until 2031 (only ~1/3 of homes have the needed staffing split); DBfK and ver.di want it struck; FINSOZ wants 50 %.
  - **§ 8 Abs. 8 uptake reframed with official data:** BAS national payouts €143.3m 2019–2024 [A] (€24–32m/yr since 2020, flat) ≈ 37 % of the €384.6m pool; ~65 % of DAK-processed facilities used it; vdek 20–30 % = full amount used. "Weak uptake" and the unsourced "IT capacity, not money" claim are removed.
  - New facts: the PNOG 1st reading happened on 5 Nov 2026 (bill went to the Health Committee); the old €12k grant drops "Entlastung der Pflegekräfte"/workflow items from 2027; the bill's general reasoning still says "ambulanten und teilstationären" for the €1.6bn fund (law text: "ambulanter und stationärer").
  - Also did A16 items 4 and 5 (same paragraphs). Synced the uptake gap line in `research/trends.md`.
- Not done: no AOK or GKV-SV count of facilities using the grant was found; BAS 2025 figure not found; GKV-SV § 113c Abs. 8 report (the "one third" figure) not opened.
- Next: A16 (remaining items 1–3, 6–9). Critic: fact-check the A15 changes in `research/reimbursement-routes.md`.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — Red team v2 of research/scoring.md (critic, RED TEAM)
- Done: reviewed the revised method (K1/K2 + R1–R4, CEO option (b)) → `research/reviews/2026-11-07-redteam-scoring-v2.md`. Verdict: **needs work** (rejected options not re-argued).
- Top issues: (1) K2 only fires if *no* direct-award, private-buyer or channel route exists. Such a route is almost always legally possible, and below-threshold and private purchases are invisible in TED. So K2 lets through S1/S3/S7/S8, where every checked tender is closed. (2) "Inference" is in both M and L, so WTP and achievability get tagged M and R2/R3 never fire. Worked example: an S1-type row scores 78/90 (76 after R4) and reaches the top 5. (3) Tiers A/B/C, the R4 order (−1 before or after the cap) and the score for unknowns are undefined. (4) K1 "category" and "budget line" are undefined (draft-law money, price lists). (5) Insurers' direct-award limit is § 22 Abs. 2 SVHV ≤€50k [A], not BayWiVG.
- Proposed: 10 one-line fixes (1–6 must-fix before B1), for CEO approval. `scoring.md` not edited.
- Tasks added: A20 (researcher, blocked on CEO approval), inserted before A18.
- Not done: no B1 scores computed; whether MDs fall under the SVHV and whether BayWiVG covers university/municipal GmbH hospitals is `[UNVERIFIED]`; BAS circular of 8 Jan 2026 not opened.
- Open questions: CEO approval of fixes 1–10 (see Open questions).

### 2026-11-07 — A8 Critic fact-check run 4 (critic, FACT-CHECK)
- Done: fact-checked `research/hospital-billing-audits.md` (A11), `research/payer-processing.md` (A12), `research/trial-recruitment-de.md` (A13): all **pass with minor fixes**. Also `research/scoring.md` K1/K2 revision (pass; two procurement thresholds supported by search results only) and a sample of the A14 revision of `research/pain-industry.md` (pass, not a full re-check). Reviews in `research/reviews/2026-11-07-*.md`. Re-run counts: CTIS (12,788 trials, 4,653 transitioned, every year/country figure) **match exactly**; ClinicalTrials.gov matches except Munich recruiting (307 in file, 314 today); GKV-SV 2023–2025 national audit statistics and the Q2 2026 per-hospital 2027 simulation (1,100/231/193 hospitals; 532 below 50 %) **match**; 28 TED notices, MD Bund report and DKI survey re-checked.
- Top issues: (1) MD-IT framework Lot 3 value is EUR 5m in TED, not EUR 7m, and the MD-IT eligibility rules rest on DTVP documents I could not re-read. (2) "TriNetX owns Clinerion" is stated as fact in A13 Findings and copied into `pain-industry.md` as "verified in A13", while A13's own Details call it snippet-level and the opened source says Citeline/Norstella bought Clinerion in 2023. (3) Smaller overstatements: Netherlands (55 single-country trials) left out of the "Germany has the most" list; 69.7 % budget overrun is of 66 RCTs, not 93; "most hospitals plan to buy AI" is "plan to use" in DKI; two incompatible MD audit counts and a stale 2023 MD capacity figure in A11.
- Not done: pain-patients.md and pain-professionals.md edits from A14 not read; vfa 2013 position PDF unreadable as text; Probando/Carelane/Ancora not opened (blocked, flagged in the files); DTVP tender documents not re-read; BayWiVG and federal EUR 50k thresholds only seen as search results.
- Next: researcher A19 (fix list, inserted before A7). Critic: remaining A8 items (A14 pain-patients/pain-professionals, A15, A16, A17, A18 outputs, A7 long list).
- Tasks added: A19 (researcher: apply fact-check fixes), inserted before A7. A8 left open (notes updated).
- Open questions: none new.

### 2026-11-07 — A14 Apply critic fixes to the three pain files (researcher)
- Done: `research/pain-industry.md`, `research/pain-professionals.md`, `research/pain-patients.md` revised.
  - Read the eligibility criteria (TED `selection-criterion-description-lot`) of 34 tender notices used as WTP evidence and added a "Tender access check" table to the industry and professionals files. Only one is open to a new company: the MD Rheinland-Pfalz AI PoC (one PoC reference, no turnover minimum). UK Saarland speech recognition has no turnover minimum but needs 2 live hospital references. All others need €250k–€10m turnover, university-hospital/GKV references, ISO 9001/27001 or a KHZG certificate [A].
  - WTP downgraded: I5 and S3 → "high buyer budget, low direct startup access"; S1, S7, S8 → "no direct access". I5 split into scan/intake BPO (5 buyers) vs billing check (3). DAK €890m reworded as claims volume checked.
  - Harzklinikum 492877-2025 re-labelled as clinical decision support; MDR caveat from MDR Annex VIII Rule 11 (EUR-Lex) and MDCG 2019-11 rev. 1 [A]: decision-support features → class IIa+.
  - Sourced or fixed: 92 insurers; 15 MDs (MD Bund report); 1.52m (2014) → 1,431,000 assessments in 2013 (MDS); 19m → 17.7m inpatients 2025 (Destatis); 1.8m nurses → 446,425 + 817,711 care-facility staff (2023); 150,000 → 191,875 contract practitioners.
  - [C] counts split into opened vs titles only (A3); leadership 9/9 → 8/9 (A4); ePA contrast added (main insurer apps 4.5–4.8 vs ePA apps 1.3–2.5); €469 marked as among users, self-estimate; voize study COI checked (first author employed by voize); 91 % AOK figure confirmed.
  - I1 updated from A13 (sponsor vs site view, CTIS share, vendors verified, CTMS line removed).
- Not done: thresholds that sit only in tender documents (DAK, gkv informatik, MD Nordrhein, 5 hospital tenders); I4 counter-source; below-threshold buys are invisible in TED.
- Next: A15. Critic: fact-check the three revised pain files.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A13 Clinical-trial recruitment in Germany (researcher)
- Done: `research/trial-recruitment-de.md`.
  - Own CTIS count of all 12,788 public trials [A]: Germany is in 668 of 1,356 (49.3 %) new commercial EU trials in 2025, second only to Spain. It also has the most single-country commercial trials. But its share of trial participants is ~2.9 % [B]. *Inference:* the gap is patients per site, not trial placement.
  - Sponsors cite "fehlende Patienten" for missed targets (72 % of university sites in oncology miss plan by ≥25 %). Sites themselves (N=169, Jan 2026) rate patient identification as a big hurdle in only 4–9 % of cases; staffing/funding is the big hurdle (50–74 %) [B].
  - EHR "patient-finder" systems at 6 MIRACUM university hospitals showed no significant enrolment effect (npj Digit Med 2026) [A].
  - 5 % rule [A]: the BStabG moved it from the G-BA assessment (deleted) to an exemption from the new 8.5 % discount (§ 130a Abs. 1c) for drugs launched from 2027. The BfArM portal is live. Uptake data: none.
  - The Kapazitätsinitiative 2030 is a lobby proposal (3 funding lines incl. recruitment capacity) with no budget or government commitment [B].
  - Sites are paid for patient identification under the 2025 joint costing recommendations, but euro amounts per patient are not public.
  - Vendors: Clariness (incl. Viomedo) merged with SubjectWell (Jan 2026); TriNetX owns Clinerion; Trialbee and Inato report 6,000+ sites each. **MPIRIQ (Munich, 2024)** already sells practice-based trial pre-screening at €99–329/month.
- Not done / blocked: per-patient site fees and sponsor recruitment budgets (not public; Stage D interviews); 5 % rule uptake; DGPharMed survey original; MPIRIQ funding (snippet only). Blocked: forschen-fuer-gesundheit.de, htgf.de, probando.de, ancora.ai, norstella.com, iduneo.com; the Bundesagentur job API returned no JSON.
- Next: A14 (should also update `pain-industry.md` I1 with this file: barometer published 28 Sep 2026; vendors now verified; the "CTMS 65 products" line is not recruitment competition). Critic: fact-check `research/trial-recruitment-de.md`.
- Tasks added: none.
- Open questions: none new.

### 2026-11-07 — A12 Insurer invoice processing and MD assessment automation (researcher)
- Done: `research/payer-processing.md`. Read the award notices for all payer/MD tenders in TED, plus the public tender documents of the new MD-IT AI framework.
  - § 302 outsourcing [A]: 13 awards, 2024–26. IQVIA Health System Services (formerly DAVASO) won 5; the others went to SPS, GFS, mediakom, AZ Emmendingen, GEOS and QuantCo. Where bids are reported, each tender drew only 1–3. Values: €5.5m–€34.3m per lot. One public-law route (§ 88 SGB X) bypasses tenders entirely. DAK €890m is the claims volume checked, not the contract value.
  - Shift from outsourcing to AI software [A]: DAK explored buying AI billing-check software to bring the work back in-house. TK bought DRG scoring software from QuantCo. BITMARCK builds AI "von Krankenkassen für Krankenkassen" [B].
  - Largest new budget [A]: MD-IT framework, 48 months, €88m max for AI case summaries in hospital billing audits. It is explicitly triggered by the statutory audit quotas; bids are due 2 Dec 2026. A startup cannot bid as prime contractor (needs €5m turnover, 25 staff, 2 references); subcontractors are allowed.
  - Most accessible entry [A]: small MD PoC tenders. MD RLP's GenAI care-assessment PoC drew 40 requests to participate and asks for only one PoC reference. The MDs have 2,148 physician FTE and produce only 3.7 % of opinions externally.
  - Admin cap [A]: § 4 Abs. 5 (from 2027) and Abs. 6 (2026: +8 % vs 2024). PNOG slightly reduces care-assessment volume. There are 92 insurers, not 93.
  - Inference: direct § 302 sales fail K2. Payer/MD audit AI has a real budget, but the realistic way in is as a subcontractor or through a small PoC.
- Not done / blocked: most contract values are withheld; several awards are still pending (DAK, BIG, gkv informatik, AOK Rheinland/Hamburg, MD RLP re-tender). AOK Hessen taking checks back in-house is a search snippet only (aok.de: WebFetch DNS fails, page is JS-rendered). caery customers not found. No [C] buyer voices.
- Next: A13. Critic: review `research/payer-processing.md`. A14 should fix "93 insurers" → 92 and the I5 WTP wording using this file.
- Tasks added: none.
- Open questions: none new. (The MD-IT deadline of 2 Dec 2026 is informational only; any contact with bidders would need CEO approval.)

### 2026-11-07 — CEO decision: scoring method (orchestrator)
- Done: applied the CEO's choice to `research/scoring.md`: option (b) knock-outs K1 (no buyer with proven spend) and K2 (no startup-accessible first sale in ≤12 months), plus ranking by confidence (R1–R4: H/M/L tag per score, L counts ≤3, criterion 3 or 5 at L = "unproven", sensitivity check, tiers instead of exact ranks). The 9 criteria and weights are unchanged (max 90), so `templates/venture-brief.md` needs no change.
- Not done: the other red-team proposals (new criteria/weights, K3–K6, minimum bars) were not adopted.
- Next: B1 uses the revised method. A18 (long-list fields incl. first-sale route) supplies the K1/K2 data.

### 2026-11-07 — Red team of research/scoring.md (critic)
- Done: RED TEAM review of the Stage B method → `research/reviews/2026-11-07-redteam-scoring.md`. Verdict: **fail as is**. Reasoning only; 3 new facts checked for the proposed scheme (Art. 20 BayWiVG direct award ≤€100k; federal ≤€50k from 1 Jul 2026; EU threshold €216k 2026–27).
- Fatal objections: (1) purely additive: a "payer unclear" idea beats a clear-payer idea 68 vs 61; (2) "budget owner" ≠ startup can sell (tenders need €0.25–6m turnover, references, KHZG certificate), and direct-award/private-buyer routes are not rewarded either; (3) founder fit = topic match, not buyer access, domain edge, part-time feasibility or co-founder dependency; (4) a score of 3 needs no evidence, so unknowns hide in the middle, and a free pilot meets "achievable"; (5) "≥€1bn EU" market size is top-down and ignores buyer counts (e.g. 15 MDs).
- Proposed: 6 knock-outs + 8 criteria (weights 4/4/3/3/2/2/1/1, max 100) + H/M/L confidence (L capped at 3) + sensitivity check and tiers. `scoring.md` not edited.
- Tasks added: A18 (researcher: long-list fields signer / budget line / first-sale route / status quo / wedge / buyer count), after A7.
- Not done: no B1 scores computed; worked examples are illustrative only.
- Open questions: CEO decision on the scoring scheme (see Open questions).

### 2026-11-07 — A11 Hospital billing audits & coding: size, rules 2027, incumbents (researcher)
- Done: `research/hospital-billing-audits.md`.
  - Size [A]: 1,138,534 MD audit reports in 2025; 48.9 % led to a reduction (avg €2,219.51). My math: ≈ €1.58bn/yr back to insurers (reductions + pre-audit dialogue + penalties). 27 % of audit reasons are coding; 68 % are medical necessity / length of stay.
  - Rules [A]: the BStabG (law, 1 Jan 2027) raises audit quotas to 5/20/40 % (thresholds 80/65 %), with no cap below 50 %, and a €500 penalty and fee. The "switch to sample audits from 2027" in `pain-professionals.md` S3 was a 2024 KHVVG draft and was never enacted, so A14 should fix S3. A 1 % tier for hospitals ≥90 % is pending (Bundesrat 20 Nov).
  - Static simulation on Q2 2026 data: 1,100 of 1,524 hospitals would land in the 40 % tier, and the legal cap rises ~4×. The MD's capacity (2,135 physician FTE) is the real limit. MD Niedersachsen already outsources 20,000 audits (€2m tender).
  - Budget [B] (DKI, Sep 2026): ~4,000 FTE / €245m/yr on audit handling; 51 % of hospitals plan AI for MD audits (median €40k).
  - Incumbents: Tiplu (LOGEX since Jul 2026; MBEG-Assistent in ~30 hospitals; >130 partner hospitals) and calliora (Munich, $6m pre-seed, double-digit hospitals) target exactly the 2027 pain. Also ID Berlin and Dedalus RICO.
  - Inference: big, budgeted, deadline-driven pain, but a crowded window. A newcomer would need a wedge (the payer/MD side, psychiatry/rehab, small private hospitals).
- Not done / blocked: status of the 1 % tier; Q3 2026 statistics (due ~end Nov); GKV-SV/DKG § 17c Abs. 7 report not found; Solventum/3M PDFs blocked (403/404); identity of UK Frankfurt's winner unconfirmed.
- Next: A12. Critic: review `research/hospital-billing-audits.md`.
- Tasks added: A17 (refresh with Q3 2026 data and the 1 % tier decision), inserted before A7.
- Open questions: none new.

### 2026-11-07 — A8 Critic fact-check run 3 (critic)
- Done: fact-checked every research file changed or new since its last review: `research/reimbursement-routes.md` (pass with fixes), `research/munich-ecosystem.md` (pass with fixes), A10 revisions of `research/trends.md` and `research/sources-map.md` (pass). Re-opened ~45 sources; all key numbers match (Bitkom, BStabG/§ 134, PNOG § 11, KHZG penalty annex, DAK, Destatis, Senate answer). TED recipe (637 / 366 cn / 384 procedures / 232 / 140) and ClinicalTrials.gov (300 / 669) reproduce. Reviews: `research/reviews/2026-11-07-*.md`.
- Top issues: (1) SCE Incubation "rolling basis" is not on the SCE page (fixed deadline 2 Aug 2026, passed), and UnternehmerTUM "no equity" is not sourced: the part-time founder path depends on both. (2) A9 still carries the "weak uptake" framing and an unsourced causal claim ("IT capacity, not money") that A10's DAK data contradict; GKV-SV press release graded [A] should be [B]; PNOG Länder co-funding "must" vs draft "sollen". (3) Munich "capital available / B2B workflow AI trend" rests on two deals and omits Bayern VC volume -46% YoY (EY); FLÜGGE "funded up to six projects" is only a plan.
- Not done: pain-* files not re-checked after A14 (A14 still open); ~19 of 43 A9 URLs and ~10 A6 URLs not opened (listed in the reviews); KHSFV § 19 unreachable (connection reset).
- Tasks added: A16 (researcher: apply fixes, combine with A15), inserted before A7.
- Next: researcher A15 + A16, A11-A14; critic reviews new outputs.
- Open questions: none new.

### 2026-11-06 — A10 Apply critic fixes to trends.md and sources-map.md (researcher)
- Done: revised `research/trends.md` and `research/sources-map.md` per both critic reviews.
  - Counts verified [A]: 32,054 care facilities in Dec 2023 (16,505 nursing homes + 15,549 outpatient services, Destatis) and 1,807 hospitals in 2025 (529 public, 549 non-profit, 729 private; Destatis PM 28 Oct 2026). KHZG €4.3bn verified (BMG); DigitalRadar 33.3 → 55.0 (DKG).
  - Framing fixed: the 8.5% FTE cut is a conditional ("müssten"); PNOG and GeDIG are marked as draft everywhere (GeDIG 2nd/3rd reading planned 13 Nov, PNOG 11 Dec 2026); KIM 40% = "applied for"; Pflegestatistik: 800,000 in homes, the definition explains the rise only "zum Teil", 640,000 Pflegegrad-1 people used no services. The old-age-ratio row was correct (33 → 43/45/47 by 2038); I added a note on the second measure.
  - PNOG updated to the cabinet draft: €1.6bn for outpatient **and residential** care, Länder "sollen" co-fund 25%. New: § 113e "Transformationsstellen" lets nursing homes convert up to 10% of the staffing corridor into a tech budget (2028–2032), but only for systems on an evidence catalogue (from 30 Sep 2027).
  - § 8 Abs. 8 grant uptake: DAK processes 48% of facilities. ~11,300 of its ~17,500 used the grant by mid-2025 (64.6%), but only €81.2m ≈ 40% of the funds was drawn. This softens A9's "weak uptake": facilities apply, but small amounts.
  - TED de-duplicated: 637 notices = 384 procedures (366 contract notices = 232 procedures, 139 buyers). Medical-software CPV contract notices: 140 procedures from 110 buyers. Added coverage limits (public buyers only; 729 private hospitals invisible).
  - Job counts downgraded to [C]; kununu needs ≥3 employers; App Store recipe must report the low-star share.
  - New source sections: Munich/Bavaria (KVB, StMGP Krankenhausplan 2026 PDF, Bavarian statistics office, LGL, BKG, AOK Bayern, München Klinik) and provider directories/filings (G-BA quality reports, InEK, AOK-Pflegenavigator, CGM/NEXUS IR, Bundesanzeiger, gematik dashboard = JS only).
  - ClinicalTrials.gov: "Munich" finds 300 recruiting trials, "Munich OR München" 669. A13 must use both spellings.
- Not done / blocked: national (AOK or GKV-SV) uptake of the § 8 Abs. 8 grant not found; incumbent care-software vendors not checked (`[UNVERIFIED]`). Blocked: pflegelotse.de (reset), pflegeportal.bayern.de and lfstat.bayern.de (502).
- Next: A11. Critic: re-check `research/trends.md` and `research/sources-map.md`.
- Tasks added: A15 (update `research/reimbursement-routes.md` with § 113e and the DAK uptake data), inserted before A7.
- Open questions: none new.

### 2026-11-06 — A9 Reimbursement & funding routes for digital health products in DE (researcher)
- Done: `research/reimbursement-routes.md`. 11 routes, each with who decides, amount, timing, evidence and status, almost all from primary law texts and drafts.
  - DiGA: BStabG (in force 30 Jul 2026) adds volume discounts from 2027 (2 % above 3,000 uses/yr, up to 30 % above 100,000) and mandatory first-year price caps. GKV spent €171m in 2025 (0.05 % of GKV spending).
  - DiPA: still zero listed (BMG, Jun 2026). €53/month. Benefits navigation and admin apps are excluded by law.
  - PNOG fund (cabinet 30 Sep 2026): €1.6bn federal + €0.4bn Länder, now also for residential homes. Payouts from 1 Jul 2027; guideline due 30 Jun 2027. My math: ≈€62k per facility over 5 years. Bundestag vote planned 11 Dec 2026.
  - Precedent: the €12k digitisation grant had been used up by only ~20–30 % of facilities in Berlin/Brandenburg by 2024.
  - Hospitals: the transformation fund is not a software budget. No KHZG successor. The KHZG penalty starts weighting actual use: 20 % of it in 2027, 80 % in 2031.
  - Insurers: § 140a contracts are now bound by contribution stability; admin-cost cap from 2027; Innovationsfonds down to €100m/yr.
  - Inference: B2B sales to providers out of their own budgets come first; DiGA/DiPA are later options.
- Not done / blocked: national uptake of the § 8 Abs. 8 grant (only regional vdek data); the current DiGA count (BfArM directory needs JS); the PNOG Bundestag Drucksache (AOK timetable used instead); prevention-course subsidy amounts; PKV. The task's "§64e" is genome sequencing, so § 140a/§ 68a–b were covered instead.
- Next: A10. Critic: review `research/reimbursement-routes.md`.
- Tasks added: none.
- Open questions: none new. Note for B1: suggest that a willingness-to-pay score of 4–5 requires a first revenue route within 12 months that does not depend on a reimbursement listing (`research/reimbursement-routes.md` §7).

### 2026-11-06 — A6 Munich ecosystem: grants, capital, co-founders (researcher)
- Done: `research/munich-ecosystem.md`. Grants (10 programs, with part-time fit), hubs (11), investors (~17), co-founder channels (9), all with sources.
  - Key: the founder stipends (EXIST €2,500/month, FLÜGGE) are not compatible with a full-time job. EXIST allows no active employment and ≤20 h/month of side work, but a sabbatical is OK; applications are accepted until 31 Dec 2027. FLÜGGE requires membership of a state Bavarian Hochschule.
  - Part-time-compatible now: SCE Incubation (≥10 h/week, rolling, prepares for EXIST), UnternehmerTUM Incubator (free, co-founder matching), BayStartUP business plan competition (phase 1 deadline 13 Jan 2027).
  - After founding: Start?Zuschuss! (50 %, max €36k; round 23 planned 25 Nov 2026–10 Jan 2027). EXIST must be approved before founding a company.
  - EIC Accelerator needs TRL 6+. EIT Health (HQ Munich) programmes are closed for now.
  - Competitor signal for A11: Calliora (Munich, AI for hospital billing) raised a >€5.3M pre-seed in Oct 2026 (BHI, Redalpine).
- Not done / blocked:
  - BayTOU 2026 status, INVEST end date and any 2026 BayDiGuP call are unverified.
  - Not opened: Heal Capital (DNS fail / reset), Peppermint and Redalpine (bot check), eu-startups (403). The Munich Startup Insights investor database has been shut down (410).
  - Not covered: pilot partners (Munich university hospitals, insurer innovation units).
- Next: A9. Critic: review `research/munich-ecosystem.md`.
- Tasks added: none.
- Open questions: CEO: is a sabbatical or leaving the job within ~12 months conceivable? EXIST (≈€30k stipend + €30k materials for a team) depends on it. Optional (outward, needs approval): ask SCE / UnternehmerTUM whether a non-alumnus working full-time can join.

### 2026-11-06 — A8 Critic review of Stage A, run 2 (critic)
- Done: reviewed `research/pain-industry.md` (needs work), `research/pain-professionals.md` (needs work) and `research/pain-patients.md` (pass, minor fixes). Re-opened ~45 sources, 9 TED notices (incl. selection criteria), 4 App Store review feeds and the ClinicalTrials.gov counts; nearly all numbers match, App Store and CT.gov counts reproduce exactly. Reviews in `research/reviews/2026-11-06-pain-*.md`.
- Top issues: (1) tenders used as "High WTP" (I5, S3, S8) exclude startups: AOK Hessen requires EUR 6m annual turnover, MUL Lausitz EUR 1m/yr in-field turnover, Charite 3 university-hospital references, Helios a KHZG certificate; DAK's re-tender ("weiterhin") has an incumbent. They prove buyer budget, not startup access. (2) DAK "EUR 890m" is claims volume processed, not contract value; "9 buyers" mixes scanning BPO with billing checks; "1.52m assessments in 2014" is not in the cited vdek page. (3) Harzklinikum "LLM discharge letter" tender is a clinical decision-support system (likely MDR software, needs primary source); A3 [C] counts mix opened threads with titles; ePA app tally picks the worst-rated standalone ident apps.
- Not done: ~40 sources not re-opened (sample-based); Jones Day (Biotech Act) behind Cloudflare on re-fetch. No venture briefs yet (no pre-mortem).
- Tasks added: A14 (researcher: apply A3-A5 fixes, incl. tender eligibility per WTP item), inserted before A7. A8 left open (notes updated).
- Open questions: none new.

### 2026-11-06 — A5 Pain mining: pharma, clinical research, payers, health admin (researcher)
- Done: `research/pain-industry.md`, with 10 problems (I1–I10), each with who has it, who pays, [A]/[B] backing, [C] counts and purchase evidence.
  - Clinical trials (I1/I2), best founder fit:
    - German sites under-recruit: 72 % of university sites miss their plan by ≥25 % (pharma/CRO barometer, Aug 2026).
    - Germany's share of trial participants fell from 4.5 % to ~3 %. My own ClinicalTrials.gov count: industry trials with a German site fell from 15.4 % of all trials (2015) to 10.5 % (2025).
    - Policy is speeding up approvals (MFG, standard contract clauses, EU Biotech Act). Site staff and patient finding remain the gap.
    - Counter-evidence: sponsors rated digital tools a minor hurdle in 2025, and the tool market is crowded (65 trial-management products on Capterra DE).
  - Payers (I5/I6), clearest willingness to pay so far:
    - 9 statutory insurers tendered outsourced invoice/receipt processing since 2025. AOK Hessen: 19.3m invoices over 4 years. DAK: €890m/yr, 2.0m receipts.
    - The MDs are buying AI-assisted assessments (MD RLP care-level assessment pilot, MD Nordrhein malpractice reviews).
    - From 2027, insurers' admin spending may only grow with insured income (§ 4 Abs. 5 SGB V).
  - Other industry pain:
    - EU HTA joint clinical assessment (JCA) dossiers: resource-heavy, but only ~58 JCAs a year and the space is full of incumbents.
    - MDR/IVDR certification: 19.5–21.8 months; 53 % of DACH manufacturers cut R&D. The EU revision proposal (Dec 2025) may shrink this pain.
  - Weak buyers: public-health offices (the federal ÖGD pact ends in 2026) and pharmacovigilance (flat case volume).
- Not done / blocked:
  - The [C] base is thin. Industry pain is not in open forums: Elsmar Cove returned 403, medi-learn has only old career threads, and the krankenschwester.de search needs a session token. Reddit was not used.
  - Primary EU texts were not opened (eur-lex bot check): HTA Regulation, MDR revision, Biotech Act. Law-firm and trade-press summaries were used instead.
  - Not identified yet: the incumbent outsourcers in the payer tenders and the DACH trial-recruitment vendors (snippet only).
- Next: A6 (Munich ecosystem). Critic: review `research/pain-industry.md`.
- Tasks added: A12 (insurer invoice processing and MD assessment automation: incumbents, contract values, buying route) and A13 (clinical-trial recruitment in DE: site economics, vendors, Kapazitätsinitiative 2030), both inserted before A7.
- Open questions: none new. Interviews in Stage D matter more for B2B buyers (sponsors, insurers), whose pain does not show up in public forums.

### 2026-11-06 — A4 Pain mining: clinicians, nurses, practice & hospital staff (researcher)
- Done: `research/pain-professionals.md`, with 10 problems (S1–S10), each with who has it, who pays, [A]/[B] backing, opened [C] counts and purchase evidence.
  - Strongest pain: documentation load. The hospital association institute DKI puts it at 3 h/day for physicians and 2.8 h for nurses (self-estimate). The only measured German study found 93 min/day (19.4 %).
  - Clearest budget owner: hospital coding and MD-audit work. Charité tendered outsourced coding support, Lausitz tendered AI coding software, and DKI ranks MD queries as the most time-consuming duty.
  - Practices: payer requests cost more than 2m hours/yr (KBV), and more than half of practices have weekly TI outages.
  - Funding is shifting. From 2027 the KHZG penalty (up to 2 % per case) starts counting actual *use* of digital services. Under the BStabG, the 2.5 % nurse-relief top-up is clawed back from 2027, and Pflegebudget overruns are no longer refinanced.
  - Counter-evidence: measured AI-scribe gains are modest (16 min per 8 h in JAMA 2026; 15 min per shift in care homes), voize ($50m, 1,100 facilities) already leads in care homes, AI phone assistants are crowded at €9–229/month, and in employer reviews leadership is a bigger complaint than software.
- Not done / blocked:
  - kununu shows page 1 only (the rest sits behind a sign-up, not bypassed), so only kununu's AI summaries were used.
  - krankenschwester.de and medi-learn are low-traffic: 8 threads opened, the rest are titles only. Reddit was not used.
  - LinkedIn job counts are unreliable (fuzzy matching) and StepStone no longer shows counts, so job ads were not used.
  - Not extracted: MD audit volumes, coding incumbents, uptake of the §8(8) SGB XI care-digitisation subsidy.
- Next: A5 (pain mining: industry/payers). Critic: review `research/pain-professionals.md`.
- Tasks added: A11 (hospital billing audits & coding: size, 2027 rule changes, incumbents), inserted before A7.
- Open questions: none new. A Reddit API key would help most for r/medizin and r/Pflege voices.

### 2026-11-06 — A3 Pain mining: patients & caregivers (researcher)
- Done: `research/pain-patients.md`. 11 problems (P1–P11), each with who has it, who pays, [A]/[B] backing, opened [C] signal counts and willingness-to-pay evidence. Strongest: P1 navigating home-care benefits (counselling used by 3% of those entitled, GKV-SV 2026; only 38.4% of Pflegegeld recipients use the relief budget); P2 finding care capacity (91% of home-care services refused new clients, DEVAP 2023); P3 carer overload (WIdO 2026: 46.9% of employed carers highly burdened, €469/month out of pocket); P4 specialist access (25% wait >30 days, GKV-SV 2025). Also: ePA onboarding friction (App Store: 271 of 300 recent reviews of DAK ePA, BARMER eCare and TK-Ident are ≤2 stars), medication shortages, discharge gaps, cancer orientation, rare-disease odyssey (4.7 years, EJHG 2024). Counter-evidence recorded: WIdO finds non-use of care benefits is mainly "no need" or preference, not missing information; the Innovation Fund navigator review found mostly no effect.
- Not done / blocked: [C] base is thin. Reddit was not used; alzheimer-forum.de (403), pflege-forum.org (502), demenz-portal/treffpunkt-pflege (TLS) and patient.info (empty) were unreachable, so P2 and P5 have no opened forum items. ME/CFS, rural GP access and 24-h care figures are snippet-only `[UNVERIFIED]`. Several key data points are >3 years old (flagged in the file).
- Next: A4 (pain mining: professionals). Critic: review `research/pain-patients.md`.
- Tasks added: none.
- Open questions: Reddit API key would mainly help P2, P3, P5 (caregiver and psychotherapy voices).

### 2026-11-06 — A8 Critic review of Stage A (critic)
- Done: reviewed `research/sources-map.md` (pass, minor fixes), `research/trends.md` (pass, minor fixes), `research/scoring.md` (needs work before B1). Re-opened 21 trends sources and re-ran 10 source-map access tests; nearly all numbers match. Reviews in `research/reviews/2026-11-06-*.md`.
- Top issues: (1) the PNOG €1.6bn "budget for a startup" inference ignores the existing §8 Abs. 8 SGB XI care-digitisation grant (max €12k/facility since 2019), whose uptake is the best test of whether grant money becomes purchases; per-facility rules only come with GKV-SV guidelines due 30 Jun 2027. (2) The TED "637 notices" are not de-duplicated (30 of the first 50 are award notices) and half the titles are generic IT; they show public-hospital IT demand, not startup willingness to pay. (3) scoring.md is purely additive (no knock-out for "unclear who pays"), lists DiGA as a 5-level payer example, and has no evidence-confidence dimension.
- Not done: ~19 trends sources not re-opened (sample-based); no venture briefs exist yet (no pre-mortem).
- Tasks added: A10 (researcher: apply trends/sources-map fixes), inserted before A7. A8 left open (notes updated).
- Open questions: CEO: should `research/scoring.md` get knock-out rules (willingness to pay ≤2 or achievability ≤2 → not top 5), a confidence tag per score, and a non-DiGA example for criterion 3 before B1? (Stage B tasks can't be added from Stage A.)

### 2026-11-06 — A2 Source map (nightly researcher)
- Done: `research/sources-map.md`. About 200 URLs across 9 source types were access-tested (curl/WebFetch/WebSearch), each with signal type, grade, access result and recipe. Works: German forums (krankenschwester.de, krebs-kompass, rheuma-online, diabetes forums, onmeda, medi-learn), kununu (incl. review text), App Store API/RSS + Google Play, LinkedIn Jobs/StepStone counts, TED tender API (637 DE hospital IT notices since 2025), G-BA Innovationsfonds (861 projects), CORDIS/EU F&T APIs, BMG/G-BA/Bundestag/insurers, Destatis/Eurostat/OECD SDMX, PubMed E-utilities, Europe PMC REST, ClinicalTrials.gov API, most trade press. Per-task recipes for A3–A6/A9 are included.
- Not done / blocked: Reddit (bot challenge, 0 reddit.com hits in DE `site:` searches; third-party mirrors not used, and the sandbox denied testing them); Facebook/LinkedIn posts (login wall); Google Trends (429); Trustpilot, Indeed, Glassdoor, Crunchbase, Dealroom, OECD web, europepmc.org web, gutefrage, allnurses, Tagesspiegel Background, Ärzte Zeitung, Springer Medizin (bot checks); BA Jobsuche API, Förderkatalog, foerderdatenbank, BAS, SVDGV, Medical Valley EMN (403/502/reset). WebFetch DNS fails for nearly all hosts.
- Next: A3 (pain mining: patients & caregivers). Critic: review `research/sources-map.md`.
- Tasks added: none.
- Open questions: Reddit API key (see Open questions, now more important).

### 2026-11-06 — A1 Trends & policy scan (DE/EU) (nightly researcher)
- Done: `research/trends.md`. Ageing (Destatis 16. kBV), care demand and workforce gap, physicians, chronic disease, hospital reform (KHVVG/KHAG, €50bn fund), digitisation (ePA, GeDIG, FDZ, DiGA, Notfallreform, EHDS, AI Act Omnibus) and cost pressure (GKV/SPV, FinanzKommission, BStabG), each with figures, who is affected and who pays. ~40 sources opened, graded [A]/[B]. Key inference: payers are cutting costs, while new public digitisation money is flowing to providers (PNOG €1.6bn for outpatient care 2027–31, hospital transformation fund). Treat this as input for A7, not as a conclusion.
- Not done / blocked: primary Destatis releases for health spending 2024 and causes of death 2025 (used [B] reports instead); RKI/GBE prevalence data; PNOG cabinet version (used the 5 Jun 2026 draft). WebFetch DNS-blocked destatis.de, bundesgesundheitsministerium.de and vdek.com, so all were fetched via curl. eur-lex.europa.eu returns 202/empty (bot check), oecd.org returns 403, gesetze-im-internet.de does not connect.
- Next: A2 (source map). Critic: review `research/trends.md`.
- Tasks added: A9 (reimbursement and funding routes for digital health products), inserted before A7 because the long list and B1 criterion 3 need it.
- Open questions: none new. (Optional: allowlist eur-lex.europa.eu and oecd.org for primary EU texts.)

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher, run 2)
- Done: verified GLOBOCAN 2024 world/Portugal/Germany figures, CDC colorectal 45–75 gap (B), CDC MMWR lung screening 2017 (A, >3 yrs old); added founder-fit ranking per updated task description; recommendation changed A → C (inference). Rewrote `research/problem-statement.md`.
- Not done / blocked: C, D, E core numbers and A's 2022 national figure still `[UNVERIFIED]` (PubMed/PMC bot check; frontiersin.org and uspreventiveservicestaskforce.org DNS-blocked; ascopubs 403). V1 left open.
- Next: verify C first (it is now the top pick); V10.
- Tasks added: V10 (EU/PT/DACH evidence for C and A).
- Open questions: host allowlist (updated list above); does the CEO agree founder fit should outweigh verified-gap size?

### 2026-11-06 — V1 Problem statement and assumptions (nightly researcher)
- Done: drafted `research/problem-statement.md` — 5 candidate problem spaces (A lung screening uptake, B colorectal screening 45–49, C trial enrollment, D financial toxicity, E time-to-treatment), each with problem, who has it, likely payer, key assumptions; provisional recommendation A, runner-up C.
- Not done / blocked: no source could be opened (hosts blocked by network allowlist: pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, www.cancer.org, www.iarc.who.int, ascopost.com). All numbers come from WebSearch summaries and are marked `[UNVERIFIED]`. V1 left open with notes.
- Next: verify leads once hosts are allowed; add IARC/EU data.
- Tasks added: none.
- Open questions: host allowlist; US vs EU vs global focus (see Open questions).

### 2026-11-06 — Setup
- Done: created workspace structure.
- Not done: no research yet (by design).
- Next: V1.
