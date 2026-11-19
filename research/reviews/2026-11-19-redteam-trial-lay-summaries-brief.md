# Red team: ventures/trial-lay-summaries/brief.md (C25)
Date: 2026-11-19 | Verdict: **needs work** (the test plan and kill lines) / **fail as a venture case** (agrees with the brief's own "niche service, not venture" verdict; not too harsh)

Mode RED TEAM, task C27 second half. First red team of this brief. Facts are taken as checked in `research/reviews/2026-11-19-trial-lay-summaries-brief.md`; its points (TrialAssure removal claim, "small/mid" label, CRO list, citation swaps, arXiv line in the bottom line) are not repeated. One new count was run (CTIS public search, 4,202 ended trials, 19 Nov 2026, method under F3); everything else is reasoning on the brief's own numbers. *My math* and *inference* are labelled. The brief's one fix round is C29 (rule 14); the red-team fixes go into the same round as task C30. After that, remaining issues are caveats.

**Summary for the CEO.**
- **The brief's verdict is right, and if anything still too kind.** Whole EU market ≈ €11m a year at an unobserved price; customers buy once (367 of 476 sponsors had one ending trial in 2025); margins are service margins. No Munich seed fund would invest. "Too harsh" is not a fair reading.
- **The real buyer is probably the CRO, and the purchase happens years earlier.** At small biotechs the lay summary is most likely written into the CRO's contract when the trial starts, not bought at close-out. A newcomer then has to sell to the CRO, which is also the competitor (F1).
- **The CEO adds the least in this chain.** The work is a medical writer's work plus a commodity AI tool. A medical writer can sell this alone; the CEO cannot deliver it alone (F2). "Anyone with a medical-writing background and ChatGPT could do this" is a finding.
- **The €0 quality test cannot pass or fail as written** (the CEO cannot judge factual errors in a trial summary; the AI may have seen the published answer) and **the "5 conversations at the spin-out events" will not reach the right people** (founders and researchers, not clinical-operations leads at small drug companies) (F4, F5).
- **Critic's recommendation for C28 (you decide): (a) drop it as a venture.** If you want to keep a door open, only a lighter (b): one free desk check by the researcher (who wrote the published lay summaries, see Cheapest test T1) and, at most, two questions in conversations you have anyway. No dedicated calls, no DIA trip. Your scarce hours belong to the spin-out deadline (named in a draft application by 28 Feb 2027).

## Fatal or near-fatal objections

**F1. Near-fatal: the buying decision is probably made at trial start inside the CRO contract, not at close-out by the sponsor.**
- Section 3: "at small companies, one clinical-operations or regulatory manager signs a small purchase order at close-out" (*inference, not sourced*). The brief's own data point the other way: 47 % of "other company" trials (330 of 702) and 71 % of US ones name a large CRO; CISCRP's only statement (2018) is that sponsors use "an independent third-party", which a full-service CRO is.
- *Inference:* a full-service CRO contract fixes its scope (CSR, results summary, lay summary, CTIS posting) when the trial is set up, 1–5 years before the summary is due. At close-out the lay summary is then a task inside an existing work order, not a new purchase. To win it, a newcomer must (a) persuade the sponsor to carve it out of a signed contract, or (b) be the CRO's subcontractor, competing with the CRO's own writers and partners (MMS–TrialAssure).
- **Buyer (clinical-operations lead at a Munich biotech):** "Our CRO does the whole close-out under the contract we signed in 2023. If I add you, I need a vendor qualification, a quality agreement, an NDA and a DPA for a €3,500 document, and I take the blame if your number is wrong. Why would I?"
- Section 12 R1 already has "most say 'the CRO includes it'" as a kill. Good. But the confirm line ("≥2 of 5 name an outside purchase ≥€2,500") counts a CRO line item as an "outside purchase", which would pass the test while showing the CRO is the buyer. Fix (C30): "outside purchase" = bought by the sponsor from a firm other than the trial's CRO, under a separate order.

**F2. Near-fatal for founder fit: the CEO is the least necessary person in the value chain.**
- `founder-brief.md`: no clinical, scientific or medical-writing background; AI-agent implementation; German/English; full-time job in Lisbon until Sep 2027. Section 11 says the medical-writer co-founder is a "must have" and that without one "the margin is gone".
- The delivery is: writer reads results → AI draft → writer checks → translator post-edits. The AI part is a prompt pipeline on a general LLM (section 4); SciencePOD already sells the same "AI-Hybrid" model (section 6). *Inference:* an experienced medical writer with an LLM licence can run this alone as a freelance business and keeps 100 % of the margin. The CEO brings sales and a pipeline, but sales here are relationship sales to clinical operations and CROs, where he has no contacts (C16 10-minute check unanswered).
- So the co-founder search (R4) has a harder question than "is anyone willing to talk?": **why would a writer split a €4m-SAM service business with a non-writer?** Fix (C30): R4 kill line adds "no writer candidate accepts a split where the CEO's share is earned by sales they cannot do themselves".
- **Investor:** "Who is the CEO here? The writer. Then why are you pitching?"

**F3. Major: the SAM is smaller and more CRO-bound than 702 trials suggest (new count).**
- Critic count, CTIS public search (`status` 8, 4,202 trials, fields `trialPhase`, `trialCountries`, `sponsorType`), 2025 end dates, sponsorType = "Pharmaceutical company" only, minus a top-50 keyword list: **496** "other company" trials (the brief's 702 uses `isCommercial` and a narrower keyword list, so only the shares below matter) [A, own count, approximate]:
  - **38 %** (190 of 496) are Phase I or bioequivalence studies (155 Phase I, 35 BE; many from generic makers such as Normon, Polpharma, Cinfa, Alter in the recent list). *Inference:* BE summaries are near-identical across a generic maker's studies and are templated in-house; adult Phase I summaries are published only after 30 months (C19), so the sponsor has little reason to pay for polish.
  - **49 %** (245 of 496) run in one country only, 37 % (184) in three or more. The pack's largest cost and value item is translation (€1.4–1.6k of €1.8–2.4k, section 7). One-country trials need one language; the multi-language trials where the pack is worth most are the ones most likely run by large CROs (*inference*, not counted: CRO share by country count is the next desk check).
- *My math, rough:* if BE and one-country Phase I trials drop out of the SAM, the realistic pool is roughly 60 % of the brief's 702, i.e. ~400 trials EU-wide, ~€1.4–2.4m a year at €3,500–6,000. €360k contribution would then need ~23–64 % of it.
- Fix (C30): add phase and country-count splits to sections 3 and 5 and re-state SAM.

**F4. Major: the €0 quality test (section 13 step 1, R3) cannot produce a valid pass or fail.**
- "Pass: 0 factual errors and ≤2 missing items per summary." Who judges a factual error in a trial result? The CEO is not a medical writer, and the researcher is an LLM grading LLM text. Self-grading is not a test.
- The input is the public results summary and the comparison is the sponsor's published lay summary. Both are public and may be in the model's training data; a match can be recall, not drafting skill.
- R3's kill line is "writer time >15 h per pack in the test". The €0 test has no writer, so it cannot measure writer time.
- The real input (unpublished CSR synopsis, confidential) is not tested at all.
- Fix (C30): either (a) pick 3 trials whose lay summary was published after the model's training cut-off, and have the draft scored against the 10 Annex V items by a person with medical-writing experience (outward: needs a named reviewer, CEO approval); or (b) say plainly that the desk test only checks "does the AI miss Annex V items", and remove the writer-time kill from it. R3 is then untested until a writer is found.

**F5. Major: the interview plan's route does not reach the buyers, and cold phone calls are narrower than the brief implies.**
- Section 13 step 3: "step 2 alongside the spin-out events (Jan–Mar 2027) so it costs no extra trips". The spin-out events in the entry pack (UnternehmerTUM info session, Impact Co-Founder Matching, TUM Healthcare Happy Hour, LMU Demo Day) gather founders, researchers and investors, not clinical-operations or regulatory leads of the 63 DACH sponsors or project leads at SocraTec or Winicker-Norimed. *Inference.* BioM events and DIA Europe (Basel, travel cost from €10k budget) are the real routes, and they are extra trips.
- § 7 UWG allows calls to businesses only with "zumindest mutmaßliche Einwilligung" (section 8). *Inference:* a call to a name pulled from CTIS without any prior contact rests on presumed interest, which is a narrow basis; the brief lists "phone" as if it were open. Before approving calls, ask the researcher for the BGH test of presumed consent in B2B cold calls `[UNVERIFIED]`.
- Fix (C30): replace "no extra trips" with the real routes and their cost; state the legal basis for calls or switch to warm intros only.

## Per item: payer / founder fit / incumbents / verdict
| Item | Payer (who signs, budget line) | Founder fit | Incumbents / status quo | Verdict |
|---|---|---|---|---|
| Direct to DACH small sponsors | Clinical-ops/regulatory lead; budget is the CRO work order or close-out budget (*inference*). Vendor qualification (SOPs, quality agreement, insurance) needed even for small jobs `[UNVERIFIED]`, hard for a 1–2-person firm | Weak: no contacts, no writing skill, part-time from Lisbon | CRO bundle; freelance writers at €82.2/h; in-house template for BE/Phase I | 81 trials a year in DACH even at 100 % share (€0.3–0.5m). Not a company |
| White-label to small CROs | CRO project lead or medical-writing head; cost line inside the CRO's quote | Weak: CRO buys writing capacity, i.e. the writer, not the CEO | CRO's own writers; freelancers; SciencePOD | Plausible as a freelance subcontract for a writer; R2 (≥20 packs/year at ≥€2,000) is the right test |
| US biotechs via large CROs | Large CRO's procurement (preferred-vendor lists, audits) | None | Large CROs' in-house teams and partners (MMS–TrialAssure) | Not reachable for a newcomer; the brief says so |
| Non-commercial sponsors (534, 19.5 % overdue) | University / hospital; grant money usually ended at trial close (*inference*) | Weak | KKS/trial centres, do nothing | Pain is highest here but nobody has a budget. The brief rightly excludes it; worth one sentence saying why |
| Seed investor view | — | — | — | €11m TAM, service margins, one-off customers: no fit for HTGF, Bayern Kapital or Munich angels. Bootstrap-only, as the brief says |

**Is the "niche service, not venture" verdict too harsh?** No. The only arguments for "bigger" are adjacent documents (lay protocol synopsis, UK summaries from 2027–28, plain-language summaries of publications). Each is either unverified (synopsis), later than Sep 2027 (UK), or a crowded medical-writing market. None changes who the founder needs to be.

**Is the CRO-channel inference fair?** Fair as a description of where volume sits; too optimistic as a channel. The brief treats CROs as "the channel as much as the competition" (section 6). For a CRO, an outside writer is a margin decision: it buys capacity only when its own writers are full. That is a freelancer market, not a partner channel.

**Are the kill lines fixed and testable?** R1, R2 and R5 are fixed and testable (with the F1 wording fix). R3 is not testable as designed (F4). R4 tests the wrong thing (F2). The overall kill line is clear.

## Pre-mortem and kill criteria
Assume the company folded in late 2029. Most likely reasons, each checked against the brief:
| # | Failure story | Evidence in the brief | Kill criterion (fixed now) |
|---|---|---|---|
| P1 | **No purchase to win.** Sponsors' lay summaries were in the CRO's scope from trial start; the few direct buyers were large firms with frameworks | 47 % / 71 % name a large CRO [A]; decision process is inference; 0 TED tenders | ≥3 of the first 5 sponsor conversations say the summary is in the CRO contract or in-house → stop |
| P2 | **Price collapse.** AI made the summary a 1-day job for any writer; CROs and freelancers priced at €1,000–1,500, below the pack's €1.8–2.4k direct cost | TrialAssure "less than one day" [B]; SciencePOD hybrid [B]; translation is 60–70 % of cost | Any quote <€1,500 for EN + 1 language from a CRO, language firm or freelancer (R5, keep) |
| P3 | **No writer partner on fair terms.** The one writer who joined left to freelance alone after the first 10 packs | Writer is "must have"; 206–228 open writer jobs in DE [B] compete for the same people | No writer candidate by 31 Mar 2027 who accepts equity for sales/AI work, not only a freelance rate |
| P4 | **One quality incident ended it.** A wrong adverse-event frequency in a published summary; the sponsor's QA dropped the vendor and the reference was lost | Annex V requires AE frequencies [A]; CISCRP/EMWA report a 2023 removal of AI summaries [B]; insurance unchecked `[UNVERIFIED]` | Professional-liability cover not obtainable below ~€2k a year, or a sponsor's vendor questionnaire cannot be passed by a 2-person firm |
| P5 | **No volume.** DACH gave ~10 packs a year; growth needed US biotechs through large CROs that never opened their vendor lists | DACH 81 trials/yr [A]; €360k contribution needs 92–257 packs | No small CRO names ≥20 packs a year at ≥€2,000 (R2, keep) |
| P6 | **Founder time.** Delivery with 10-day turnaround next to a full-time job and the spin-out route; one missed deadline lost the first customer | Part-time to Sep 2027 (founder brief); spin-out kill date 28 Feb 2027 | If the CEO is named in a spin-out draft application, stop this idea (no time for both) |

## Cheapest tests
| Test | Cost | Confirms | Kills |
|---|---|---|---|
| **T1. Desk: who wrote the published summaries** (researcher, no outward action). Open the lay-summary PDFs of 30 trials from DACH/EU "other companies" that ended 2025–26 and record any named writer, vendor or CRO, the languages, and the page layout (template reuse). Many sponsor and vendor summaries carry a "prepared by" line `[UNVERIFIED]` | 1 run | ≥⅓ name an independent writing firm or show no CRO style → a separate market exists | ≥⅔ are CRO or in-house templates, or BE/Phase I copies → P1 confirmed; drop |
| T2. Desk: CRO share by number of trial countries (re-use the brief's 3,388 retrieve records) | 1 run | Multi-country "other company" trials are mostly not run by large CROs | ≥70 % of 3+-country trials name a large CRO → the high-value part of the market is CRO-bound |
| T3. One conversation with a freelance medical writer (CEO's network or EMWA; outward, needs approval) | 1 hour | Writer says small sponsors buy lay summaries from freelancers and names a price ≥€2,500 | Writer says it is a 1-day job at day rate (~€650–800 at €82.2/h, *my math*) or CRO work → P2 confirmed |
| T4. One conversation with a small DACH CRO's medical-writing lead (outward) | 1 hour | Names ≥20 overflow lay summaries a year it would subcontract | "We do it in-house" or "we use freelancers" → R2 fails |
| T5. Only if T1–T4 pass: R1 sponsor conversations, with the F1 wording | 5 h | per R1 | per R1 |

T1 and T2 are free and decide most of this. If T1 kills, no outward step is needed.
