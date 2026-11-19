# Venture brief: AI-drafted, human-checked lay summary + translation pack for trial sponsors
Task: C25 | Date: 2026-11-19 | Status: draft (not yet fact-checked or red-teamed) | Score: not scored (variant of direction 1 in `research/new-directions.md`; no scoring run for it)

Builds on `research/direction1-trial-summaries.md` (C19, fact-checked in `research/reviews/2026-11-19-direction1-trial-summaries.md`). C19 counts are reused, not repeated. New in this brief: an own count of the sponsors' **seat country** and **CRO use** for every trial that ended in 2025–2026 (3,388 trials, CTIS public API, pulled 2026-11-19), EMA's first official compliance figures, UK rules, AI-quality studies, and cost per package. Grades per `CLAUDE.md` rule 2. *My math* and *inference* are labelled.

**Bottom line for the CEO (researcher's view; you decide):**
- **The job is real and required by law, but the whole market is small.** Every EU drug trial must publish a lay summary within 12 months of its end (Art. 37(4) and Annex V CTR [A]). About **1,826** trials ended in 2025 [A, own count]. If every one of them bought a €6,000 package, the market would be **€11.0m a year** EU-wide (*my math*). The realistic target group, small and mid-size companies, is **702 trials a year** (**€4.2m**). €1m revenue would need **24 %** of that group.
- **Germany and DACH alone cannot carry the company.** Small and mid-size sponsors **based in Germany** ended only **43** trials in 2025 (30 companies); with Austria and Switzerland, **81** (63 companies) [A, own count]. At €6,000 each, that is **€258k** (DE) or **€486k** (DACH) a year even at 100 % market share (*my math*). The largest single group is **US companies (262 trials)**, and **71 %** of their trials name a large CRO as a contractor [A, own count]. So the volume sits with US biotechs and is reached through CROs.
- **The "late report" pressure is weaker than we assumed.** EMA's first official figures (Sep 2026) show companies on time in **83.8 %** of cases; only **5.9 %** of company trials are overdue [A]. Pain therefore comes from workload and cost, not from fines.
- **AI drafting works on paper, but buyers and guidelines demand a human check.** In trials, AI drafts were as good as or better than human drafts (Cochrane RCT, 36 summaries; writers saved >40 % of their time) [A]. But only **12.3 %** of 1,010 patients trust AI-only documents "a lot" [A]. EMA wants generative-AI text used only "under close human supervision" [A]. In 2023, a vendor's ~50,000 AI summaries had to be taken offline after accuracy concerns [B]. So the product needs a medical writer, and the CEO is not one.
- **Margins are service margins, not software margins.** I estimate the direct cost of one package at **€1.8–2.4k** with human translation (*my math*, section 7). At €3,500 the gross margin is 31–50 %; at €6,000 it is 60–71 %. No source shows anyone paying €6,000 for this `[UNVERIFIED]`.
- **Recommendation: do not found this as the main venture. Keep it as a side option (option b in task C28).** If you want a real-world signal, the cheapest test is a **€0 quality test this month** plus **5 phone or event conversations with DACH small sponsors and CROs** (outward, needs your OK). Kill the idea if none of them has paid an outside firm ≥€2,500 for a lay summary (section 12). The test also helps the spin-out route: it gives you something concrete to talk about with trial people.

## 1. One-liner
Small and mid-size drug companies (and the CROs that run their trials) must publish a plain-language results summary for every EU trial, usually in several languages, within 12 months, without in-house plain-language writers. We deliver an AI-drafted, medical-writer-checked lay summary plus translations as a fixed-price pack, ready to upload to CTIS, so that they file on time at a lower cost.

## 2. Problem evidence
**Hard data**
| What | Number | Source | Grade |
|---|---|---|---|
| Legal duty | Sponsor submits a results summary "accompanied by a summary written in a manner that is understandable to laypersons" within one year of trial end; content fixed in Annex V (10 items, incl. "Description of adverse reactions and their frequency", "Overall results") | [Regulation 536/2014](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) | [A] |
| Translations | "While the EU CTR does not request translations", the expert group suggests "as a minimum" the local language(s) of each trial country | [GLSP, EudraLex Vol. 10, 2021](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) | [A] (guidance, >3 years old) |
| Cost drivers | "The major costs will account for staff or contractors for the production and translation of the lay summary" | same GLSP | [A] |
| Effort today | "between 35 to 105 hours" per lay summary (workshop Feb 2022); a vendor says "approximately 20 hours per document" manually (Oct 2023) | [EFGCP/EFPIA report](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf); [TranspariMED quoting TrialAssure](https://www.transparimed.org/single-post/pls-automated) | [B] (both >3 years old for the first; vendor claim for the second) |
| Volume | 1,826 EU trials ended in 2025; 702 by small/mid companies, 590 by top-50 pharma, 534 non-commercial | own count (method in section 5) | [A, own count] |
| Translation practice | 75 % (372/495) of German-run multi-country trials with a lay summary include a German version; median 5 lay-summary documents per EU multi-country trial | C19, re-counted by the critic | [A, own count] |
| Compliance today | Results reported by the deadline: all trials 77.3 %, commercial 83.8 %, non-commercial 58.3 %; overdue and not reported: 9.4 % / 5.9 % / 19.5 % (data to 30 Sep 2026; deadline = later of legal deadline and sponsor's justified date) | [ACT EU KPI report Jul–Sep 2026](https://accelerating-clinical-trials.europa.eu/document/download/1271bfdd-8830-479c-8e3a-2ada45477c30_en?filename=ACT%20EU%20KPI%20Report_September_2026.pdf) | [A] |
| Fine in Germany | up to €25,000 for a late or missing Art. 37(4) document (§ 97 AMG) | [buzer.de](https://www.buzer.de/97_AMG.htm) (via C19) | [A] |

*Note:* EMA's 9.4 % overdue is lower than C19's own count (21 % missing). EMA uses each sponsor's justified later date, which the public data do not show (C19 limit (a)). Use EMA's figure from now on.

**Online voices [C]: weak.** 0 threads opened. Reddit is blocked and only reachable through mirrors, which `lessons.md` says not to use. One search snippet of a r/RegulatoryClinWriting post (mirror, not opened) said lay summaries are "low-hanging fruits" for AI but free tools "do not provide high quality summaries" `[UNVERIFIED]`. The practitioner voice comes from industry groups instead: a sponsor-and-vendor working group (Biogen, AstraZeneca, Merck KGaA, UCB, CSL Behring, CISCRP and others) formed "in response to the challenges faced by the industry in late 2023, beginning of 2024" with AI-written summaries ([Applied Clinical Trials/Informa](https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results)) [B]. A language company reports that "translation services have approximately one day, to translate an unknown quantity into an unknown number of languages" during CTIS requests ([RWS, sponsored article, Oct 2022](https://www.pharmaceutical-technology.com/sponsored/lay-of-the-land-understanding-lay-summary-requirements-and-the-challenges-they-bring/)) [B, vendor, >3 years old].

**Why now**
- EMA began publishing compliance figures in Sep 2026 [A] (above). After a letter from 20 health groups, it now sends reminders and shows national regulators which of their trials are overdue ([TranspariMED, 9 Jul 2026](https://www.transparimed.org/single-post/european-medicines-agency-takes-rapid-action-on-missing-clinical-trial-results); [17 Nov 2026](https://www.transparimed.org/single-post/european-medicines-agency-takes-multiple-steps-to-improve-clinical-trial-reporting)) [B].
- The same groups wrote to BfArM on 15 Jun 2026 asking how it enforces results reporting. They count 9 of 30 BfArM-supervised trials (30.0 %) without results as of Nov 2025 ([letter, PDF](https://bukopharma.de/wp-content/uploads/2026/06/CTIS-legal-violations-in-Germany_2026.pdf)) [B, advocacy].
- **UK:** for trials submitted from **28 Apr 2026**, participants "must be offered a summary of the trial's results in a way that can be understood by members of the public" within 12 months of trial end ([HRA](https://www.hra.nhs.uk/planning-and-improving-research/policies-standards-legislation/clinical-trials-investigational-medicinal-products-ctimps/clinical-trial-regulations-reform/guidance-on-changes-to-the-clinical-trials-regulations/research-transparency-requirements-for-clinical-trials/offering-to-share-a-summary-of-results-with-participants)) [A]. *Inference:* the first UK summaries under this rule fall due from about 2027–2028, once these trials have ended.
- LLMs now draft plain-language text at human quality in controlled tests (section 8) [A].

## 3. Customer
| Role | Who | Evidence |
|---|---|---|
| User | Clinical-trial transparency / disclosure lead or medical writer at the sponsor; at small biotechs, clinical operations or regulatory staff | Working-group roles: "Clinical Trial Transparency Lead, Biogen", "Senior Expert Clinical Trial Transparency, Merck Healthcare KGaA" ([CISCRP/EMWA paper, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf)) [B] |
| Buyer (signs) | Sponsor, directly (budget: trial close-out) **or** the CRO running the trial, which buys in a subcontractor | The sponsor carries the legal duty (Art. 37(4) CTR [A]). CISCRP says "most research sites and sponsors choose to work with an independent third-party" ([CISCRP, 2018](https://legacy.ciscrp.org/?p=9491)) [B, >3 years old]. One CRO (MMS) partnered with an AI vendor to produce PLS drafts ([Applied Clinical Trials, 3 Aug 2023](https://appliedclinicaltrialsonline.com/view/trialassure-announces-ai-generative-text-partnership-with-mms)) [B] |
| Payer | Sponsor (the CRO passes the cost on) | *inference* |

**Who the sponsors are: own count, trials that ended in 2025 [A, own count]** (method in section 5)

| Group | Trials | Sponsors | Trials naming a large CRO as contractor | Seat of sponsor |
|---|---|---|---|---|
| Top-50 pharma groups | 590 | 69 | 356 (60 %) | US 217, DE 99, CH 72 |
| Small and mid-size companies | 702 | 476 (367 with one trial) | 330 (47 %) | **US 262**, ES 62, **DE 43**, FR 35, CH 33 |
| – of which US-based | 262 | 175 | **186 (71.0 %)** | |
| – of which EU/EEA-based | 315 | 210 | 85 (27.0 %) | |
| – of which Germany-based | 43 | 30 | 13 (30.2 %) | 15 trials from Bavaria, 10 from greater Munich |
| Non-commercial | 534 | 293 | 23 (4 %) | FR 128, NL 81, ES/DE 51 each |

- "Large CRO" = contractor name matches IQVIA, ICON, PPD, Syneos, Parexel, Medpace, Fortrea/Covance, PRA, PSI, Worldwide, Premier, Novotech and similar (list in the script notes, section 5). Contractors are recorded at authorisation, so this shows who runs the trial, not who writes the lay summary. Only **3** of 3,388 trials name a contractor whose recorded task mentions "lay".
- **First target segment (inference):** DACH-based small and mid-size companies with a trial that ended in the last 12 months. That is **114 trials from 80 companies** that ended Jan–mid-Nov 2026, **107** of them with no public lay summary yet [A, own count]. Caveat: summaries of adult Phase I trials are published only 30 months after the end (EMA, via C19), so some "missing" ones are filed but hidden.
- Germany-based names with a 2026 trial and no public summary yet include CureVac, Immunic, Formycon, CatalYm, AiCuris, Heidelberg Pharma, Pentixapharm, Dr. Falk, Medac, Merz and Grünenthal (40 companies, public CTIS data). Five of the German "sponsors" are themselves CROs or contract-research firms acting as sponsor (CCDRD, SocraTec, Winicker-Norimed, GCP-Service, Charité Research Organisation). They are possible channel partners.
- **Decision process (inference, not sourced):** at small companies, one clinical-operations or regulatory manager signs a small purchase order at close-out. At US biotechs, the CRO's project manager adds a line item or names a preferred vendor. Large pharma use framework contracts with CROs and language companies (Lionbridge case study: a "global biopharma" buys lay-summary translations centrally, [Lionbridge, 2022](https://www.lionbridge.com/content/dam/lionbridge/pages/case-studies/global-biopharma-company-case-study/global-biopharma-company-case-study-english.pdf) [B]); a newcomer cannot get into these.

## 4. Solution & product wedge
- **Smallest product:** a fixed-price pack per trial. (1) An AI first draft of the CTR Annex V lay summary in English from the sponsor's results summary / CSR synopsis. (2) A review by a medical writer (accuracy, non-promotional tone, readability). (3) Machine translation into the trial-country languages, post-edited by native medical translators (DE and PT in-house via the network; others bought in). (4) CTIS-ready PDFs with a short AI-use and QC record. Turnaround target: 10 working days `[UNVERIFIED]`, not benchmarked.
- **What AI does:** extract the Annex V items from tables, draft at a set reading level using the sponsor's glossary and template, check numbers against the source and flag differences for the writer, and make translation first drafts. The workflow follows the CISCRP/EMWA model: "Initial Draft Creation (Human and AI involvement)" → "Human Refinement" → "quality control (QC) and compliance check" ([CISCRP/EMWA, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf)) [B].
- **Non-goals:** no full results summary or CSR writing (that is CRO and regulatory-writer work); no self-serve SaaS for large pharma (Weave Bio, Peer AI, TrialAssure already sell that); no patient-panel testing in version 1 (GLSP calls user testing "not mandatory" [A]); no overdue-rescue campaign (C19: pool too small).

## 5. Market size
**Method (re-runnable) [A, own count, 2026-11-19]:** `POST https://euclinicaltrials.eu/ctis-public-api/search` with `searchCriteria: {"status":[8]}` ("Ended"), 100 per page, sorted by `decisionDate` both ways → **4,202** ended trials. Year = last 4 characters of `endDateEU`: 2025 = **1,826** (matches C19), 2026 to date = 1,562. Each of the 3,388 trials was read with `GET /ctis-public-api/retrieve/<ctNumber>`. Sponsor = `authorizedPartI.sponsors[primary]`; commercial = sponsor field `isCommercial`; seat = `addresses[0].address.countryName`; top-50 = name keyword list as in C19 plus Hexal, Principia, Tesaro, MyoKardia, Otsuka, Regeneron, Bausch (590 vs C19's 585); contractors = `thirdParties[].organisationAddress.organisation.name`; trial countries = `authorizedApplication.memberStatesConcerned`; lay summary = `results.laypersonResults` or a document labelled "Laypersons summary".

| Level | Trials / year | × price | Value / year | Basis |
|---|---|---|---|---|
| TAM: every EU trial buys one pack | 1,826 | €6,000 | **€11.0m** | *my math* (1,826 × 6,000 = 10,956,000) |
| SAM: small and mid-size companies, EU-wide | 702 | €6,000 | **€4.2m** | 702 × 6,000 = 4,212,000 |
| SOM, direct only: DACH-based small/mid companies | 81 | €6,000 | **€486k** | 81 × 6,000 |
| SOM, direct only: Germany-based | 43 | €6,000 | **€258k** | 43 × 6,000 |
| Upside not counted | UK trials from 2027–28; lay protocol synopses at application (vendor claim, [Excelya, Nov 2024](https://excelya.com/wp-content/uploads/2024/11/Lay-Summaries-for-Clinical-Trials.pdf) [B]; not checked in CTIS rules `[UNVERIFIED]`) | | | |

- €6,000 is C19's assumed mid-point, built from labour value (€2,877–8,631 per lay summary + translations), **not an observed price** `[UNVERIFIED]`. At €3,500 (section 7), every value above falls by 42 %.
- **Packages needed (*my math*):**

| Target | at €3,500 | at €6,000 | Share of the 702 small/mid trials |
|---|---|---|---|
| €360k revenue (three salaries, C19 basis; ignores direct costs) | 103 | 60 | 15 % / 8.5 % |
| €360k **contribution** after direct costs (mid €2.1k a pack) | 257 (€1.4k each) | 92 (€3.9k each) | 37 % / 13 % |
| €1m revenue | 286 | 167 | 41 % / 24 % |

- *Inference:* even the best case needs about one in four small-company trials EU-wide, more than half of them from outside DACH and mostly through CROs. That is a niche service firm, not a venture-scale market.

## 6. Competitors
| Company | URL | Offering | Pricing | Funding | Gap we exploit |
|---|---|---|---|---|---|
| TrialAssure (US) | trialassure.com | Disclosure software; LINK AI drafts PLS; ~50,000 AI summaries published 2023 (later criticised, see section 8); CRO partnership with MMS | Not public | Private | Software for disclosure teams; small sponsors need the finished document |
| Weave Bio (US) | weave.bio | "AI-native regulatory platform"; NDA workflow with Parexel and Takeda deal (snippets only `[UNVERIFIED]`) | Not public | $20m Series A, $36m total (Oct 2025) ([Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development)) [B] | Focus on large regulatory dossiers, not lay summaries (no PLS product found) |
| Peer AI (US) | — | AI for protocols, CSRs | Not public | $12.1m [B] (C19) | Same |
| Yseop (FR) | yseop.com | Generative AI for clinical reports, ">150 trials" | Not public | Novartis dRx, Lilly [B] (C19) | Same |
| Carelane (Berlin) | htgf.de | AI end-to-end trial platform incl. medical writing; ">130 research sites" | Not public | €2.6m seed, Apr 2025 (Vorwerk Ventures, HTGF) ([HTGF](https://www.htgf.de/carelane-seed/)) [B] | Platform for running trials, not a disclosure service |
| CROs: Quanticate, Clinbay, Excelya, Certara/Synchrogenix ("over 200 PLS", snippet) | various | Lay summaries + translations as a service | "cost-effective" (Clinbay), no prices | Private / listed | They are the channel as much as the competition; small CROs may white-label |
| CISCRP (US non-profit) | ciscrp.org | Full-service or editorial-review lay summaries ([CISCRP, 2020](https://legacy.ciscrp.org/making-it-clear-lay-language-summaries/)) [B] | Not public | Non-profit | US-centred, English-first |
| SciencePOD (Dublin) | sciencepod.net | PLS incl. "AI-Hybrid content, where a first draft is generated by AI tools and then complemented by quality checks from a human editor" ([SciencePOD, 2024](https://sciencepod.net/?p=380039)) [B] | Not public | Small firm | Same model as ours already on offer |
| Language companies: RWS, Lionbridge, TransPerfect | — | Lay-summary creation and translation for big pharma | Not public | Listed / large | Framework contracts with large pharma; not set up for one-trial biotechs |
| Indegene + Trilogy Writing (Frankfurt) | — | Medical writing with "Generative AI" (acquired Mar 2024) [B] (C19) | Not public | Listed group | German-based competitor with the same pitch |

*Inference:* the exact model (AI draft + human check + translation) is already offered by at least one small firm (SciencePOD) and by CROs. Our only edge would be price and speed for DACH/PT small sponsors, plus German and Portuguese in-house. That edge is copyable.

## 7. Business model & pricing
- **Model:** fixed price per trial pack, sold directly or white-labelled to CROs (CRO margin on top). Optional yearly bundle for sponsors with several trials.
- **Price hypothesis:** **€3,500** for EN + up to 4 languages (below C19's €5–12k labour value, to undercut CROs); **€6,000** with patient-panel review and graphics. Both are `[UNVERIFIED]` (no observed price, 10+ searches in C19, 6 more here; TED: 0 lay-summary tenders). Benchmarks: US university results-posting service $1,000–2,500 (UCLA) [B]; patient-panel review "$3,000 to $3,500" (Citeline, snippet only, page 404) `[UNVERIFIED]`.
- **Direct cost per pack (*my math*, assumptions marked):**
  - Writer time: manual "approximately 20 hours", AI "less than one day" (TrialAssure claim [B]); AI saved writers ">40 %" of drafting time in a study ([JAMIA Open 2025, PMID 40183004](https://europepmc.org/article/MED/40183004)) [A]. Assume 8–20 h per pack.
  - Writer cost: Medical Writer average **€55,400 gross a year** in Germany (range €46,500–65,100; [StepStone](https://www.stepstone.de/gehalt/Medical-Writer.html), undated, read 2026-11-19) [B]. With ~21 % employer costs `[UNVERIFIED assumption]` ≈ €67k. Assume 1,600 productive hours a year `[UNVERIFIED assumption]` → 80–200 packs per writer → **€335–838** per pack (67,000 / 200 and / 80).
  - Translation: 4 languages at the German court rate, ~€355–391 each for ~10,000 characters (C19, length assumed) → **€1,420–1,564**. AI pre-translation plus post-editing could lower this; not sourced.
  - **Total ≈ €1,755–2,402** (335 + 1,420; 838 + 1,564). Gross margin at €3,500: 31–50 %; at €6,000: 60–71 %.
- *Inference:* service margins and one-off buys per customer (367 of 476 small sponsors had one ending trial in 2025). Grows with headcount, not software. VC investors look for software-like margins; this gets there only if writer time falls well below 8 h, which nobody shows with real CTR documents yet.

## 8. Regulation & data
| Topic | Rule | What it means for us | Source |
|---|---|---|---|
| Content | Annex V CTR, 10 items | Fixed template; good for AI | [CTR](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) [A] |
| Tone | LS must be "non-promotional"; review by "patient(s), medical monitor, statistician" recommended; user testing "not mandatory" | Writer review is the core of the offer; promotional slip = sponsor risk | [GLSP](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) [A] |
| AI use by regulators' standard | AI "used for drafting, compiling, editing, translating … medicinal product information documents should be used under close human supervision … quality review mechanisms need to be in place" (about product information, the closest EMA text found) | Human QC is expected, not optional | [EMA reflection paper, Sep 2024](https://www.ema.europa.eu/en/documents/scientific-guideline/reflection-paper-use-artificial-intelligence-ai-medicinal-product-lifecycle_en.pdf) [A] |
| EU AI Act Art. 50(4) | Deployers of AI that generates text "published with the purpose of informing the public on matters of public interest shall disclose" it, **unless** it "has undergone a process of human review or editorial control" with a person holding "editorial responsibility"; Art. 50 applies from 2 Aug 2026 | With documented writer review and sponsor sign-off, disclosure is not required by law, but the CISCRP group and 62.4 % of patients want it anyway | [AI Act text, Art. 50](https://artificialintelligenceact.eu/article/50/), [Art. 113](https://artificialintelligenceact.eu/article/113/) [B, secondary copy of the law]; [JMIR AI 2026, PMID 42330509](https://europepmc.org/article/MED/42330509) [A] |
| Industry practice | "Standalone use of AI for creating LS concerns clinical trial sponsors"; in 2023 "publicly posted, AI-generated LS that lacked proper human oversight … were eventually removed" | Buyers will audit the QC step | [CISCRP/EMWA paper, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) [B] |
| AI quality evidence | ChatGPT-4o PLS scored 1 point higher on information and 2 points higher on readability than Cochrane human PLS (36 summaries, blinded RCT); GPT-4 lay summaries more readable than originals (204 articles); but in a crowdsourced test (150 readers) "human-written PLSs lead to significantly better comprehension" | Drafts are good; comprehension still needs a human | [Cochrane Evid Synth Methods 2025, PMID 40727555](https://europepmc.org/article/MED/40727555) [A]; [JMIR 2025, PMID 41259712](https://europepmc.org/article/MED/41259712) [A]; [arXiv 2505.10409, May 2025](https://arxiv.org/abs/2505.10409) [B, preprint] |
| Patient trust | Trust "a lot": AI-only documents 12.3 %, human-only 39.1 %; 95.0 % want human review (n = 1,010, EU + US) | Sell "human-checked", not "AI-written" | [JMIR AI 2026, PMID 42330509](https://europepmc.org/article/MED/42330509) [A] (authors from CISCRP, a lay-summary provider) |
| Data protection | Inputs should use aggregated data; "organizations must ensure that AI models are not retaining sensitive information" | Lay summaries use aggregate results, so little personal data (*inference*). Unpublished results are confidential: EU-hosted model, no training on client data, NDA + data processing agreement | [CISCRP/EMWA](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) [B] |
| MDR / DiGA | Not applicable: documents for the public, no medical purpose for a patient (*inference*) | No certification needed | — |
| Marketing in Germany | Email advertising needs "vorherige ausdrückliche Einwilligung" of the addressee; phone calls to businesses need "zumindest mutmaßliche Einwilligung" | No cold emails to sponsors; use calls, events, CRO partners | [§ 7 UWG](https://www.buzer.de/7_UWG.htm) [A] |

- **Certifications:** none required by law. Language firms advertise ISO 17100 for translation ([Translated](https://translated.com/resources/medical-translation-services-pricing-healthcare-documentation-cost-analysis)) [B]; large sponsors may ask for it in vendor audits `[UNVERIFIED]`. Professional liability insurance: cost not checked `[UNVERIFIED]`.
- **Time and cost to compliance (inference):** weeks, not months: written SOPs for AI use and QC, an EU-hosted LLM contract, NDA/DPA templates. No regulator approval.

## 9. Go-to-market
- **First 10 customers (inference):** from the public CTIS list of the 80 DACH-based small/mid companies with a 2026 trial and no summary yet (section 3), start with the 10 in greater Munich (e.g., Formycon, CatalYm, Immunic, Dermapharm, Nucleus Medical) and the German contract-research firms that act as sponsors (CCDRD, SocraTec, Winicker-Norimed, GCP-Service) as white-label partners.
- **Channels:** phone and events, not cold email (§ 7 UWG [A]). BioM/BayStartUP life-science events in Munich (repo `research/munich-ecosystem.md`) [B]; DIA Europe 2027, Basel, 16–18 Mar 2027 [B] (C19); EMWA conferences for writers and partners [B] (C19).
- **Pilot design:** one real trial, fixed price (e.g. €2,500 for an EN summary + German version), delivery within 10 working days. Success = sponsor files it in CTIS unchanged except for wording, and agrees to be a reference.
- **CRO route:** offer a white-label rate to 2–3 small DACH CROs. US biotechs are reached only through CROs (71 % name a large CRO [A, own count]), and large CROs have in-house teams or partners (MMS–TrialAssure [B]).

## 10. Funding path
- **Grants now: none fit while you are employed.** EXIST-Gründungsstipendium excludes an active job (side work ≤20 h a month) and must be filed by a German university; FLÜGGE requires membership of the applying Bavarian university (via repo `research/munich-ecosystem.md`, fact-checked) [A]. From Sep 2027: EXIST through a host university (SCE/HM, TUM, LMU) is possible if the CEO has left his job or is on a sabbatical, and the team has a graduate medical writer (via repo) [A].
- **Investors:** HTGF and Vorwerk Ventures funded an AI trial platform with medical writing (Carelane, €2.6m seed, 2025) [B]. *Inference:* a service pack with 31–71 % gross margin will not fit a seed fund. The realistic path is to bootstrap: €10k own money covers the LLM setup and a first freelance writer for 2–3 pilots (*my math:* 3 packs × ~€2.1k direct cost = €6.3k).
- **Capital to first revenue (inference):** <€10k if a pilot customer pays on delivery. No outside capital until there is repeat demand.

## 11. Team
- **Must have: a medical-writer co-founder** with CTR lay-summary experience, German + English, ideally Portuguese. This covers the CEO's main gap (no clinical or medical-writing background, `founder-brief.md`). Without one, every pack depends on freelancers bought at €82.2/h (EMWA median [B], C19), and the margin is gone.
- **Where to find one:** EMWA (membership "over 1,000" per a search snippet `[UNVERIFIED]`); StepStone lists **228** Medical Writer ads and names Berlin, Hamburg and **München** as cities with many openings ([StepStone](https://www.stepstone.de/gehalt/Medical-Writer.html)) [B]; Lisbon: a Hays ad "Scientific Communication & Medical Writer (M/F/D)", Grande Lisboa (title only seen) [C], and German-language scientific-communications roles in Lisbon (search snippets only) `[UNVERIFIED]`.
- **Optional later:** native translators/reviewers for PT and DE (Lisbon network); an engineer for the document pipeline (the CEO's AI-agent skills cover a first version, *inference*).

## 12. Risks & kill criteria (pre-mortem by the researcher; critic red team still to come)
| Riskiest assumption | Evidence so far | How to test | Kill if |
|---|---|---|---|
| R1. Small sponsors pay outside firms ≥€2,500 per lay summary pack | None observed; labour value €2.9–8.6k (C19 math); vendors publish no prices | 5–10 calls with DACH small sponsors / CROs: "Who wrote your last lay summary, what did it cost, who signed?" | **Fewer than 2 of the first 5 conversations** report an outside purchase ≥€2,500, or most say "the CRO includes it" with no separate price |
| R2. Enough reachable volume | DACH-based small/mid: 81 trials / 63 sponsors in 2025 [A, own count]; €1m needs 167–286 packs | Ask 2–3 small CROs for a white-label volume estimate | No CRO will name ≥20 packs a year at ≥€2,000 |
| R3. AI draft + human check takes ≤8 h of writer time | Vendor: "less than one day" [B]; study: >40 % saving on abstracts [A]; no data on real CTR documents | €0 quality test (section 13, step 1) | Writer time >15 h per pack in the test, or the AI draft has a factual error the writer misses |
| R4. A medical-writer co-founder joins | 228 DE job ads show demand and competition for writers [B]; none approached | EMWA/LinkedIn search after the CEO's OK | No candidate willing to talk by **31 Mar 2027** |
| R5. Incumbents do not cut prices with AI | SciencePOD already sells an AI-hybrid PLS [B]; Indegene/Trilogy add GenAI [B] | Price question in the R1 calls | A CRO or language firm quotes <€1,500 for the same pack |

- **Overall kill line (proposal):** if R1 fails, or R1 passes but R2 shows <20 packs a year within reach, drop the idea as a company. At most keep it as a freelance side service.
- **Pre-mortem (inference):** the most likely way this fails is "nobody objects, nobody buys". Sponsors say lay summaries are a pain, but the CRO already bundles them into the trial budget. No separate purchase decision exists for a newcomer to win.

## 13. Validation plan
1. **€0 quality test (desk, no outward action; CEO or researcher, 1 evening):** take 3 public CTIS trials that already have an English and a German lay summary. Generate a draft from the public results summary only, then compare it with the sponsor's published version on the 10 Annex V items: errors, missing items, reading level. Pass: 0 factual errors and ≤2 missing items per summary.
2. **5–10 interviews (outward; needs your approval).** Who: 3 DACH small-sponsor clinical-ops or regulatory leads (Munich list in section 9); 2 small CRO project leads (CCDRD, SocraTec, Winicker-Norimed); 1–2 freelance medical writers (cost check and co-founder search). Route: phone, BioM events, DIA Europe; no cold email (§ 7 UWG).
   - Questions (Mom Test): "Tell me about the last lay summary you filed. Who wrote it? How long did it take? What did it cost, and from which budget? Which languages, and who translated? What went wrong? Did your CRO quote it separately?"
   - **Confirms:** ≥2 of 5 name an outside purchase ≥€2,500 and a separate budget line; ≥1 agrees to a paid pilot.
   - **Kills:** see R1/R2. Wording fixed now, before any calls.
3. **Timing (inference):** step 1 in December 2026; step 2 alongside the spin-out events (Jan–Mar 2027) so it costs no extra trips. Decide by 31 Mar 2027, the same date as the EXIST-Forschungstransfer cut-off.

## Gaps / [UNVERIFIED]
- No observed price for a lay summary or pack (16+ searches across C19 and C25; TED 0). €3,500 and €6,000 are hypotheses.
- Who signs in practice (sponsor vs CRO) is inferred from contractor lists and a 2018 CISCRP statement, not from a survey; none was found.
- Writer hours with AI on real CTR documents: no data; 8–20 h is an assumption from a vendor claim and a study on abstracts.
- Employer-cost add-on (21 %), 1,600 productive hours, lay-summary length (10,000 characters): assumptions.
- Weave Bio–Parexel/Takeda, Certara "200 PLS", EMWA membership size, Lisbon German-language writer roles, the Reddit post: search snippets only.
- Large-CRO keyword list may miss smaller CROs, so "naming a large CRO" understates CRO use, mainly for EU-based sponsors.
- AI Act text read from a secondary site (EUR-Lex returned an empty page to curl).
- Lay protocol synopsis as a second paid document: vendor claim only.

## Sources
- https://euclinicaltrials.eu/ctis-public-api/search and https://euclinicaltrials.eu/ctis-public-api/retrieve/<ctNumber> — own count: 4,202 ended trials; 3,388 ended 2025–2026 read one by one; sponsor seat, CRO contractors, lay-summary status; accessed 2026-11-19
- https://accelerating-clinical-trials.europa.eu/document/download/1271bfdd-8830-479c-8e3a-2ada45477c30_en?filename=ACT%20EU%20KPI%20Report_September_2026.pdf — EMA/ACT EU compliance 77.3 / 83.8 / 58.3 %, overdue 9.4 / 5.9 / 19.5 %; accessed 2026-11-19
- https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf — Art. 37(4), Annex V CTR; accessed 2026-11-19
- https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf — translations recommended, cost drivers, review, non-promotional; accessed 2026-11-19
- https://www.ema.europa.eu/en/documents/scientific-guideline/reflection-paper-use-artificial-intelligence-ai-medicinal-product-lifecycle_en.pdf — "close human supervision" for AI drafting (Sep 2024); accessed 2026-11-19
- https://artificialintelligenceact.eu/article/50/ and https://artificialintelligenceact.eu/article/113/ — AI Act Art. 50(4) text and 2 Aug 2026 application date (secondary copy); accessed 2026-11-19
- https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf — CISCRP/EMWA AI working group: human oversight, 2023 removal, roles, workflow (Medical Writing, Jun 2025); accessed 2026-11-19
- https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results — working group formed after "challenges faced by the industry in late 2023"; accessed 2026-11-19
- https://www.transparimed.org/single-post/pls-automated — TrialAssure ~50,000 AI PLS, "approximately 20 hours per document", "less than one day" (24 Oct 2023); accessed 2026-11-19
- https://www.transparimed.org/single-post/european-medicines-agency-takes-rapid-action-on-missing-clinical-trial-results — EMA reminders and national monitoring (9 Jul 2026); accessed 2026-11-19
- https://www.transparimed.org/single-post/european-medicines-agency-takes-multiple-steps-to-improve-clinical-trial-reporting — EMA KPIs, reminders (17 Nov 2026); accessed 2026-11-19
- https://bukopharma.de/wp-content/uploads/2026/06/CTIS-legal-violations-in-Germany_2026.pdf — letter to BfArM, 9 of 30 trials without results (15 Jun 2026); accessed 2026-11-19
- https://www.hra.nhs.uk/planning-and-improving-research/policies-standards-legislation/clinical-trials-investigational-medicinal-products-ctimps/clinical-trial-regulations-reform/guidance-on-changes-to-the-clinical-trials-regulations/research-transparency-requirements-for-clinical-trials/offering-to-share-a-summary-of-results-with-participants — UK lay-results duty from 28 Apr 2026; accessed 2026-11-19
- https://europepmc.org/article/MED/40727555 — Cochrane RCT, ChatGPT-4o vs human PLS (2025); accessed 2026-11-19 (abstract via Europe PMC REST)
- https://europepmc.org/article/MED/41259712 — ChatGPT-4 lay summaries, 204 prostate-cancer articles (JMIR 2025); accessed 2026-11-19 (abstract)
- https://europepmc.org/article/MED/40183004 — bespoke AI saved writers >40 % time on PLS abstracts (JAMIA Open 2025); accessed 2026-11-19 (abstract)
- https://europepmc.org/article/MED/42330509 — patient trust in AI documents, n = 1,010 (JMIR AI 2026); accessed 2026-11-19 (abstract)
- https://arxiv.org/abs/2505.10409 — crowdsourced comprehension, human PLS better understood (preprint, May 2025); accessed 2026-11-19
- https://legacy.ciscrp.org/?p=9491 — "most research sites and sponsors choose to work with an independent third-party" (2018); accessed 2026-11-19
- https://legacy.ciscrp.org/making-it-clear-lay-language-summaries/ — CISCRP full-service vs editorial-review models (2020); accessed 2026-11-19
- https://appliedclinicaltrialsonline.com/view/trialassure-announces-ai-generative-text-partnership-with-mms — CRO MMS + TrialAssure AI PLS drafts (3 Aug 2023); accessed 2026-11-19
- https://www.pharmaceutical-technology.com/sponsored/lay-of-the-land-understanding-lay-summary-requirements-and-the-challenges-they-bring/ — RWS sponsored article, translation turnaround pain (28 Oct 2022); accessed 2026-11-19
- https://www.lionbridge.com/content/dam/lionbridge/pages/case-studies/global-biopharma-company-case-study/global-biopharma-company-case-study-english.pdf — lay-summary translation for a global biopharma (Sep 2022); accessed 2026-11-19
- https://sciencepod.net/?p=380039 — SciencePOD AI-Hybrid PLS (2024); accessed 2026-11-19
- https://www.htgf.de/carelane-seed/ — Carelane €2.6m seed, Vorwerk + HTGF (Jul 2025); accessed 2026-11-19
- https://excelya.com/wp-content/uploads/2024/11/Lay-Summaries-for-Clinical-Trials.pdf — CRO lay-summary service; lay protocol synopsis claim (Nov 2024); accessed 2026-11-19
- https://www.stepstone.de/gehalt/Medical-Writer.html — Medical Writer salary €55,400 average, 228 ads; accessed 2026-11-19
- https://www.buzer.de/7_UWG.htm — § 7 UWG consent rules for email and phone advertising; accessed 2026-11-19
- https://translated.com/resources/medical-translation-services-pricing-healthcare-documentation-cost-analysis — ISO 17100 cited by a language firm; accessed 2026-11-19
- https://expressoemprego.pt/emprego/scientific-communication---medical-writer-(m-f-d)/grande-lisboa/2434256 — Hays ad title, Lisbon medical writer (title only); accessed 2026-11-19
- Via repo (C19, fact-checked 2026-11-19): EFGCP/EFPIA 35–105 h; EMWA €82.2/h; UCLA fees; JVEG €1.95; § 97 AMG; Weave Bio, Peer AI, Yseop, Indegene/Trilogy, Quanticate, Clinbay; DIA Europe 2027. Via repo `research/munich-ecosystem.md` (fact-checked): EXIST and FLÜGGE eligibility, HTGF/Bayern Kapital.
