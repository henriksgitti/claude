# Fact-check: ventures/trial-lay-summaries/brief.md (task C27, fact-check half)
Date 2026-11-19 | Verdict: **needs work (one critical fix, otherwise minor)** | Sources checked: 34 of 34 cited URLs opened (curl + text extraction; Europe PMC REST for the 4 abstracts; WebFetch for TranspariMED and the RWS article), plus a full CTIS re-run (4,202 ended trials; 3,388 ended 2025–26 retrieved one by one)

Scope: first fact-check of this brief (created in C25, commit 028185d). Red-team half of C27 (CRO-channel logic, kill lines, "niche service" verdict) is left for a separate RED TEAM run.

**What holds.** Every law and guidance quote was found verbatim: Art. 37(4) and the 10 Annex V items (CTR), the GLSP translation, cost-driver, review and "not mandatory" lines, § 97 AMG (€25,000), § 7 UWG (e-mail: "vorherige ausdrückliche Einwilligung"; phone to businesses: "zumindest mutmaßliche Einwilligung"), AI Act Art. 50(4) and the 2 Aug 2026 date (Art. 113, amended text), the EMA reflection paper ("close human supervision", Sep 2024), and the HRA rule (CTIMPs submitted from 28 Apr 2026). All EMA KPI figures match (77.3 / 83.8 / 58.3 % on time; 9.4 / 5.9 / 19.5 % overdue; data to 30 Sep 2026). The 4 study abstracts say what the brief says (Cochrane RCT +1 information / +2 readability, 36 summaries; JMIR 204 articles; JAMIA Open >40 % time saved; JMIR AI 12.3 % vs 39.1 % trust "a lot", 62.4 % transparency "very important"). The headline CTIS counts reproduce exactly (4,202 ended; 1,826 in 2025; 1,562 in 2026; 534 non-commercial; EU/EEA-based 315 trials / 210 sponsors; Germany-based 43 / 30; Bavaria 15, greater Munich 10). All arithmetic in sections 5 and 7 recomputes. No invented quotes or interviews.

