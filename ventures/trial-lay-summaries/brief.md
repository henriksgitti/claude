# Venture brief: AI-drafted, human-checked lay summary + translation pack for trial sponsors
Task: C25, revised in C29 + C30 (the brief's one fix round, rule 14) | Date: 2026-11-19 | Status: draft, fact-checked and red-teamed; fixes applied (log at the end) | Score: not scored (variant of direction 1 in `research/new-directions.md`; no scoring run for it)

Builds on `research/direction1-trial-summaries.md` (C19, fact-checked in `research/reviews/2026-11-19-direction1-trial-summaries.md`). Reviews applied: `research/reviews/2026-11-19-trial-lay-summaries-brief.md` (fact-check) and `research/reviews/2026-11-19-redteam-trial-lay-summaries-brief.md` (red team). New in the C30 run: a full re-count of the CTIS public data (4,202 ended trials; all 3,388 that ended in 2025–2026 read one by one, 2026-11-19) with the company and CRO lists written down (section 5), splits by trial phase and number of countries, and the two free desk checks T1 (who is named as writer in published lay summaries) and T2 (CRO share by number of trial countries). Grades per `CLAUDE.md` rule 2. *My math* and *inference* are labelled.

**Bottom line for the CEO (researcher's view; you decide):**
- **The job is real and required by law, but the market is small.** Every EU drug trial must publish a lay summary within 12 months of its end (Art. 37(4) and Annex V CTR [A]). **1,826** trials ended in 2025 [A, own count]. If every one bought a €6,000 pack (an assumed price, never observed), the whole market would be **€11.0m a year** (*my math*).
- **The part a newcomer could reach is about €0.6–1.1m a year EU-wide.** "Other companies" (not on the large-company list, section 5) ended **639** trials in 2025. Take out bioequivalence studies (61) and one-country Phase I studies (151), where a polished summary has little value, and **427** remain. Of these, **181** do not name a large CRO. At €3,500–6,000 a pack that is **€0.63–1.09m a year** for all of Europe and the US together (*my math*). For DACH-based companies it is **26 trials** a year (€91–156k) [A, own count].
- **The two free desk checks the critic set as the condition for keeping this open do not pass.**
  - **T2 (CRO share):** **77 %** (178 of 231) of the "other company" trials that run in 3 or more countries name a large CRO [A, own count]. These are the trials where a translation pack is worth most. This meets the critic's kill line (≥70 %): the valuable part of the market is CRO-bound.
  - **T1 (who wrote the published summaries):** in a fixed sample of 30 published summaries from EU/Swiss "other companies", **only 1** names an outside writing firm. 17 name nobody, and 3 are placeholder letters with no results. The other 9 show a CRO template or a CRO as sponsor (4), big-pharma group house style (1), the sponsor's own letterhead (1), or a document built by a script or AI tool (3). A wider sweep of all 165 such trials found an outside writer in **4** (two of them from one sponsor using one writing firm, one by the large CRO Syneos). It also found **6** summaries whose PDF files carry script or AI-tool traces. One of them is from a biotech in Martinsried (Munich), whose PDF author field reads "OpenAI" [A, own count; what the traces mean is *inference*]. By the critic's thresholds T1 is **inconclusive**: too few summaries name anyone. The signs that are there point to CROs, in-house writing and do-it-yourself AI, not to a market for outside writers.
- **The "late report" pressure is weaker than we assumed.** EMA's first official figures (Sep 2026) show company trials reporting results on time in **83.8 %** of cases; only **5.9 %** are overdue. These figures cover results reporting in general, not lay summaries alone [A]. The pain is workload and cost, not fines.
- **AI drafting is good enough to be a do-it-yourself tool, and buyers still want a human check.** In studies on Cochrane and journal summaries (none tested CTR lay summaries), AI drafts scored as well as or better than human drafts (Cochrane RCT, 36 summaries) [A]. In a separate crowdsourced test, "human-written PLSs lead to significantly better comprehension" (150 readers, preprint) [B]. In another study, writers saved >40 % of their time (10 writers, 6 journal abstracts) [A]. Only **12.3 %** of 1,010 patients trust AI-only documents "a lot" [A]. EMA wants AI-drafted product-information documents used "under close human supervision"; this is the closest EMA text found [A]. In 2023, a large set of publicly posted AI-written lay summaries was removed after accuracy concerns. The source names no vendor (CISCRP/EMWA 2025) [B].
- **You would be the least needed person in this business.** The work is a medical writer's work plus a general AI tool. An experienced writer with an LLM licence can sell this alone and keep the whole margin. You cannot deliver it alone. Any writer co-founder would have to accept a split in which your share is earned by sales and AI set-up (red team F2; *inference*).
- **Margins are service margins.** With the measured median summary length (11,799 characters), the direct cost of a pack in English plus 4 languages is **€2.0–2.7k** (*my math*, section 7). That gives a gross margin of **23–43 %** at €3,500 and **55–67 %** at €6,000.
- **Recommendation (changed from the C25 draft): (a) drop it as a venture, no outward steps.** The free desk checks were the gate for option (b), and they did not pass. Keep this file as reference for the spin-out route (it shows how CTIS data can be used). If you still pick (b): two warm-intro conversations only (one freelance medical writer, one small CRO's writing lead), with the pass and kill lines in section 13. No cold calls (section 8).

## 1. One-liner
Smaller drug companies and the CROs that run their trials must publish a plain-language results summary for every EU trial within 12 months, often in several languages. We deliver an AI-drafted, medical-writer-checked lay summary plus translations as a fixed-price pack, ready to upload to CTIS.

## 2. Problem evidence
**Hard data**
| What | Number | Source | Grade |
|---|---|---|---|
| Legal duty | Sponsor submits a results summary "accompanied by a summary written in a manner that is understandable to laypersons" within one year of trial end; content fixed in Annex V (10 items, incl. "Description of adverse reactions and their frequency", "Overall results") | [Regulation 536/2014](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) | [A] |
| Translations | "While the EU CTR does not request translations", the expert group suggests "as a minimum" the local language(s) of each trial country | [GLSP, EudraLex Vol. 10, 2021](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) | [A] (guidance, >3 years old) |
| Cost drivers | "The major costs will account for staff or contractors for the production and translation of the lay summary" | same GLSP | [A] |
| Effort today | "between 35 to 105 hours" per lay summary (workshop Feb 2022); a vendor says "approximately 20 hours per document" manually (Oct 2023) | [EFGCP/EFPIA report](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf); [TranspariMED quoting TrialAssure](https://www.transparimed.org/single-post/pls-automated) | [B] (first >3 years old; second a vendor claim) |
| Volume | 1,826 EU trials ended in 2025: 639 by "other companies", 653 by large pharma groups, 534 non-commercial (lists in section 5) | own count | [A, own count] |
| Length and languages | Published lay summaries of EU/Swiss "other companies": median **11,799 characters** (159 documents); median **4** lay-summary documents per multi-country trial (108 trials) | own count, section 5 | [A, own count] |
| Translation practice | 75 % (372/495) of German-run multi-country trials with a lay summary include a German version | C19, re-counted by the critic | [A, own count] |
| Compliance today | Results reported by the deadline: all trials 77.3 %, commercial 83.8 %, non-commercial 58.3 %; overdue and not reported: 9.4 % / 5.9 % / 19.5 % (data to 30 Sep 2026). Deadline = "the later of the expected submission date communicated by the sponsor and the relevant regulatory deadline"; covers results reporting in general, not lay summaries alone | [ACT EU KPI report Jul–Sep 2026](https://accelerating-clinical-trials.europa.eu/document/download/1271bfdd-8830-479c-8e3a-2ada45477c30_en?filename=ACT%20EU%20KPI%20Report_September_2026.pdf) | [A] |
| Fine in Germany | up to €25,000 for a late or missing Art. 37(4) document (§ 97 AMG) | [buzer.de](https://www.buzer.de/97_AMG.htm) (via C19) | [A] |

*Note:* EMA's 9.4 % overdue is lower than C19's own count (21 % missing). EMA uses the sponsor's communicated later date, which the public data do not show (C19 limit (a)). Use EMA's figure from now on.

**Online voices [C]: weak.** 0 threads opened. Reddit is blocked and only reachable through mirrors, which `lessons.md` says not to use. One search snippet of a r/RegulatoryClinWriting post (mirror, not opened) said lay summaries are "low-hanging fruits" for AI but free tools "do not provide high quality summaries" `[UNVERIFIED]`. The practitioner voice comes from industry groups instead. A sponsor-and-vendor working group formed "in response to the challenges faced by the industry in late 2023, beginning of 2024" with AI-written summaries ([Informa, with Biogen and AstraZeneca panellists](https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results)) [B]. Its members include Merck KGaA, UCB, CSL Behring and CISCRP ([CISCRP/EMWA paper, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf)) [B]. A language company reports that "translation services have approximately one day, to translate an unknown quantity into an unknown number of languages" during CTIS requests ([RWS, sponsored article, Oct 2022](https://www.pharmaceutical-technology.com/sponsored/lay-of-the-land-understanding-lay-summary-requirements-and-the-challenges-they-bring/)) [B, vendor, >3 years old].

**Why now**
- EMA began publishing compliance figures in Sep 2026 [A] (above). After a letter from 20 health groups, it now sends reminders and shows national regulators which of their trials are overdue ([TranspariMED, 9 Jul 2026](https://www.transparimed.org/single-post/european-medicines-agency-takes-rapid-action-on-missing-clinical-trial-results); [17 Nov 2026](https://www.transparimed.org/single-post/european-medicines-agency-takes-multiple-steps-to-improve-clinical-trial-reporting)) [B].
- The same groups wrote to BfArM on 15 Jun 2026 asking how it enforces results reporting. They count 9 of 30 BfArM-supervised trials (30.0 %) without results as of Nov 2025 ([letter, PDF](https://bukopharma.de/wp-content/uploads/2026/06/CTIS-legal-violations-in-Germany_2026.pdf)) [B, advocacy].
- **UK:** for trials submitted from **28 Apr 2026**, participants "must be offered a summary of the trial's results in a way that can be understood by members of the public" within 12 months of trial end ([HRA](https://www.hra.nhs.uk/planning-and-improving-research/policies-standards-legislation/clinical-trials-investigational-medicinal-products-ctimps/clinical-trial-regulations-reform/guidance-on-changes-to-the-clinical-trials-regulations/research-transparency-requirements-for-clinical-trials/offering-to-share-a-summary-of-results-with-participants)) [A]. *Inference:* the first UK summaries under this rule fall due from about 2027–2028, once these trials have ended.
- LLMs now draft plain-language text that scores at human level in controlled tests on journal and Cochrane summaries (section 8) [A]. The same fact makes do-it-yourself drafting by sponsors cheap (T1 below).

## 3. Customer
| Role | Who | Evidence |
|---|---|---|
| User | Clinical-trial transparency / disclosure lead or medical writer at the sponsor; at small biotechs, clinical-operations or regulatory staff | "Clinical Trial Transparency Lead, Biogen" ([Informa](https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results)) [B]; "Senior Expert Clinical Trial Transparency, Merck Healthcare KGaA" ([CISCRP/EMWA, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf)) [B] |
| Buyer (signs) | Most likely the **CRO**, inside the full-service contract signed at trial start; the sponsor directly only where no large CRO runs the trial | The sponsor carries the legal duty (Art. 37(4) CTR [A]). CISCRP says "most research sites and sponsors choose to work with an independent third-party" ([CISCRP, 2018](https://legacy.ciscrp.org/?p=9491)) [B, >3 years old]; a full-service CRO is such a third party. One CRO (MMS) partnered with an AI vendor to produce PLS drafts ([Applied Clinical Trials, 3 Aug 2023](https://appliedclinicaltrialsonline.com/view/trialassure-announces-ai-generative-text-partnership-with-mms)) [B]. T1: CRO templates and a CRO-written summary seen; outside writing firms rare (below) [A, own count] |
| Payer | Sponsor (the CRO passes the cost on) | *inference* |

**Who the sponsors are: own count, trials that ended in 2025 [A, own count]** (method and lists in section 5; "large CRO" excludes their central-lab entities)

| Group | Trials | Sponsors | Trials naming a large CRO | Seat of sponsor |
|---|---|---|---|---|
| Large pharma groups (list in section 5) | 653 | 90 | 364 (55.7 %) | US 238, DE 102, CH 75 |
| Other companies (not on the list; mostly small/mid, but includes established private firms such as Grünenthal, Merz, Medac, Dr. Falk, Dermapharm, Bionorica) | 639 | 455 (355 with one trial) | 252 (39.4 %) | **US 241**, ES 60, **DE 40**, FR 35, CH 30 |
| – of which US-based | 241 | 169 | **155 (64.3 %)** (161, 66.8 %, if central labs count) | |
| – of which EU/EEA-based | 295 | 200 | 48 (16.3 %) | |
| – of which Germany-based | 40 | 28 | 7 (17.5 %) | 13 trials from Bavaria, 11 from greater Munich (postcodes 80–82); 9 of the 40 are by contract-research firms acting as sponsor (CCDRD 8, Charité Research Organisation 1) |
| – of which DACH-based | 75 | 58 | 24 (32.0 %) | |
| Non-commercial | 534 | 293 | 10 (1.9 %) | FR 128, NL 81, ES/DE 51 each |

**Phase and number of countries, "other companies", 2025 (F3) [A, own count]**

| Phase | 1 country | 2 countries | 3+ countries | Total |
|---|---|---|---|---|
| Bioequivalence | 60 | 1 | 0 | 61 |
| Phase I (incl. first-in-human) | 151 | 25 | 14 | 190 |
| Phase II–IV and integrated I/II, II/III, III/IV | 107 | 64 | 217 | 388 |
| **Total** | 318 | 90 | 231 | 639 |

- *Inference:* bioequivalence summaries are near-identical across a generic maker's studies, and summaries of adult Phase I trials are published only after 30 months (EMA, via C19). Sponsors have little reason to pay for polish there. Taking out bioequivalence and one-country Phase I leaves **427** "core" trials.

**T2: large-CRO share by number of trial countries, "other companies" [A, own count]**

| Trial countries | 2025 | of which US-based | EU/EEA-based | DACH-based | 2025–26 combined |
|---|---|---|---|---|---|
| 1 | 39 / 318 (12.3 %) | 20 / 67 | 6 / 198 | 4 / 40 | 66 / 562 (11.7 %) |
| 2 | 35 / 90 (38.9 %) | 21 / 40 | 11 / 38 | 1 / 8 | 61 / 149 (40.9 %) |
| 3+ | **178 / 231 (77.1 %)** | 114 / 134 | 31 / 59 | 19 / 27 | 347 / 466 (74.5 %) |

- The critic's kill line for T2 was "≥70 % of 3+-country trials name a large CRO". **Met** (77.1 %). The list misses mid-size CROs, so the true CRO share is higher. EU-based sponsors are the exception (31 of 59, 53 %).
- Contractor lists do not show who writes the lay summary. Of 6,588 free-text duty entries in the contractor records of the 3,388 trials, **0** mention a lay summary. One published summary says it was "prepared by Syneos Health®" although Syneos is not among that trial's contractors (T1).

**T1: who is named as writer of published lay summaries [A, own count]**
Method: all EU/EEA/Swiss-based "other companies" with a trial ended 2025–26 and a published lay summary (165 trials). A fixed random sample of 30 (seed 30; 15 DACH-based, 15 other European), all lay-summary documents read (text, header, footer, PDF metadata). Then a sweep of the first two documents of all 165 trials for attribution phrases (e.g. "prepared by", "written by", "template", "elaborado por", vendor and CRO names) and PDF metadata.

| Result in the sample of 30 | Count | Examples (public documents) |
|---|---|---|
| Names an outside writing firm | **1** | iTeos (BE): "SIRO Medical Writing Pvt. Ltd, a clinical research organization, prepared this summary" |
| CRO template or CRO as sponsor | 4 | Sintetica (CH): "This document is based on CRO template tmp-0007 … CROSS Research S.A."; Synartro (SE): template code "TMP-CO03"; GCP-Service and Becro are CRO groups acting as sponsor |
| Large-group house style | 1 | Advanced Accelerator Applications (Novartis group; missed by the keyword list) |
| Sponsor letterhead only | 1 | Philogen (IT) |
| Script or AI-tool traces in the PDF metadata (author "python-docx") | 3 | F4-Pharma (AT), Cutiss (CH), Diater (ES) |
| Placeholder or "no results" letter | 3 | Formycon, Cinclus, Merus |
| No author, vendor or template shown | **17** | e.g. Grünenthal, Merz, Affimed, Pentixapharm, Idorsia, Alvotech |

| Wider sweep, all 165 trials (first 2 documents each) | Trials |
|---|---|
| Outside writer named | **4**: iTeos (2 trials, SIRO Medical Writing); Imcheck (FR): "created by Ipsen with the assistance of a third-party writing service provider"; Carrick (IE): "prepared by Syneos Health®" |
| Sponsor says it wrote the summary itself | 2: PPM Services (CH): "This summary was written by the sponsor"; Ryvu (PL): "Este resumen ha sido elaborado por el promotor" |
| CRO or sponsor template codes | 4: CROSS Research template (Sintetica); "TMP-CO03" template on two different sponsors' summaries (Synartro, Dicot); GALENpharma: "SOP CLI/REP/01, Template from 20240916" |
| Script or AI-tool traces in metadata | **6**: author "OpenAI" (iOmx Therapeutics, Martinsried/Munich); author "python-docx" (Theriva, Cutiss, Diater, OSIVAX, plus F4-Pharma from the sample) |

- *Inference:* "python-docx" is the default author of Word files made by that programming library, which AI chat tools also use to export files. Together with the "OpenAI" author field, this suggests that some small sponsors draft or format their lay summaries with general AI tools in-house. It does not prove that the text was written by AI.
- **T1 verdict against the critic's lines:** pass needed ≥10 of 30 naming an independent writing firm or showing no CRO style (seen: 1 named; "no CRO style" cannot be judged when no author is shown). Kill needed ≥20 of 30 that are CRO or in-house templates or bioequivalence/Phase I copies (identifiable: 12 incl. placeholders). **Neither line is reached; T1 is inconclusive.** Where attribution exists, it points to CROs, in-house writing and AI tools. The only outside writers seen are a CRO-type writing firm and a large CRO, both able to price below a two-person DACH start-up (*inference*).

- **First target segment (inference, if pursued):** DACH-based "other companies" with a trial that ended in the last 12 months: **99 trials** ended Jan–16 Nov 2026 (72 sponsor entities, CureVac counted under two names), **92** without a public lay summary yet [A, own count]. Caveat: summaries of adult Phase I trials are published only 30 months after the end (EMA, via C19), so some "missing" ones are filed but hidden.
- Germany-based companies with a 2026 trial and no public summary yet (37 sponsor entities, public CTIS data) include CureVac, Immunic, Formycon, CatalYm, AiCuris, Heidelberg Pharma, Pentixapharm and Nucleus Medical. The list also includes established firms such as Grünenthal, Merz, Medac, Dr. Falk, Dermapharm and Dr. Willmar Schwabe. Contract-research firms acting as sponsor (CCDRD, SocraTec, Winicker-Norimed) are in it too.
- **Decision process.** The C25 draft assumed a small purchase order at close-out, signed by a clinical-operations or regulatory manager. **The data contradict this for most trials** (red team F1): multi-country trials mostly run through large CROs (T2), and a CRO's full-service scope is usually fixed at trial start (*inference*). A close-out purchase is plausible only for one- or two-country trials run without a large CRO. Large pharma use framework contracts with CROs and language companies. Lionbridge reports that a "global biopharma" buys lay-summary translations centrally ([Lionbridge, 2022](https://www.lionbridge.com/content/dam/lionbridge/pages/case-studies/global-biopharma-company-case-study/global-biopharma-company-case-study-english.pdf)) [B].
- Adjacent purchase seen: the Austrian company Croma-Pharma bought AI-powered readability testing and re-authoring of the lay part of a medical-device safety summary (SSCP, MDR) from Lionbridge ([Lionbridge case study, Nov 2025](https://www.lionbridge.com/case-study/croma-pharma-case-study)) [B]. This is a device document, not a CTR lay summary, but it shows a DACH mid-size firm buying plain-language work from a large language company.

## 4. Solution & product wedge
- **Smallest product:** a fixed-price pack per trial. (1) An AI first draft of the CTR Annex V lay summary in English from the sponsor's results summary / CSR synopsis. (2) A review by a medical writer (accuracy, non-promotional tone, readability). (3) Machine translation into the trial-country languages, post-edited by native medical translators. (4) CTIS-ready PDFs with a short AI-use and QC record. Turnaround target: 10 working days `[UNVERIFIED]`, not benchmarked.
- **What AI does:** extract the Annex V items from tables, draft at a set reading level using the sponsor's glossary and template, check numbers against the source and flag differences for the writer, and make translation first drafts. The workflow follows the CISCRP/EMWA model: "Initial Draft Creation (Human and AI involvement)" → "Human Refinement" → "quality control (QC) and compliance check" ([CISCRP/EMWA, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf)) [B].
- **Non-goals:** no full results summary or CSR writing (CRO and regulatory-writer work); no self-serve SaaS for large pharma (Weave Bio, Peer AI, TrialAssure already sell software); no patient-panel testing in version 1 (GLSP calls user testing "not mandatory" [A]); no overdue-rescue campaign (C19: pool too small).
- *Inference:* T1 shows the substitute is not only CROs but sponsors' own staff using general AI tools. The pack's value over do-it-yourself is the writer's check and the translations, and both are human work.

## 5. Market size
**Method (re-runnable) [A, own count, 2026-11-19]:**
- Search: `POST https://euclinicaltrials.eu/ctis-public-api/search`, `searchCriteria: {"status":[8]}` ("Ended"), 100 per page, sorted by `decisionDate` both ways → **4,202** ended trials. Year = last 4 characters of `endDateEU`: 2025 = **1,826**, 2026 to 16 Nov = 1,562. Phase = search field `trialPhase`.
- Each of the 3,388 trials read with `GET /ctis-public-api/retrieve/<ctNumber>`. Sponsor = `authorizedApplication.authorizedPartI.sponsors[]` with `primary: true`; commercial = sponsor field `commercial` = "Commercial"; seat = `addresses[0].address.countryName`; countries = `authorizedApplication.memberStatesConcerned[].mscName`; contractors = `sponsors[].thirdParties[].organisationAddress.organisation.name`.
- **Lay summary present** = `results.laypersonResults` not empty, or a document whose `documentTypeLabel` contains "layperson" or "lay summary" (document titles are not used: they catch protocol synopses).
- **Large pharma groups** = sponsor name contains (word start, case-insensitive) one of: pfizer, roche, genentech, hoffmann, novartis, sandoz, hexal (incl. "H e x a l"), merck, msd, sanofi, genzyme, aventis, astrazeneca, alexion, glaxo, gsk, viiv, lilly, abbvie, allergan, bristol, celgene, myokardia, janssen, johnson, amgen, gilead, kite pharma, bayer, boehringer, novo nordisk, takeda, baxalta, shire, astellas, eisai, daiichi, ucb, csl, teva, biogen, vertex, moderna, biontech, servier, ipsen, chiesi, grifols, menarini, lundbeck, leo pharma, fresenius, stada, otsuka, regeneron, bausch, principia, tesaro, organon, viatris, mylan, sun pharma, jazz pharma, galderma, ferring, almirall, pierre fabre, zambon, recordati, angelini, orion, sumitomo, kyowa, chugai, ono pharm, beigene, beone, seagen, incyte, argenx, ascendis, lupin, lantheus, biotest. This list is wider than C19's top-50, so "other companies" is 639 instead of C25's 702. Known misses: subsidiaries under other names (e.g. Advanced Accelerator Applications, Novartis group).
- **Large CRO** = contractor name matches iqvia, quintiles, icon, pra health, pharmaceutical research associates, ppd, pharmaceutical product development, thermo fisher, syneos, inc research, inventiv, parexel, medpace, fortrea, covance, labcorp, psi cro / psi, worldwide clinical trials, premier research, novotech. Names containing "laborator", "central lab", "labs", "bioanaly" or "labcorp central" are excluded (central labs do not run trials). Mid-size CROs are not on the list, so CRO use is understated.
- Scripts were run from the session scratchpad and are not in the repo; the lists above are enough to re-run them.

| Level | Trials / year | × price | Value / year | Basis (*my math*) |
|---|---|---|---|---|
| TAM: every EU trial buys one pack | 1,826 | €6,000 | **€11.0m** | 1,826 × 6,000 = 10,956,000 |
| "Other companies", EU-wide | 639 | €3,500–6,000 | €2.24–3.83m | 639 × 3,500 = 2,236,500; × 6,000 = 3,834,000 |
| **SAM: "core"** (other companies minus bioequivalence and one-country Phase I) | 427 | €3,500–6,000 | **€1.49–2.56m** | 639 − 61 − 151 = 427; 427 × 3,500 = 1,494,500; × 6,000 = 2,562,000 |
| **Reachable without a large CRO** (core trials naming none) | 181 | €3,500–6,000 | **€0.63–1.09m** | 181 × 3,500 = 633,500; × 6,000 = 1,086,000 |
| – DACH-based core, no large CRO | 26 (of 50 core) | €3,500–6,000 | €91–156k | 26 × 3,500 = 91,000; × 6,000 = 156,000 |
| – Germany-based core, no large CRO | 16 (of 23 core) | €3,500–6,000 | €56–96k | 16 × 3,500 = 56,000; × 6,000 = 96,000 |
| Upside not counted | UK trials from 2027–28; lay protocol synopses at application (vendor claim, [Excelya, Nov 2024](https://excelya.com/wp-content/uploads/2024/11/Lay-Summaries-for-Clinical-Trials.pdf) [B]; not checked in CTIS rules `[UNVERIFIED]`) | | | |

- €3,500 and €6,000 are hypotheses, **not observed prices** `[UNVERIFIED]`. €6,000 is C19's assumed mid-point built from labour value (€2,877–8,631 per lay summary + translations).
- **Packages needed (*my math*; direct cost mid-point €2,346 from section 7):**

| Target | at €3,500 | at €6,000 | Share of the 427 core trials | Share of the 181 without a large CRO |
|---|---|---|---|---|
| €360k revenue (three salaries, C19 basis; ignores direct costs) | 103 | 60 | 24 % / 14 % | 57 % / 33 % |
| €360k **contribution** after direct costs | 312 (€1,154 each) | 99 (€3,654 each) | 73 % / 23 % | 172 % / 55 % |
| €1m revenue | 286 | 167 | 67 % / 39 % | 158 % / 92 % |

- *Inference:* even at the higher price, paying three salaries from contribution needs more than half of all reachable trials in Europe and the US. That is a freelance or small-agency business, not a venture-scale market.

## 6. Competitors
| Company | URL | Offering | Pricing | Funding | Gap we exploit |
|---|---|---|---|---|---|
| TrialAssure (US) | trialassure.com | Disclosure software; LINK AI drafts PLS; ~50,000 AI summaries for ClinicalTrials.gov studies (2023, [TranspariMED](https://www.transparimed.org/single-post/pls-automated) [B]); CRO partnership with MMS | Not public | Private | Software for disclosure teams; small sponsors need the finished document |
| Weave Bio (US) | weave.bio | "AI-native regulatory platform"; NDA workflow with Parexel and Takeda deal (snippets only `[UNVERIFIED]`) | Not public | $20m Series A, $36m total (Oct 2025) ([Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development)) [B] | Focus on large regulatory dossiers (no PLS product found) |
| Peer AI (US) | — | AI for protocols, CSRs | Not public | $12.1m [B] (C19) | Same |
| Yseop (FR) | yseop.com | Generative AI for clinical reports, ">150 trials" | Not public | Novartis dRx, Lilly [B] (C19) | Same |
| Carelane (Berlin) | htgf.de | AI end-to-end trial platform incl. medical writing; ">130 research sites" | Not public | €2.6m seed, Apr 2025 (Vorwerk Ventures, HTGF) ([HTGF](https://www.htgf.de/carelane-seed/)) [B] | Platform for running trials, not a disclosure service |
| CROs: Quanticate, Clinbay, Excelya, Certara/Synchrogenix ("over 200 PLS", snippet); Syneos and CROSS Research seen writing or templating published summaries (T1) | various | Lay summaries + translations as a service or inside the trial contract | "cost-effective" (Clinbay), no prices | Private / listed | They hold the buying decision for most multi-country trials (T2); a newcomer can at most be their overflow subcontractor |
| SIRO Medical Writing | — | Named as writer of 2 published summaries for one Belgian sponsor (T1); described there as "a clinical research organization" | Not public | Not checked | A CRO-type writing firm already sells to small EU sponsors |
| CISCRP (US non-profit) | ciscrp.org | Full-service or editorial-review lay summaries ([CISCRP, 2020](https://legacy.ciscrp.org/making-it-clear-lay-language-summaries/)) [B] | Not public | Non-profit | US-centred, English-first |
| SciencePOD (Dublin) | sciencepod.net | PLS incl. "AI-Hybrid content, where a first draft is generated by AI tools and then complemented by quality checks from a human editor" ([SciencePOD, undated page](https://sciencepod.net/?p=380039)) [B] | Not public | Small firm | Same model as ours already on offer |
| Language companies: RWS, Lionbridge, TransPerfect | — | Lay-summary creation and translation for big pharma; Lionbridge also re-authors lay text with AI for a DACH mid-size firm (Croma-Pharma, SSCP) [B] | Not public | Listed / large | Framework contracts; now also AI plain-language services |
| Indegene + Trilogy Writing (Frankfurt) | — | Medical writing with "Generative AI" (acquired Mar 2024) [B] (C19) | Not public | Listed group | German-based competitor with the same pitch |
| Do-it-yourself with general AI tools | — | Sponsor staff draft or format summaries with AI tools (T1: 6 of 165 trials show traces) | LLM licence | — | Free substitute; the pack must beat it on the writer check and translations |

*Inference:* the exact model (AI draft + human check + translation) is already offered by at least one small firm (SciencePOD), by CROs, by a CRO-type writing firm, and by large language companies, and some sponsors do it themselves with AI tools. A newcomer's only edge would be price and speed for DACH/PT small sponsors plus German and Portuguese in-house. That edge is copyable.

## 7. Business model & pricing
- **Model:** fixed price per trial pack, sold directly or white-labelled to CROs (CRO margin on top). Optional yearly bundle for sponsors with several trials.
- **Price hypothesis:** **€3,500** for EN + up to 4 languages (below C19's €5–12k labour value, to undercut CROs); **€6,000** with patient-panel review and graphics. Both `[UNVERIFIED]` (no observed price; 10+ searches in C19, 6 more in C25; TED: 0 lay-summary tenders). Benchmarks: US university results-posting service $1,000–2,500 (UCLA) [B]; patient-panel review "$3,000 to $3,500" (Citeline, snippet only, page 404) `[UNVERIFIED]`.
- **Direct cost per pack (*my math*, assumptions marked):**
  - Writer time: manual "approximately 20 hours", AI "less than one day" (TrialAssure claim [B]); AI saved writers ">40 %" of drafting time on 6 journal abstracts ([JAMIA Open 2025, PMID 40183004](https://europepmc.org/article/MED/40183004)) [A]. Assume 8–20 h per pack.
  - Writer cost: Medical Writer average **€55,400 gross a year** in Germany (range €46,500–65,100; [StepStone](https://www.stepstone.de/gehalt/Medical-Writer.html), undated, read 2026-11-19) [B]. With ~21 % employer costs `[UNVERIFIED assumption]` ≈ €67k. Assume 1,600 productive hours a year `[UNVERIFIED assumption]` → 80–200 packs per writer → **€335–838** per pack (67,000 / 200 and / 80).
  - Translation: measured median length **11,799 characters** [A, own count, section 2] → 11,799 / 55 = 214.5 lines × €1.95–2.15 (German court rate, § 11 JVEG via C19) = **€418–461** per language; 4 languages → **€1,673–1,845**. AI pre-translation plus post-editing could lower this; not sourced.
  - **Total ≈ €2,008–2,683** (335 + 1,673; 838 + 1,845), mid-point €2,346. Gross margin at €3,500: 23–43 %; at €6,000: 55–67 %.
- *Inference:* service margins and one-off buys per customer (355 of 455 "other companies" had one ending trial in 2025). Revenue grows with headcount, not software. Investors look for software-like margins; this gets there only if writer time falls well below 8 h, and nobody shows that with real CTR documents yet.

## 8. Regulation & data
| Topic | Rule | What it means for us | Source |
|---|---|---|---|
| Content | Annex V CTR, 10 items | Fixed template; good for AI, and equally good for do-it-yourself AI | [CTR](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) [A] |
| Tone | LS must be "non-promotional"; review by "patient(s), medical monitor, statistician" recommended; user testing "not mandatory" | Writer review is the core of the offer; promotional slip = sponsor risk | [GLSP](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) [A] |
| AI use, regulators' standard | AI "used for drafting, compiling, editing, translating … medicinal product information documents should be used under close human supervision … quality review mechanisms need to be in place" (about product information, the closest EMA text found) | Human QC is expected, not optional | [EMA reflection paper, Sep 2024](https://www.ema.europa.eu/en/documents/scientific-guideline/reflection-paper-use-artificial-intelligence-ai-medicinal-product-lifecycle_en.pdf) [A] |
| EU AI Act Art. 50(4) | Deployers of AI that generates text "published with the purpose of informing the public on matters of public interest shall disclose" it, **unless** it "has undergone a process of human review or editorial control" with a person holding "editorial responsibility"; Art. 50 applies from 2 Aug 2026 | With documented writer review and sponsor sign-off, disclosure is not required by law, but the CISCRP group and 62.4 % of patients want it anyway | [AI Act text, Art. 50](https://artificialintelligenceact.eu/article/50/), [Art. 113](https://artificialintelligenceact.eu/article/113/) [B, secondary copy of the law]; [JMIR AI 2026, PMID 42330509](https://europepmc.org/article/MED/42330509) [A] |
| Industry practice | "Standalone use of AI for creating LS concerns clinical trial sponsors"; in 2023 "publicly posted, AI-generated LS that lacked proper human oversight … were eventually removed" (no vendor named) | Buyers will audit the QC step | [CISCRP/EMWA paper, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) [B] |
| AI quality evidence | ChatGPT-4o PLS scored 1 point higher on information and 2 points higher on readability than Cochrane human PLS (36 summaries, blinded RCT); GPT-4 lay summaries more readable than originals (204 articles); but in a crowdsourced test (150 readers) "human-written PLSs lead to significantly better comprehension". None tested CTR trial-result lay summaries | Drafts are good; comprehension still needs a human | [Cochrane Evid Synth Methods 2025, PMID 40727555](https://europepmc.org/article/MED/40727555) [A]; [JMIR 2025, PMID 41259712](https://europepmc.org/article/MED/41259712) [A]; [arXiv 2505.10409, May 2025](https://arxiv.org/abs/2505.10409) [B, preprint] |
| Patient trust | Trust "a lot": AI-only documents 12.3 %, human-only 39.1 %; 95.0 % rate human involvement in review "very" or "somewhat important" (n = 1,010, EU + US) | Sell "human-checked", not "AI-written" | [JMIR AI 2026, PMID 42330509](https://europepmc.org/article/MED/42330509) [A] (authors from CISCRP, a lay-summary provider) |
| Data protection | Inputs should use aggregated data; "organizations must ensure that AI models are not retaining sensitive information" | Lay summaries use aggregate results, so little personal data (*inference*). Unpublished results are confidential: EU-hosted model, no training on client data, NDA + data processing agreement | [CISCRP/EMWA](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) [B] |
| MDR / DiGA | Not applicable: documents for the public, no medical purpose for a patient (*inference*) | No certification needed | — |
| Marketing in Germany: email | Email advertising needs "vorherige ausdrückliche Einwilligung" of the addressee | No cold emails | [§ 7 UWG](https://www.buzer.de/7_UWG.htm) [A] |
| Marketing in Germany: phone to businesses | Needs "zumindest mutmaßliche Einwilligung". The Federal Court of Justice requires that "aufgrund konkreter tatsächlicher Umstände ein sachliches Interesse des Anzurufenden an der Telefonwerbung vermutet werden kann"; a "allgemeiner Sachbezug" to the called firm's business is not enough, and neither is the custom of cold calling in an industry (BGH, 11 Mar 2010, I ZR 27/08, para. 27, 31–32). The chamber of commerce adds that it does not matter whether the offer is useful to the firm (IHK Bonn, citing BGH I ZR 191/03 and OLG Hamm 4 U 189/09) | A call to a name taken from CTIS with no prior contact has no concrete basis for presumed interest, so it is a weak legal footing (*inference*; not legal advice). Use warm introductions or contacts made at events. Whether a pure "research" call by a would-be seller counts as advertising was not checked `[UNVERIFIED]`; the IHK notes that even customer-satisfaction calls need consent (KG Berlin 5 U 35/20) | [BGH I ZR 27/08 (lexetius)](https://lexetius.com/2010,2788) [A]; [IHK Bonn, May 2024](https://www.ihk-bonn.de/fileadmin/dokumente/Downloads/Recht_und_Steuern/Wettbewerbsrecht/WerbungTelefonBriefE-Mail.pdf) [B] |

- **Certifications:** none required by law. Language firms advertise ISO 17100 for translation ([Translated](https://translated.com/resources/medical-translation-services-pricing-healthcare-documentation-cost-analysis)) [B]; large sponsors may ask for it in vendor audits `[UNVERIFIED]`. Professional liability insurance: cost not checked `[UNVERIFIED]`.
- **Time and cost to compliance (inference):** weeks, not months: written SOPs for AI use and QC, an EU-hosted LLM contract, NDA/DPA templates. No regulator approval.

## 9. Go-to-market
- **Reachable buyers (inference):** sponsors whose one- or two-country trials run without a large CRO (181 core trials a year EU-wide, 26 DACH). Multi-country trials are mostly CRO-bound (T2), so for those the route is the CRO's overflow work, which goes to writers, not to a sales-led firm.
- **First 10 contacts, only if (b) is chosen (inference):** DACH companies from the public CTIS list (section 3) with a 2026 trial and no summary yet. Contract-research firms acting as sponsor (CCDRD, SocraTec, Winicker-Norimed, GCP-Service) are possible white-label partners.
- **Routes and their cost (F5).** The spin-out events in `ventures/spinout-cofounder/entry-pack.md` gather founders, researchers and investors, not trial managers, so they do **not** count as a route here. Real routes:
  - BioM / BayStartUP life-science events in Munich (repo `research/munich-ecosystem.md`) [B]; fees not checked.
  - DIA Europe 2027, Basel, 16–18 Mar 2027: a "Connect & Discover" day pass costs **EUR 179 per day plus VAT** and "does not include access to the full DIA Europe scientific programme"; full-conference rates on the page run from €1,090 (young professional) and €2,050 (EMA-registered SME) up to €3,350 ([DIA registration page](https://www.diaglobal.org/en/flagship/dia-europe-2027/about/register)) [B]. Travel from Lisbon is extra and not costed.
  - EMWA (writers, for the co-founder search) [B] (C19); event fees not checked.
  - Warm introductions through people you already know. No cold calls or cold emails (section 8).
- **Pilot design (if ever):** one real trial at a fixed price (e.g. €2,500 for an EN summary + German version), delivery within 10 working days. Success = the sponsor files it in CTIS with wording changes only and agrees to be a reference.

## 10. Funding path
- **Grants now: none fit while you are employed.** EXIST-Gründungsstipendium excludes an active job (side work ≤20 h a month) and must be filed by a German university. FLÜGGE requires membership of the applying Bavarian university (via repo `research/munich-ecosystem.md`, fact-checked) [A]. From Sep 2027, EXIST through a host university (SCE/HM, TUM, LMU) is possible if you have left your job or are on a sabbatical and the team has a graduate medical writer (via repo) [A].
- **Investors:** HTGF and Vorwerk Ventures funded an AI trial platform with medical writing (Carelane, €2.6m seed, 2025) [B]. *Inference:* a service pack with 23–67 % gross margin and a reachable market of about €1m a year will not fit a seed fund. The only path is to bootstrap. €10k of your own money covers the LLM set-up and a freelance writer for 2–3 pilots (*my math:* 3 packs × ~€2.3k direct cost = €7.0k).

## 11. Team
- **Must have: a medical-writer co-founder** with CTR lay-summary experience, German + English, ideally Portuguese. This covers your main gap (no clinical or medical-writing background, `founder-brief.md`). Without one, every pack depends on freelancers bought at €82.2/h (EMWA median [B], C19), and the margin is gone.
- **The harder question (F2):** why would such a writer split a small service business with a non-writer? An experienced writer with an LLM licence can sell this alone (*inference*). You would bring sales and AI set-up, but sales here are relationship sales to clinical operations and CROs, where you have no contacts yet.
- **Where to find one:** EMWA (membership "over 1,000" per a search snippet `[UNVERIFIED]`); StepStone lists **206** Medical Writer ads (re-read 2026-11-19; 228 earlier the same day) and names Berlin, Hamburg and **München** as cities with many openings ([StepStone](https://www.stepstone.de/gehalt/Medical-Writer.html)) [B]; Lisbon: a Hays ad "Scientific Communication & Medical Writer (M/F/D)", Grande Lisboa (title only seen) [C]; German-language scientific-communications roles in Lisbon (search snippets only) `[UNVERIFIED]`.
- **Optional later:** native translators/reviewers for PT and DE; an engineer for the document pipeline (your AI-agent skills cover a first version, *inference*).

## 12. Risks & kill criteria (researcher pre-mortem, updated with the red team's)
| Riskiest assumption | Evidence so far | How to test | Kill if (fixed now) | Status 2026-11-19 |
|---|---|---|---|---|
| R1. Small sponsors buy lay summaries as an **outside purchase** at ≥€2,500. *Outside purchase* = bought by the sponsor from a firm other than the trial's CRO, under a separate order | T1: 1 of 30 published summaries names an outside writing firm; 4 of 165 in the sweep [A, own count]; no price seen | Only if (b): conversations via warm intros (section 13) | Fewer than 2 of the first 5 report an outside purchase ≥€2,500; or ≥3 of 5 say the summary is in the CRO contract or written in-house (red team P1) | Not tested; desk signals point to "kill" |
| R2. Enough reachable volume | 181 core trials a year without a large CRO EU-wide, 26 DACH [A, own count]; €360k contribution needs 99–312 packs | Ask 1–2 small CROs for overflow volume | No small CRO names ≥20 packs a year at ≥€2,000 | Not tested |
| R2b. Multi-country trials are not CRO-bound (T2) | 77.1 % of 3+-country "other company" trials name a large CRO [A, own count] | Desk count (done) | ≥70 % name a large CRO | **Met: kill line reached** |
| R3. AI draft + human check takes ≤8 h of writer time | Vendor: "less than one day" [B]; study: >40 % saving on 6 abstracts [A]; no data on real CTR documents | Cannot be tested without a writer. The desk test in section 13 checks only whether the AI misses Annex V items | Writer time >15 h per pack in a writer-run test | Untested until a writer is found |
| R4. A medical-writer co-founder joins **on fair terms** | 206 DE job ads show demand for writers [B]; none approached | EMWA/LinkedIn after your OK | No writer candidate by **31 Mar 2027** who accepts a split in which your share is earned by sales and AI work, not only a freelance rate | Not tested |
| R5. Incumbents do not undercut with AI | SciencePOD AI-hybrid [B]; Indegene/Trilogy GenAI [B]; offshore writing firm seen (T1) [A, own count]; do-it-yourself AI seen (T1) | Price question in any conversation | A CRO, writing firm or language firm quotes <€1,500 for EN + 1 language | Not tested |
| R6. Your time | Part-time until Sep 2027 (founder brief); spin-out kill date 28 Feb 2027 (decision 2026-11-19) | — | You are named in a spin-out draft application → stop this idea (no time for both) | Open |

- **Overall kill line:** if R1 fails, or R1 passes but R2 shows <20 packs a year within reach, drop the idea as a company. R2b is already met on desk evidence, so the remaining case rests on one- and two-country trials only.
- **Pre-mortem (inference):** the most likely failure is "nobody objects, nobody buys". Sponsors call lay summaries a chore, but the CRO bundles them into the trial contract or staff do them in-house with AI tools. No separate purchase exists for a newcomer to win.

## 13. Validation plan (only if you choose option b in C28)
1. **Desk check, no outward action (researcher, 1 run):** take 3 trials whose lay summary was posted in CTIS after 1 Sep 2026, so the model cannot have seen them in training (*assumption* about model cut-offs). Draft from the public results summary only and check the draft against the 10 Annex V items. This tests **only** "does the AI miss Annex V items". It cannot test factual accuracy or writer time: nobody qualified checks the result. Pass: ≤2 missing items per summary. A failure here kills the AI-drafting step, not the idea.
2. **Two conversations, warm introductions only (outward; needs your approval):** (T3) one freelance medical writer; (T4) one small DACH CRO's medical-writing lead. Mom-Test questions: "Tell me about the last lay summary you wrote or bought. Who paid, under which order, how long did it take, what did it cost? Did the CRO quote it separately?"
   - **Confirms:** the writer says small sponsors buy lay summaries outside the CRO contract and names a price ≥€2,500; the CRO names ≥20 overflow lay summaries a year it would subcontract.
   - **Kills:** the writer says it is a one-day job at day rate (~€650–800 at €82.2/h, *my math*: 8–10 h × 82.2 = 658–822) or CRO work; the CRO says "in-house" or "freelancers".
3. **Only if both pass:** 5 sponsor conversations per R1 (definition of outside purchase above), reached at BioM events or DIA Europe (day pass €179 + VAT, section 9).
4. **Timing (inference):** step 1 in December 2026; step 2 by 31 Jan 2027; decide by 28 Feb 2027, the spin-out kill date, so this never competes with the spin-out route for your hours.

## Gaps / [UNVERIFIED]
- No observed price for a lay summary or pack (16+ searches across C19 and C25; TED 0). €3,500 and €6,000 are hypotheses.
- Who signs in practice (sponsor vs CRO) is inferred from contractor lists, T1 attributions and a 2018 CISCRP statement; no survey found.
- T1: 17 of 30 sampled summaries show no author at all, so the share written by outside firms cannot be measured from public documents. PDF metadata traces ("python-docx", "OpenAI") show the tool that made the file, not who wrote the text.
- Writer hours with AI on real CTR documents: no data; 8–20 h is an assumption from a vendor claim and a study on abstracts.
- Employer-cost add-on (21 %) and 1,600 productive hours: assumptions. Lay-summary length is now measured (median 11,799 characters).
- Weave Bio–Parexel/Takeda, Certara "200 PLS", EMWA membership size, Lisbon German-language writer roles, the Reddit post: search snippets only. SIRO Medical Writing: seat and prices not checked.
- The large-CRO list misses mid-size CROs; the large-company list misses some subsidiaries (e.g. Advanced Accelerator Applications).
- AI Act text read from a secondary site (EUR-Lex returned an empty page to curl).
- Whether a research-only call by a would-be seller is "advertising" under § 7 UWG: not checked; this is not legal advice.
- BioM and EMWA event fees, travel cost to Basel: not checked.

## Sources
- https://euclinicaltrials.eu/ctis-public-api/search and https://euclinicaltrials.eu/ctis-public-api/retrieve/<ctNumber> — own count: 4,202 ended trials; 3,388 ended 2025–2026 read one by one; sponsor seat, phase, countries, CRO contractors, contractor duties, lay-summary status; accessed 2026-11-19
- https://euclinicaltrials.eu/ctis-public-api/documents/<ctNumber>/<uuid>/download — returns a short-lived download URL for a public CTIS document; used for T1 (all lay-summary documents of 30 sampled trials, first two documents of 165 trials: text and PDF metadata); accessed 2026-11-19
- https://accelerating-clinical-trials.europa.eu/document/download/1271bfdd-8830-479c-8e3a-2ada45477c30_en?filename=ACT%20EU%20KPI%20Report_September_2026.pdf — EMA/ACT EU compliance 77.3 / 83.8 / 58.3 %, overdue 9.4 / 5.9 / 19.5 %, deadline definition; accessed 2026-11-19
- https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf — Art. 37(4), Annex V CTR; accessed 2026-11-19
- https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf — translations recommended, cost drivers, review, non-promotional; accessed 2026-11-19
- https://www.ema.europa.eu/en/documents/scientific-guideline/reflection-paper-use-artificial-intelligence-ai-medicinal-product-lifecycle_en.pdf — "close human supervision" for AI drafting of product information (Sep 2024); accessed 2026-11-19
- https://artificialintelligenceact.eu/article/50/ and https://artificialintelligenceact.eu/article/113/ — AI Act Art. 50(4) text and 2 Aug 2026 application date (secondary copy); accessed 2026-11-19
- https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf — CISCRP/EMWA AI working group: members (Merck KGaA, UCB, CSL Behring), Merck KGaA role, human oversight, 2023 removal (no vendor named), workflow (Jun 2025); accessed 2026-11-19
- https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results — working group formed after "challenges faced by the industry in late 2023"; Biogen and AstraZeneca panellists and roles; accessed 2026-11-19
- https://www.transparimed.org/single-post/pls-automated — TrialAssure ~50,000 AI PLS, "approximately 20 hours per document", "less than one day" (24 Oct 2023); accessed 2026-11-19
- https://www.transparimed.org/single-post/european-medicines-agency-takes-rapid-action-on-missing-clinical-trial-results — EMA reminders and national monitoring (9 Jul 2026); accessed 2026-11-19
- https://www.transparimed.org/single-post/european-medicines-agency-takes-multiple-steps-to-improve-clinical-trial-reporting — EMA KPIs, reminders (17 Nov 2026); accessed 2026-11-19
- https://bukopharma.de/wp-content/uploads/2026/06/CTIS-legal-violations-in-Germany_2026.pdf — letter to BfArM, 9 of 30 trials without results (15 Jun 2026); accessed 2026-11-19
- https://www.hra.nhs.uk/planning-and-improving-research/policies-standards-legislation/clinical-trials-investigational-medicinal-products-ctimps/clinical-trial-regulations-reform/guidance-on-changes-to-the-clinical-trials-regulations/research-transparency-requirements-for-clinical-trials/offering-to-share-a-summary-of-results-with-participants — UK lay-results duty from 28 Apr 2026; accessed 2026-11-19
- https://europepmc.org/article/MED/40727555 — Cochrane RCT, ChatGPT-4o vs human PLS (2025); accessed 2026-11-19 (abstract via Europe PMC REST)
- https://europepmc.org/article/MED/41259712 — ChatGPT-4 lay summaries, 204 prostate-cancer articles (JMIR 2025); accessed 2026-11-19 (abstract)
- https://europepmc.org/article/MED/40183004 — bespoke AI saved writers >40 % time on PLS abstracts, 10 writers, 6 abstracts (JAMIA Open 2025); accessed 2026-11-19 (abstract)
- https://europepmc.org/article/MED/42330509 — patient trust in AI documents, n = 1,010 (JMIR AI 2026); accessed 2026-11-19 (abstract)
- https://arxiv.org/abs/2505.10409 — crowdsourced comprehension, human PLS better understood (preprint, May 2025); accessed 2026-11-19
- https://legacy.ciscrp.org/?p=9491 — "most research sites and sponsors choose to work with an independent third-party" (2018); accessed 2026-11-19
- https://legacy.ciscrp.org/making-it-clear-lay-language-summaries/ — CISCRP full-service vs editorial-review models (2020); accessed 2026-11-19
- https://appliedclinicaltrialsonline.com/view/trialassure-announces-ai-generative-text-partnership-with-mms — CRO MMS + TrialAssure AI PLS drafts (3 Aug 2023); accessed 2026-11-19
- https://www.pharmaceutical-technology.com/sponsored/lay-of-the-land-understanding-lay-summary-requirements-and-the-challenges-they-bring/ — RWS sponsored article, translation turnaround pain (28 Oct 2022); accessed 2026-11-19
- https://www.lionbridge.com/content/dam/lionbridge/pages/case-studies/global-biopharma-company-case-study/global-biopharma-company-case-study-english.pdf — lay-summary translation for a global biopharma (Sep 2022); accessed 2026-11-19
- https://www.lionbridge.com/case-study/croma-pharma-case-study — Croma-Pharma SSCP laypersons' part: AI-powered readability testing and re-authoring by Lionbridge (published 18 Nov 2025); accessed 2026-11-19
- https://sciencepod.net/?p=380039 — SciencePOD AI-Hybrid PLS (undated page); accessed 2026-11-19
- https://www.htgf.de/carelane-seed/ — Carelane €2.6m seed, Vorwerk + HTGF (Jul 2025); accessed 2026-11-19
- https://excelya.com/wp-content/uploads/2024/11/Lay-Summaries-for-Clinical-Trials.pdf — CRO lay-summary service; lay protocol synopsis claim (Nov 2024); accessed 2026-11-19
- https://www.stepstone.de/gehalt/Medical-Writer.html — Medical Writer salary €55,400 average; 206 ads (re-read); accessed 2026-11-19
- https://www.buzer.de/7_UWG.htm — § 7 UWG consent rules for email and phone advertising; accessed 2026-11-19
- https://lexetius.com/2010,2788 — BGH 11 Mar 2010, I ZR 27/08 (full text): presumed consent for B2B calls needs concrete circumstances; general relevance and industry custom not enough (paras. 27–32); accessed 2026-11-19
- https://www.ihk-bonn.de/fileadmin/dokumente/Downloads/Recht_und_Steuern/Wettbewerbsrecht/WerbungTelefonBriefE-Mail.pdf — IHK Bonn guidance on phone, letter and email advertising (PDF dated 8 May 2024), incl. BGH I ZR 191/03, OLG Hamm 4 U 189/09, KG Berlin 5 U 35/20; accessed 2026-11-19
- https://www.diaglobal.org/en/flagship/dia-europe-2027/about/register — DIA Europe 2027 rates: Connect & Discover EUR 179/day + VAT; €1,090 young professional, €2,050 SME, up to €3,350; accessed 2026-11-19
- https://translated.com/resources/medical-translation-services-pricing-healthcare-documentation-cost-analysis — ISO 17100 cited by a language firm; accessed 2026-11-19
- https://expressoemprego.pt/emprego/scientific-communication---medical-writer-(m-f-d)/grande-lisboa/2434256 — Hays ad title, Lisbon medical writer (title only); accessed 2026-11-19
- Via repo (C19, fact-checked 2026-11-19): EFGCP/EFPIA 35–105 h; EMWA €82.2/h; UCLA fees; JVEG €1.95–2.15 per 55 characters; § 97 AMG; Weave Bio, Peer AI, Yseop, Indegene/Trilogy, Quanticate, Clinbay; DIA Europe 2027. Via repo `research/munich-ecosystem.md` (fact-checked): EXIST and FLÜGGE eligibility, HTGF/Bayern Kapital, BioM.

## Fix log (C29 + C30, 2026-11-19; the brief's one fix round, rule 14)
| Review item | Fix |
|---|---|
| FC 1 (critical): TrialAssure "~50,000 taken offline" | Bottom line and section 8 now say a 2023 removal was reported by CISCRP/EMWA with no vendor named; TrialAssure row no longer says "later criticised" |
| FC 2: "small and mid-size" not a size test | Renamed "other companies" with established private firms named; large-company list widened and written out (section 5) |
| FC 3/4: CRO and top-50 lists not recorded | Both lists written out in section 5; central-lab entities excluded from "large CRO"; all counts re-run on the recorded lists |
| FC 5: lay-summary rule | Rule = `laypersonResults` or `documentTypeLabel` with "layperson"/"lay summary"; titles not used. New 2026 DACH figure: 99 trials, 92 without a public summary |
| FC 6: "3 contractors mention lay" | Now: 0 of 6,588 free-text duty entries |
| FC 7: citation swap | Biogen role → Informa; Merck KGaA / UCB / CSL Behring members → CISCRP/EMWA (sections 2, 3) |
| FC 8: one-sided AI bullet | Bottom line adds the arXiv comprehension result, says which study the >40 % comes from, that no study tested CTR summaries, and that the EMA text is about product information |
| FC 9: wording | "95.0 % rate human involvement in review very/somewhat important"; EMA deadline definition quoted; KPI scope noted |
| FC 10: trivia | StepStone 206 (re-read); 92 → superseded by the new cost (99); SciencePOD "2024" → undated page |
| RT F1: buyer at trial start | R1 and section 13 define "outside purchase"; the close-out decision process is marked as contradicted by the CRO data (section 3) |
| RT F2: founder value | Bottom-line bullet added; R4 kill line changed to "accepts a split …"; section 11 |
| RT F3: phase and country splits | Tables added (section 3); SAM restated as 427 core / 181 without large CRO (section 5); package table re-based |
| RT F4: €0 quality test | Redefined as a desk check of Annex V completeness only, on post-1 Sep 2026 summaries; writer-time kill removed from it; R3 untested until a writer is found |
| RT F5: routes and calls | Spin-out events removed as a route; real routes with costs (DIA day pass €179 + VAT); BGH test for B2B calls quoted; warm introductions only |
| RT T1, T2 desk checks | Run (section 3). T2 meets its kill line; T1 is inconclusive by its thresholds, with signals toward CRO / in-house / do-it-yourself AI |
| Recommendation | Changed from (b) to (a): drop as a venture |
| Not in a review | Translation cost re-based on the measured median length (11,799 characters): direct cost €2,008–2,683 (was €1,755–2,402); margins and the package table updated |
