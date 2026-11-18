# Direction 1 desk run: trial results and lay-summary service
Task: C19 | Date: 2026-11-18 | Status: draft

Question: is "AI-assisted results summaries + lay summaries (+ translations) for trial sponsors" (direction 1 in `research/new-directions.md`) worth a full venture brief? Grades per `CLAUDE.md` rule 2. *My math* and *inference* are labelled.

## Findings
- **The overdue pool is much smaller than assumed, and it is not where we thought.** Own count of the official EU trial register (CTIS public API, all 12,873 public trials, pulled 2026-11-18) [A, own count]: **1,621** ended trials are past their results deadline. **835 (51.5 %) reported on time, 442 (27.3 %) late, 344 (21.2 %) still have no results summary.** That matches the only published study (116 of 234 on time, ~50 %) [B, preprint] ([TranspariMED](https://www.transparimed.org/single-post/half-of-clinical-trials-of-medicines-in-europe-violate-new-transparency-law-new-study)). For trials that run in **Germany, 85** have neither summary today (42 at top-50 pharma groups, 36 at other companies, 7 flagged non-commercial, of which only 4 at German universities/university hospitals). **Portugal: 12** (all commercial).
- **German academic sponsors comply well; the late payers are pharma and small biotech.** On-time rate for Germany-run trials: universities 82 % (18/22), university hospitals 75 % (21/28), other companies 55 %, top-50 pharma 56 % [A, own count]. EU-wide, academic hospitals are worst (38 % on time; 128 trials still missing, half of them French). Several overdue small biotechs are wound down or bankrupt (Viracta wound down Feb 2025 [B] ([Nasdaq/GlobeNewswire](https://nasdaq.com/press-release/viracta-therapeutics-announces-wind-down-operations-2025-02-05)); Seelos filed Chapter 11, Nov 2024, snippet only `[UNVERIFIED]`). *Inference:* the "overdue rescue" customer is small, mostly non-German, and partly insolvent; it does not carry a company.
- **The real market is the flow, not the backlog: about 1,800 EU trials end per year, ~600 with German sites.** In 2025, 1,826 CTIS trials ended (969 of them transitioned from the old system), 609 with German participation, 115 with Portuguese [A, own count]. Every one needs a results summary and a lay summary (Art. 37(4) CTR [A], [Regulation 536/2014](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf)). Missing or late results are fined up to **€25,000** in Germany (§ 97 Abs. 2d Nr. 2, Abs. 3 AMG) [A] ([buzer.de § 97 AMG](https://www.buzer.de/97_AMG.htm)).
- **Prices exist, all indirect; they support roughly €3–9k per lay summary of labour.** Writing one lay summary takes "between 35 to 105 hours" (EFGCP/EFPIA workshop report, 2022) [B] ([EFPIA](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf)); at the freelance median of €82.2/h (EMWA 2023) [B] that is **€2,877–8,631** (*my math*). US university services charge **$1,000–2,500 per study** for results posting (UCLA, updated 11 Jun 2024) [B] ([UCLA CTSI](https://www.researchgo.ucla.edu/clinicaltrialsgov-0)) and **$5,400** for registration plus upkeep (Emory, Jul 2025) [B] ([Emory memo](https://ocr.emory.edu/_includes/documents/emory-2025-industry-funded-study-fees.pdf)). A UK freelancer sells charity lay summaries at **£200** [B] ([richardberks.co.uk](https://richardberks.co.uk/services/lay-summaries/)). German court translation rate: **€1.95 per 55 characters** (§ 11 JVEG) [A] ([buzer.de § 11 JVEG](https://www.buzer.de/11_JVEG.htm)). No vendor publishes a per-trial price (10+ searches).
- **Sponsors do pay for translations, even though the law does not require them.** Of Germany-run multi-country trials with a posted lay summary, **75 % (372/495)** include a German version; top-50 pharma 82 %, other companies 71 %. Portugal: 77 % (76/99) include Portuguese. EU multi-country trials carry a median of **5** lay-summary documents (one per language) [A, own count]. Academic sponsors rarely translate (their trials are mostly single-country).
- **Crowded supply side, with funded AI entrants.** CROs and writing firms sell lay summaries (Quanticate, Clinbay, Certara, Excelya) [B]; Frankfurt's Trilogy Writing was bought by Indegene in Mar 2024 to add "Generative AI" [B] ([Samedan](https://www.samedanltd.com/press-releases/indegene-acquires-trilogy-writing-consulting-gmbh-a-medical-writing-consultancy/)); Weave Bio raised $20m Series A ($36m total, Oct 2025) [B] ([Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development)); Peer AI $12.1m [B]; TrialAssure claims AI summaries for ~50,000 studies [B, vendor claim, 2023].
- **Verdict: no full brief for direction 1 as framed (overdue-compliance rescue).** A narrower variant (AI-drafted lay summary + translation pack for small and mid-size commercial sponsors, sold through CROs) is plausible on paper but needs 60–167 packages a year from a fragmented, mostly non-German buyer group (*my math*, Details §5), with no medical writer on the team. *Inference:* weaker than assumed in C15. Decide after C20 (direction 2), see "What it means" in `progress.md`.

## Details

### 1. Method (re-runnable) [A, own count]
- Pull all public trials: `POST https://euclinicaltrials.eu/ctis-public-api/search` with `{"pagination":{"page":n,"size":100},"sort":{"property":"decisionDate","direction":"DESC"|"ASC"},"searchCriteria":{}}`, pages 1–100 in both directions, de-duplicate by `ctNumber` → 12,873 trials on 2026-11-18. `ctStatus` 8 = "Ended" (4,194 trials; codes checked against `GET /ctis-public-api/retrieve/<ctNumber>` → `ctStatus`).
- Per ended trial `GET https://euclinicaltrials.eu/ctis-public-api/retrieve/<ctNumber>`: `endDateEU` (global end), `results.summaryResults[]` and `results.laypersonResults[]` (with `submissionDate`), `authorizedApplication.authorizedPartI.sponsors[0]` (`organisation.type`, `commercial`, name), `memberStatesConcerned[].mscName`, `eudraCt.isTransitioned`, `documents[]` with `documentTypeLabel` = "Laypersons summary of results (for publication)" and `languageCode`.
- Deadline: end + 12 months; + 6 months if the age group includes 0–17 (EMA: "within one year … unless the trial includes paediatric participants, in which case … within 6 months") [A] ([EMA CTIS public portal: Trial Results, 21 Aug 2026](https://www.ema.europa.eu/en/documents/other/clinical-trial-information-system-ctis-public-portal-trial-results_en.pdf)). Due = deadline before 2026-11-18.
- Excluded: **1,286** adult-only Phase I trials ("Category 1"), because EMA publishes their results only "30 months after the end of trial date" (same EMA document), so the public data cannot show whether they reported.
- Sponsor groups: CTIS `commercial` flag. Commercial sponsors split by a keyword list of ~50 large pharma groups (Pfizer, Roche, Novartis, Merck/MSD, Sanofi, AstraZeneca, GSK, Lilly, AbbVie, BMS, J&J, Amgen, Gilead, Bayer, Boehringer, Novo Nordisk, Takeda, Astellas, Eisai, Daiichi, UCB, CSL, Teva, Biogen, Vertex, Moderna, BioNTech, Servier, Ipsen, Chiesi, Grifols, Menarini, Lundbeck, LEO, Fresenius, STADA and subsidiaries) vs "other companies (incl. small biotech)". Non-commercial split by `organisation.type`: university, hospital/clinic, other. CTIS has no reliable SME flag (only 4 trials tagged "SME"), so "small biotech" cannot be isolated; "other companies" is the proxy.
- Limits: (a) the protocol may justify a later deadline (Art. 37(4) CTR) and CTIS does not show it publicly; (b) trials that never enrolled may need no results ("Results are expected for trials that have recruited participants", EMA); 39 of the 85 German overdue trials were terminated early; (c) a few posted "results" are placeholders (e.g. "Study terminated without enrollment"); (d) country = trial runs in that country, not sponsor seat. All counts are therefore upper bounds for real non-compliance.

### 2. Overdue results by sponsor type [A, own count, 2026-11-18]
Status of results summaries for trials past their deadline:

| Trials run in | Sponsor group | Due | On time | Late, posted | Still missing |
|---|---|---|---|---|---|
| EU (all) | University | 74 | 42 (57 %) | 16 | 16 |
| | University hospital / clinic | 360 | 135 (38 %) | 93 | 132 |
| | Other non-commercial | 129 | 71 (55 %) | 36 | 22 |
| | Other companies (incl. small biotech) | 540 | 299 (55 %) | 141 | 100 |
| | Top-50 pharma groups | 518 | 288 (56 %) | 156 | 74 |
| | **Total** | **1,621** | **835 (51.5 %)** | **442 (27.3 %)** | **344 (21.2 %)** |
| Germany | University | 22 | 18 (82 %) | 2 | 2 |
| | University hospital / clinic | 28 | 21 (75 %) | 5 | 2 |
| | Other non-commercial | 38 | 26 (68 %) | 8 | 4 |
| | Other companies | 233 | 128 (55 %) | 68 | 37 |
| | Top-50 pharma groups | 289 | 162 (56 %) | 85 | 42 |
| | **Total** | **610** | **355 (58.2 %)** | **168 (27.5 %)** | **87 (14.3 %)** |
| Portugal | All non-commercial | 7 | 5 | 2 | 0 |
| | Other companies | 36 | 17 (47 %) | 11 | 8 |
| | Top-50 pharma groups | 60 | 39 (65 %) | 17 | 4 |
| | **Total** | **103** | **61 (59.2 %)** | **30 (29.1 %)** | **12 (11.7 %)** |

- Trials with **neither** results summary nor lay summary: EU 331 (from 229 distinct sponsors); Germany 85; Portugal 12. Germany: 36 are ≤3 months past the deadline, 38 are 4–12 months, 11 more than 12 months.
- EU academic trials still missing, by country (a trial counts once per country): France 64, Netherlands 18, Denmark 13, Belgium 12, Italy 11, Sweden 10, Spain 8, Norway 7, Poland 5, Germany 4.
- **Named sponsors, Germany-run trials with neither summary** (public CTIS data):
  - Top-50 pharma (42 trials, 26 sponsor entities): Merck Sharp & Dohme (5), Sanofi R&D (4), Roche (3), Eli Lilly (3), and 2 each: Pfizer, Merck Healthcare KGaA, BMS, AbbVie Deutschland, GSK R&D; 1 each: AstraZeneca (2 entities), Amgen, Astellas, Baxalta, Bayer, Boehringer Ingelheim, Celgene, CSL Behring, Eisai, Genzyme, Gilead, GSK Biologicals, Janssen-Cilag, MyoKardia, Novartis, UCB.
  - Other companies (36 trials, 35 sponsors; one trial each unless noted): ROXALL Medizin (2), Acacia Pharma, Amicus, Amylyx, AnaptysBio, Aptose, Areteia, aTyr, BioInvent, Cassiopea, Curis, Dermapharm, Diamyd, Dr. Falk Pharma, Eledon, Equillium, Hexal, Immunovant, Jasper, LIB Therapeutics, Noema, Octapharma, Oculis, Panbela, Praxis Precision, Principia, Realta, Seelos, SK Life Science, Sutro, Syros, Tesaro, Vertanical, Vir, Viracta. (Hexal, Principia and Tesaro belong to large groups but escaped the keyword list; the "other companies" counts are slightly too high for that reason.)
  - Non-commercial (7): Universität Münster, Charité Berlin, Universitätsklinikum Tübingen, Goethe-Universität Frankfurt (1 each); three companies flagged non-commercial in CTIS (Kinarus, RemeGen, Kite).
- **Portugal-run trials with neither summary (12):** other companies: Pathalys (2), Melinta, Alnylam, Equillium, Hexal, Amylyx, Seelos; top-50: Gilead, Sanofi (2 entities), AstraZeneca.
- *Inference:* the German market for "rescue the overdue report" is ~85 trials, mostly at large pharma with internal disclosure teams. German academic sponsors are not the late group. Of the German "other companies" list, most are US/Swiss/Swedish biotechs, and some no longer operate (Viracta: "terminated its employees and will wind down operations", Feb 2025 [B]).

### 3. Annual flow: who must produce these documents [A, own count]
| Trials that ended in 2025 | EU | of which Germany-run | of which Portugal-run | Distinct sponsors (EU) |
|---|---|---|---|---|
| Top-50 pharma groups | 585 | 293 | 58 | 66 entities (19 with one trial) |
| Other companies (incl. small biotech) | 707 | 239 | 51 | 479 (368 with one trial) |
| University hospitals / clinics | 354 | 32 | 3 | 161 |
| Universities | 67 | 19 | 1 | 43 |
| Other non-commercial | 113 | 26 | 2 | 92 |
| **Total** | **1,826** | **609** | **115** | |

- 969 of the 1,826 were transitioned from EudraCT (a one-off wave); 600 were terminated early. New authorisations run at ~2,232 a year (repo, `research/trial-recruitment-de.md`), so the steady flow should stay near 2,000 a year (*inference*).
- *Inference:* the buyer group that a newcomer could reach without a framework contract is "other companies": ~700 trials a year from ~480 sponsors, three in four with a single trial. That is a one-off purchase per customer, which makes each sale expensive to win.

### 4. Prices and rates (task item 2)
| # | Price / rate | What it buys | Source, date | Grade |
|---|---|---|---|---|
| 1 | "Estimated time for writing a LS is between 35 to 105 hours" | Effort per lay summary (planning, writing, review) | [EFGCP/EFPIA GLSP workshop report](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf), workshop Feb 2022 (>3 years old) | [B] |
| 2 | Median €82.2/h (223 respondents) | EU freelance medical writer | [EMWA freelance survey 2018–2023](https://emwa.org/journal/freelancing/seventh-freelance-business-survey-the-freelance-landscape-2018-2023/) (3 years old; via repo C15, fact-checked 2026-11-18) | [B] |
| 1×2 | **€2,877–8,631** per lay summary (35 × 82.2; 105 × 82.2) | Labour value of one lay summary | *my math* | — |
| 3 | Results reporting "Option #1" $2,500, "Option #2" $1,000, registration $1,500 per study | Option 1: the office "will perform data entry" of results; option 2: one or two Zoom sessions plus review | [UCLA CTSI ORA](https://www.researchgo.ucla.edu/clinicaltrialsgov-0), "Last updated: 11 Jun 2024" | [B] |
| 4 | "Emory ClinicalTrials.gov Service Center Fee (PI-initiated only) $5,400"; updates and "results reporting, if applicable, will also result in additional fees" | Registration plus upkeep for investigator-initiated trials | [Emory memo, 10 Jul 2025](https://ocr.emory.edu/_includes/documents/emory-2025-industry-funded-study-fees.pdf) | [B] |
| 5 | "Investment: £200 per summary" (500–750 words) | Lay summary of research outcomes for charities, not CTR-grade | [Richard Berks](https://richardberks.co.uk/services/lay-summaries/), undated | [B] (single freelancer) |
| 6 | Clinical writer "USD 40-60 per hour", experienced "above USD 80"; regulatory writers "USD 100 and above" for complex work | Freelance platform rates | [Kolabtree blog, 14 Aug 2020](https://www.kolabtree.com/blog/how-much-does-it-cost-to-hire-a-freelance-medical-writer/) (>3 years old) | [B] |
| 7 | "1,95 Euro für jeweils angefangene 55 Anschläge" (2.15 if difficult) | Statutory fee for court translators in Germany | [§ 11 JVEG](https://www.buzer.de/11_JVEG.htm) | [A] |
| — | Patient-panel review "$3,000 to $3,500" per summary | Lay-reader testing | Citeline page returns 404; search snippet only | `[UNVERIFIED]` |
| — | Plain-language summary of a journal article $5,940 | Publisher product, not a trial summary | Taylor & Francis; search snippet only | `[UNVERIFIED]` |

- *My math, translation:* if a lay summary is ~10,000 characters `[UNVERIFIED]` length, one translation at the JVEG rate costs 10,000 / 55 = 182 lines × €1.95 = **~€355** (€391 at 2.15). A median multi-country trial has 5 lay-summary documents, i.e. ~4 translations ≈ **€1,400–1,600** per trial at court-translator rates.
- *Inference, package price:* lay summary €2.9–8.6k + results-summary entry (US academic services $1–2.5k) + ~4 translations €1.4–1.6k ≈ **€5–12k per trial** at today's human-labour rates. That is close to the €5–10k assumed in C15, now built from sourced parts. AI drafting lowers the cost of the writing hours, and with it the price buyers will accept (*inference*).

### 5. Customers × price (K3) (*my math*)
- At €6,000 per trial package (assumed mid-point, `[UNVERIFIED]` as a price anyone pays): three salaries (€360k) = **60 packages a year**; €1m revenue = **167**.
- Against the reachable flow of ~707 "other company" trials a year EU-wide: 60 = 8.5 %, 167 = 23.6 %. Against the 239 Germany-run "other company" trials: 25 % and 70 %.
- Against the overdue stock: Germany 85 trials (one-off), Portugal 12. Even all of them at €6,000 = €510k + €72k once.
- *Inference:* the volume exists only EU-wide and mostly through CROs and large pharma vendor lists; a Munich start-up would need many one-trial biotech customers or a subcontracting deal with CROs.

### 6. Competitors (task item 3)
| Player | Type | What it sells | Funding / owner | Source | Grade |
|---|---|---|---|---|---|
| Weave Bio (San Francisco) | AI regulatory documents | "AI-native regulatory platform" for drafting/reviewing submissions | $20m Series A, $36m total (Oct 2025; USVP lead) | [Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development) | [B] |
| Peer AI (San Francisco) | AI regulatory documents | Protocols, CSRs; "top 20 pharmaceutical firms and emerging biotechs" | $12.1m (2025) | [eeNews Europe](https://www.eenewseurope.com/en/peer-ai-raises-12-1m-to-speed-up-drug-approvals-with-agentic-ai) (repo C15) | [B] |
| Yseop (France) | AI clinical writing | Generative AI for study reports; "more than 150 clinical trials" (2023) | Novartis dRx Capital, Eli Lilly | [Yseop](https://yseop.com/news-and-press-releases/yseop-announces-strategic-investment-and-celebrates-milestone-of-150-clinical-trials-powered-by-generative-ai/) (repo C15) | [B] |
| TrialAssure (US, est. 2009) | Disclosure software | LINK GenAI plain-language summaries, "nearly 50,000 documents" (2023) | private | [PRWeb](https://www.prweb.com/releases/trialassure-uses-artificial-intelligence-to-create-plain-language-summaries-for-50-000-studies-listed-on-clinicaltrialsgov-301960306.html) (repo C15; own site 403 today) | [B] |
| Narrativa (Madrid/US) | AI clinical documents | CSRs, patient narratives | $1.3m round (2021; nothing later found) | [PR Newswire](https://prnewswire.com/news-releases/narrativa-raises-an-additional-1-3m-to-help-pharma-companies-accelerate-the-fda-drug-approval-process-through-artificial-intelligence-natural-language-generation-301292601.html) | [B] |
| Artos (YC) | AI regulatory drafting | INDs, protocols, study reports | $0.13–0.5m, sources conflict | search snippets only | `[UNVERIFIED]` |
| Indegene + Trilogy Writing (Frankfurt) | Medical-writing firm in a listed group | Clinical/regulatory writing; Indegene adds "Generative AI" | Acquired 27 Mar 2024 | [Samedan](https://www.samedanltd.com/press-releases/indegene-acquires-trilogy-writing-consulting-gmbh-a-medical-writing-consultancy/) | [B] |
| Quanticate (UK CRO) | CRO service | Lay summaries for "EU CTIS"; "Translation of summaries into local languages"; lay-panel review | private CRO | [quanticate.com](https://www.quanticate.com/lay-summaries-services) | [B] |
| Clinbay (biometrics CRO) | CRO service | Lay summaries "at a cost-effective price" | private | [clinbay.com](https://www.clinbay.com/layperson-summaries) | [B] |
| Certara | CRO / software | "over 200 PLS" authored; CoAuthor AI tool | listed | site 403; search snippet only | `[UNVERIFIED]` |
| CISCRP (US non-profit) | Lay summaries | "thousands of plain language trial results summaries" | non-profit | search snippet only | `[UNVERIFIED]` |
| Citeline TrialScope / TrialSummaries.com, RWS, Lionbridge, CSOFT | Disclosure portals, language providers | Hosting and translating lay summaries (TrialSummaries flyer: 45 languages) | listed / large | search snippets only | `[UNVERIFIED]` |

*Inference:* the job is already sold by CROs, disclosure-software vendors and language companies, and AI-first entrants have $12–36m each. A new entrant's only open angle is price for small sponsors, which AI tools will also compress.

### 7. Do sponsors pay for translations? (task item 4) [A, own count]
| Germany-run trials with a posted lay summary | Trials | With a German version | Multi-country trials | Multi-country with German |
|---|---|---|---|---|
| University hospital / clinic | 31 | 15 (48 %) | 8 | 5 |
| University | 20 | 9 (45 %) | 5 | 1 |
| Other non-commercial | 46 | 27 (59 %) | 30 | 19 |
| Other companies | 229 | 159 (69 %) | 201 | 142 (71 %) |
| Top-50 pharma groups | 274 | 221 (81 %) | 251 | 205 (82 %) |
| **Total** | **600** | **431 (72 %)** | **495** | **372 (75 %)** |

- Portugal-run trials: 84 of 119 (71 %) carry a Portuguese version; multi-country 76 of 99 (77 %); top-50 pharma 50 of 61.
- EU-wide, 667 of 855 (78 %) multi-country trials with a lay summary upload two or more lay-summary documents (median 5, the same as the median number of trial countries); academic sponsors 7 of 24.
- Method: language detected from the CTIS `languageCode` or, where it is empty (748 of 1,585 trials), from the file title (e.g. "_de-DE", "_deu", "German"). Single-country German trials without a tag are probably German already, so the German shares are lower bounds.
- Law vs practice: translations are "recommended, not required" ([Good Lay Summary Practice](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf), repo C18) [A]. The EFGCP/EFPIA report calls "at least one language of the participants and English" "the minimum" [B]. *Inference:* commercial sponsors treat translation as standard and pay for it (in-house or language providers); the translation demand is real but goes to incumbents. Academic sponsors seldom translate, in line with "Academic sponsor organisations have no central budget for experienced 'medical writing' staff" (EFGCP/EFPIA report) [B].

### 8. Legal pressure
- Duty: "within one year from the end of a clinical trial in all Member States concerned, the sponsor shall submit to the EU database a summary of the results … accompanied by a summary written in a manner that is understandable to laypersons" (Art. 37(4) CTR) [A] ([Regulation 536/2014](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf)). Member States must set penalties, including for non-submission of information "intended to be made publicly available" (Art. 94) [A] (same).
- Germany: an administrative offence to submit an Art. 37(4) document "nicht, nicht richtig, nicht vollständig oder nicht rechtzeitig"; fine "bis zu 25.000 Euro" (§ 97 Abs. 2d Nr. 2, Abs. 3 AMG) [A] ([buzer.de](https://www.buzer.de/97_AMG.htm)). No enforcement case found (2 searches) `[UNVERIFIED]`.
- Portugal: Lei n.º 9/2026 (in force 5 Apr 2026) implements the CTR; offences carry €5,000–750,000 fines for companies, "entre outras", for breaches of notification duties [B, law-firm note] ([Abreu Advogados, Mar 2026](https://abreuadvogados.com/wp-content/uploads/2026/03/NL-Novo-regime-dos-ensaios-clinicos-PT.pdf)). Whether late results are a listed offence was not confirmed (law text on diariodarepublica.pt did not load) `[UNVERIFIED]`.

### 9. Access routes for a stranger (no contact made)
| Route | Where / when | What it gives | Source | Grade |
|---|---|---|---|---|
| CTIS public data | Online, free | Named sponsors with overdue or upcoming results (the lists in §2); the trial end dates show who needs documents in the next 6–12 months | own count | [A] |
| EMWA (European Medical Writers Association) | Autumn conference online 9–21 Nov 2026; local groups (e.g. Bologna, 13 Nov 2026); Spring 2027 in Amsterdam, 4–7 May (snippet only) | Where EU medical writers (possible co-founder) meet; membership needed | [emwa.org](https://emwa.org/conference/spring-conference-2027/) (read via WebFetch; Amsterdam date `[UNVERIFIED]`) | [B] |
| DIA Europe 2027 | Basel, 16–18 Mar 2027 | Sponsors' regulatory, disclosure and clinical-operations staff | [DIA newsletter](https://connect.diaglobal.org/dia-europe-2027-newsletter) | [B] |
| PtCRIN (Portuguese clinical research network, ECRIN partner) | Portugal; annual meeting (Coimbra, Jan 2025, snippet only) | Portuguese academic trial units | [ECRIN](https://ecrin.org/news/get-know-our-national-partner-ptcrin) | [B] |
| BioM / BayStartUP life-science events | Munich; BioEntrepreneur Bootcamp 2027 (applications from 2 Nov 2026) | Munich biotech founders (small sponsors) | repo `research/munich-ecosystem.md` | [B] |
| Munich medical-writer job ads | Real Chemistry, Syneos Health, cake Kommunikation (Munich) | Shows where writers work locally | search snippets only | `[UNVERIFIED]` |
| CISCRP call for input on AI lay summaries | Online | Working group of sponsors and writers on AI use | search snippet only | `[UNVERIFIED]` |

## Gaps / [UNVERIFIED]
- No per-trial price from any EU vendor, CRO or tender (TED: 0 notices for "lay summary/summaries", "Laienzusammenfassung"; 9 for "plain language summary", all EFSA communication contracts). The package price is built from effort × hourly rate (§4), not observed.
- EMA's own count of trials with results (promised for end-2026 ACT EU reports) was not yet found.
- "Small biotech" cannot be isolated in CTIS; "other companies" includes mid-size firms (Octapharma, Dr. Falk, Dermapharm).
- Seelos Chapter 11 (Nov 2024), Artos funding, Certara "200 PLS", CISCRP "thousands", TrialSummaries "45 languages", Citeline $3,000–3,500, Taylor & Francis $5,940: search snippets only.
- Whether Portuguese law fines late results specifically; any German enforcement case.
- Lay-summary length (~10,000 characters) used in the translation math is an assumption.

## Sources
- https://euclinicaltrials.eu/ctis-public-api/search and https://euclinicaltrials.eu/ctis-public-api/retrieve/<ctNumber> — own count: 12,873 trials, 4,194 ended, overdue, flow, translations; accessed 2026-11-18
- https://www.ema.europa.eu/en/documents/other/clinical-trial-information-system-ctis-public-portal-trial-results_en.pdf — 12/6-month deadlines, Category 1 30-month publication delay, results expected only if recruited; accessed 2026-11-18
- https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf — Art. 37(4) and Art. 94 CTR; accessed 2026-11-18
- https://www.buzer.de/97_AMG.htm — § 97 Abs. 2d Nr. 2, Abs. 3 AMG, fine up to €25,000; accessed 2026-11-18
- https://abreuadvogados.com/wp-content/uploads/2026/03/NL-Novo-regime-dos-ensaios-clinicos-PT.pdf — Lei 9/2026, fine ranges; accessed 2026-11-18
- https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf — 35–105 hours per lay summary; academic budget gap; translation minimum; accessed 2026-11-18
- https://emwa.org/journal/freelancing/seventh-freelance-business-survey-the-freelance-landscape-2018-2023/ — €82.2/h median (cited from repo C15; fact-checked 2026-11-18)
- https://www.researchgo.ucla.edu/clinicaltrialsgov-0 — UCLA results-reporting fees $1,000/$2,500, registration $1,500; accessed 2026-11-18
- https://ocr.emory.edu/_includes/documents/emory-2025-industry-funded-study-fees.pdf — Emory ClinicalTrials.gov service fee $5,400; accessed 2026-11-18
- https://richardberks.co.uk/services/lay-summaries/ — £200 per lay summary (charity); accessed 2026-11-18
- https://www.kolabtree.com/blog/how-much-does-it-cost-to-hire-a-freelance-medical-writer/ — freelance writer hourly rates (2020); accessed 2026-11-18
- https://www.buzer.de/11_JVEG.htm — § 11 JVEG translation fee €1.95/2.15 per 55 characters; accessed 2026-11-18
- https://www.transparimed.org/single-post/half-of-clinical-trials-of-medicines-in-europe-violate-new-transparency-law-new-study — 116 of 234 on time (preprint); via repo C15
- https://nasdaq.com/press-release/viracta-therapeutics-announces-wind-down-operations-2025-02-05 — Viracta wind-down; accessed 2026-11-18
- https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development — Weave Bio $20m / $36m; accessed 2026-11-18
- https://www.samedanltd.com/press-releases/indegene-acquires-trilogy-writing-consulting-gmbh-a-medical-writing-consultancy/ — Indegene acquires Trilogy (Frankfurt), GenAI; accessed 2026-11-18
- https://prnewswire.com/news-releases/narrativa-raises-an-additional-1-3m-to-help-pharma-companies-accelerate-the-fda-drug-approval-process-through-artificial-intelligence-natural-language-generation-301292601.html — Narrativa $1.3m; accessed 2026-11-18
- https://www.quanticate.com/lay-summaries-services — CRO lay-summary + translation service; accessed 2026-11-18
- https://www.clinbay.com/layperson-summaries — CRO lay-summary service; accessed 2026-11-18
- https://www.eenewseurope.com/en/peer-ai-raises-12-1m-to-speed-up-drug-approvals-with-agentic-ai, https://yseop.com/news-and-press-releases/yseop-announces-strategic-investment-and-celebrates-milestone-of-150-clinical-trials-powered-by-generative-ai/, https://www.prweb.com/releases/trialassure-uses-artificial-intelligence-to-create-plain-language-summaries-for-50-000-studies-listed-on-clinicaltrialsgov-301960306.html — Peer AI, Yseop, TrialAssure (via repo C15, fact-checked)
- https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf — translations recommended, not required (via repo C18)
- https://connect.diaglobal.org/dia-europe-2027-newsletter — DIA Europe 2027 Basel 16–18 Mar; accessed 2026-11-18
- https://emwa.org/conference/spring-conference-2027/ — EMWA Autumn 2026 virtual 9–21 Nov (WebFetch); accessed 2026-11-18
- https://ecrin.org/news/get-know-our-national-partner-ptcrin — PtCRIN role; accessed 2026-11-18
- https://api.ted.europa.eu/v3/notices/search — 0 lay-summary tenders; "medical writing" research-services frameworks only; accessed 2026-11-18