## Critical issues (must fix)
1. **"A vendor's ~50,000 AI summaries had to be taken offline" is not in any source (Bottom line, bullet 4; section 6, TrialAssure row "later criticised, see section 8").** Two true facts were merged into one claim about a named company:
   - The [CISCRP/EMWA paper](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) says a concern "was observed in 2023 in a large-scale instance of publicly posted, AI-generated LS that lacked proper human oversight. These lay summaries were eventually removed …". It names **no vendor and no number**.
   - The [TranspariMED post (24 Oct 2023)](https://www.transparimed.org/single-post/pls-automated) reports TrialAssure's "nearly 50,000" AI summaries. It says **nothing about removal**; it quotes the company's own caveat that AI "is not a complete replacement of a skilled human writer".
   - A web search (TrialAssure + removed / accuracy concerns) found no takedown report.
   Fix: say "In 2023 a large set of publicly posted AI-written lay summaries was removed after accuracy concerns (CISCRP/EMWA 2025; vendor not named) [B]", and drop "later criticised" from the TrialAssure row, or tag the link `[UNVERIFIED]`. This names a competitor as having failed in public, so it must be right before the brief is used outside the repo. It does not change the recommendation.

## Minor issues (for the researcher in the same fix round; not separate tasks)
2. **"Small and mid-size companies" is not a size test (sections 2, 3, 5).** The group is every commercial sponsor not on the top-50 keyword list (C19 called it "other companies"). Germany-based 2026 members include Grünenthal, Merz, Medac, Dr. Falk, Dermapharm, Dr. Willmar Schwabe, Lupin Europe and Lantheus; "H e x a l AG" (Sandoz group) escapes the keyword list because CTIS spells it with spaces. So the 702 "SAM" and the DACH 81 include some large private firms. Rename to "other companies (mostly small/mid, incl. some large private firms)" or remove the large ones.
3. **Large-CRO counts reproduce only roughly, and the list cannot be re-run.** Section 3 says "and similar (list in the script notes, section 5)", but section 5 has no list and no script is in the repo. With the 12 named CROs plus their former names (Quintiles, Covance, Labcorp, PRA, INC) the critic gets: US-based 178 of 254 (70.1 %; file 186 of 262, 71.0 %); EU/EEA-based 74 (file 85); Germany-based 9 (file 13); non-commercial 12 (file 23). The US finding ("~70 % through large CROs") holds; the EU/DE CRO counts depend on the unlisted names. Record the full list in the file.
4. **Top-50 vs other split differs by ~1.5 %** (critic 599 / 693 vs file 590 / 702; US "other" 254 vs 262; DACH 80 / 62 sponsors vs 81 / 63) because the keyword list is only partly written down. Not decision-relevant.
5. **"107 of 114 DACH trials with no public lay summary" (section 3)**: critic gets **104 of 113** (79 sponsors vs 80) with lay summary = `results.laypersonResults` or a document whose label contains "layperson"/"lay summary". A looser text match (any document containing "lay") wrongly counts "Synopsis of the protocol" files and addresses such as "Industrial Layout"; say which rule was used. Germany-based 2026 companies without a summary: 39 (file 40); all 11 named examples are in the list.
6. **"Only 3 of 3,388 trials name a contractor whose recorded task mentions 'lay'"**: the critic searched the free-text duty field (`thirdParties[].sponsorDuties[].value`, 6,588 entries) and found **0** mentions of lay summaries (one "Safety Summary" narrative task). Point unchanged (contractor lists do not show who writes lay summaries); fix the number or the field.
7. **Wrong source for two working-group facts (section 2 voices; section 3 table).** "Clinical Trial Transparency Lead, Biogen" is the [Informa article](https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results)'s wording, not the CISCRP/EMWA paper's (which lists that person as "Associate Director, Head of Health Literacy & Plain Language Center of Excellence, Biogen"). Conversely, the member list "Merck KGaA, UCB, CSL Behring" is in the CISCRP/EMWA paper, not in the Informa article (which names only Biogen and AstraZeneca panellists). Swap the citations.
8. **Bottom line, bullet 4, is more one-sided than section 8.** It says AI drafts were "as good as or better" but leaves out the crowdsourced study in the same section ("human-written PLSs lead to significantly better comprehension", 150 readers, [arXiv](https://arxiv.org/abs/2505.10409)). The ">40 % time saved" is from a different study (JAMIA Open: 10 writers, 6 journal abstracts), not the Cochrane RCT it is bracketed with. None of the 4 studies tested CTR trial-result lay summaries. The same bullet's EMA quote is about "medicinal product information documents"; section 8 says so, the bottom line does not.
9. **Wording a notch stronger than the sources.** "95.0 % want human review": the survey asked whether human involvement in review is "Very" or "Somewhat important" (95.0 %). EMA KPI "sponsor's justified date": the report says "the later of the expected submission date communicated by the sponsor and the relevant regulatory deadline", and it measures results reporting in general, not lay summaries.
10. **Trivia:** StepStone now shows 206 Medical Writer ads (file 228; live count). The contribution row "92 packs at €6,000" is 360,000 / 3,900 = 92.3, so 93. SciencePOD "2024" is not on the page; Lionbridge "2022" is from the PDF metadata (8 Sep 2022), fine.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| Art. 37(4) lay summary "understandable to laypersons"; Annex V 10 items incl. "Description of adverse reactions and their frequency", "Overall results" | [CTR](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) | supported | Verbatim |
| "While the EU CTR does not request translations … as a minimum … local official language(s)"; "major costs will account for staff or contractors …"; review "(patient(s), medical monitor, statistician, etc.)"; user test "not mandatory"; "non-promotional" | [GLSP 2021](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) | supported | Verbatim; >3 years old (flagged) |
| "between 35 to 105 hours" | [EFGCP/EFPIA](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf) | supported | Verbatim; 2022 |
| TrialAssure "approximately 20 hours per document", "less than one day", ~50,000 PLS (24 Oct 2023) | [TranspariMED](https://www.transparimed.org/single-post/pls-automated) | supported | WebFetch; no removal mentioned (critical 1) |
| 77.3 / 83.8 / 58.3 %; 9.4 / 5.9 / 19.5 %; to 30 Sep 2026 | [ACT EU KPI Sep 2026](https://accelerating-clinical-trials.europa.eu/document/download/1271bfdd-8830-479c-8e3a-2ada45477c30_en?filename=ACT%20EU%20KPI%20Report_September_2026.pdf) | supported | Deadline = later of sponsor's expected date and legal deadline (minor 9) |
| § 97 AMG up to €25,000 for Art. 37(4) documents | [buzer.de](https://www.buzer.de/97_AMG.htm) | supported | Verbatim |
| EMA reminders, national monitoring, letter from 20 groups (9 Jul 2026) | [TranspariMED](https://www.transparimed.org/single-post/european-medicines-agency-takes-rapid-action-on-missing-clinical-trial-results) | supported | Verbatim |
| EMA KPIs published, reminders (17 Nov 2026) | [TranspariMED](https://www.transparimed.org/single-post/european-medicines-agency-takes-multiple-steps-to-improve-clinical-trial-reporting) | supported | Page "2 days ago" on 19 Nov |
| Letter to BfArM 15 Jun 2026; 9 (30.0 %) of 30 trials without results as of Nov 2025 | [BUKO PDF](https://bukopharma.de/wp-content/uploads/2026/06/CTIS-legal-violations-in-Germany_2026.pdf) | supported | Verbatim |
| UK: from 28 Apr 2026, summary "understood by members of the public" within 12 months; not for CTIMPs submitted before | [HRA](https://www.hra.nhs.uk/planning-and-improving-research/policies-standards-legislation/clinical-trials-investigational-medicinal-products-ctimps/clinical-trial-regulations-reform/guidance-on-changes-to-the-clinical-trials-regulations/research-transparency-requirements-for-clinical-trials/offering-to-share-a-summary-of-results-with-participants) | supported | Verbatim; "from 2027–28" is labelled inference |
| Working group formed "in response to the challenges faced by the industry in late 2023, beginning of 2024"; Biogen, AstraZeneca roles | [Informa](https://informaconnect.com/guiding-ai-in-plain-language-summaries-for-clinical-trial-results) | partially | Quote verbatim; Merck KGaA / UCB / CSL members are in the CISCRP paper (minor 7) |
| Workflow "Initial Draft Creation (Human and AI involvement)" → "Human Refinement"; "Standalone use of AI for creating LS concerns clinical trial sponsors"; 2023 removal; "not retaining sensitive information"; Merck KGaA role | [CISCRP/EMWA, Jun 2025](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) | supported | Verbatim; Biogen role wording is from Informa (minor 7); vendor of the removed summaries not named (critical 1) |
| "approximately one day, to translate an unknown quantity into an unknown number of languages" (28 Oct 2022) | [RWS / Pharmaceutical Technology](https://www.pharmaceutical-technology.com/sponsored/lay-of-the-land-understanding-lay-summary-requirements-and-the-challenges-they-bring/) | supported | WebFetch (curl 403); sponsored, RWS |
| "most research sites and sponsors choose to work with an independent third-party" (14 Mar 2018) | [CISCRP](https://legacy.ciscrp.org/?p=9491) | supported | Verbatim; >3 years old (flagged) |
| CISCRP full-service vs Editorial Review (13 Feb 2020) | [CISCRP](https://legacy.ciscrp.org/making-it-clear-lay-language-summaries/) | supported | Verbatim |
| MMS + TrialAssure PLS partnership (3 Aug 2023) | [Applied Clinical Trials](https://appliedclinicaltrialsonline.com/view/trialassure-announces-ai-generative-text-partnership-with-mms) | supported | Verbatim |
| Lionbridge lay-summary translations for a global biopharma, centralised | [Lionbridge PDF](https://www.lionbridge.com/content/dam/lionbridge/pages/case-studies/global-biopharma-company-case-study/global-biopharma-company-case-study-english.pdf) | supported | PDF dated 8 Sep 2022 |
| SciencePOD "AI-Hybrid content, where a first draft is generated by AI tools …" | [SciencePOD](https://sciencepod.net/?p=380039) | supported | Date "2024" not on page |
| Weave Bio $20m Series A, $36m total, 17 Oct 2025 | [Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development) | supported | Verbatim |
| Carelane €2.6m seed, Apr 2025, Vorwerk lead, HTGF; >130 sites; medical writing | [HTGF](https://www.htgf.de/carelane-seed/) | supported | Page dated 2 Jul 2025 |
| Lay protocol synopsis "has to be submitted as part of the initial application" | [Excelya PDF](https://excelya.com/wp-content/uploads/2024/11/Lay-Summaries-for-Clinical-Trials.pdf) | supported (as vendor claim) | Brief tags the rule `[UNVERIFIED]`; correct |
| Cochrane RCT: ChatGPT-4o +1 information, +2 readability, 36 PLS | [PMID 40727555](https://europepmc.org/article/MED/40727555) | supported | Abstract |
| GPT-4 lay summaries more readable, 204 articles | [PMID 41259712](https://europepmc.org/article/MED/41259712) | supported | Abstract; accuracy also higher |
| AI saved writers >40 % time on PLS abstracts | [PMID 40183004](https://europepmc.org/article/MED/40183004) | supported | Abstract; 10 writers, 6 abstracts (minor 8) |
| Trust "a lot" 12.3 % AI-only, 39.1 % human-only; 95.0 %; 62.4 %; n = 1,010 | [PMID 42330509](https://europepmc.org/article/MED/42330509) | supported | "95.0 % want human review" slightly reworded (minor 9); authors include CISCRP founder (noted in brief) |
| "human-written PLSs lead to significantly better comprehension", 150 participants, 15 May 2025 | [arXiv 2505.10409](https://arxiv.org/abs/2505.10409) | supported | Preprint [B] correct |
| "close human supervision … quality review mechanisms need to be in place" | [EMA reflection paper](https://www.ema.europa.eu/en/documents/scientific-guideline/reflection-paper-use-artificial-intelligence-ai-medicinal-product-lifecycle_en.pdf) | supported | PDF dated 17 Sep 2024; about product information |
| Art. 50(4) text incl. "human review or editorial control … editorial responsibility" | [AI Act Art. 50](https://artificialintelligenceact.eu/article/50/) | supported | Secondary copy [B], correct |
| AI Act applies from 2 Aug 2026 (no Art. 50 exception) | [Art. 113](https://artificialintelligenceact.eu/article/113/) | supported | Amended text shown; Art. 50 not deferred |
| § 7 UWG consent rules | [buzer.de](https://www.buzer.de/7_UWG.htm) | supported | Verbatim |
| Medical Writer average €55,400 (€46,500–65,100); Berlin, Hamburg, München; 228 ads | [StepStone](https://www.stepstone.de/gehalt/Medical-Writer.html) | supported | Ads now 206 (minor 10) |
| ISO 17100 cited by a language firm | [Translated](https://translated.com/resources/medical-translation-services-pricing-healthcare-documentation-cost-analysis) | supported | Verbatim |
| Hays Lisbon "Scientific Communication & Medical Writer (M/F/D)" | [expressoemprego](https://expressoemprego.pt/emprego/scientific-communication---medical-writer-(m-f-d)/grande-lisboa/2434256) | unverifiable | Page is script-loaded; brief already says "title only" [C] |

Via-repo items (EXIST/FLÜGGE rules in `research/munich-ecosystem.md`; EMWA €82.2/h, UCLA, JVEG, competitors in C19) match the fact-checked repo files.

## Re-run counts (CTIS public API, 2026-11-19)
| Count | File | Re-run | Result |
|---|---|---|---|
| Ended trials (`status` 8) | 4,202 | 4,202 | match |
| Ended 2025 / 2026 | 1,826 / 1,562 | 1,826 / 1,562 | match |
| 2025: top-50 / other / non-commercial | 590 / 702 / 534 | 599 / 693 / 534 | ~match (keyword list, minor 4) |
| 2025 other, sponsor seat: US / EU-EEA / DE / DACH | 262 / 315 / 43 / 81 | 254 / 315 / 43 / 80 | match for EU and DE; US and DACH within 3 % |
| Sponsors: EU-EEA / DE / DACH; one-trial sponsors | 210 / 30 / 63; 367 | 210 / 30 / 62; 365 | ~match |
| Large CRO named: US other / EU other / DE other / non-commercial | 186 (71.0 %) / 85 / 13 / 23 | 178 (70.1 %) / 74 / 9 / 12 | partial (CRO list not recorded, minor 3) |
| DE other 2025: Bavaria / greater Munich | 15 / 10 | 15 / 10 (12 incl. Holzkirchen) | match |
| 2026 DACH other: trials / sponsors / no lay summary | 114 / 80 / 107 | 113 / 79 / 104 | ~match (minor 5) |
| Contractor task mentions "lay" | 3 | 0 | mismatch (minor 6) |
| Section 5 and 7 arithmetic (TAM/SAM/SOM, packs needed, writer cost, translation, margins) | — | all recompute | match (92 → 93, minor 10) |

## [UNVERIFIED] items
| Item | Treated as fact later? |
|---|---|
| €3,500 / €6,000 package price | No. Used only as labelled hypotheses in TAM/SAM and margin maths; the kill line tests it. Fair. |
| Turnaround 10 working days | No. |
| Reddit r/RegulatoryClinWriting snippet | No; counted as 0 opened threads. |
| Weave Bio–Parexel/Takeda; Certara "200 PLS"; EMWA "over 1,000"; Lisbon German-language roles; Citeline $3,000–3,500 | No. |
| 21 % employer cost, 1,600 productive hours, 10,000-character length | Used in the cost maths, labelled as assumptions next to the result. Fair. |
| ISO 17100 vendor audits; liability insurance | No. |
| Lay protocol synopsis as a second paid document | Listed as "upside not counted". Fair. |
| Who signs (sponsor vs CRO) | Labelled inference; rests on a 2018 statement and contractor lists. Fair, but it is the red team's main question. |

Unsourced claims: none material beyond critical 1. "Decision process (inference, not sourced)" and the Munich target list are labelled.
