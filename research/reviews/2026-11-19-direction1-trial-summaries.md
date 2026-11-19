# Fact-check: research/direction1-trial-summaries.md (task C21)
Date 2026-11-19 | Verdict: **pass (minor fixes)** | Sources checked: 25 of 25 cited URLs (curl + text extraction; WebFetch for EMA, EMWA and Nasdaq), plus a full CTIS re-run (12,873 trials, 4,194 ended trials retrieved one by one) and the TED re-run

Scope: first fact-check of this file (created in C19, commit e7ca4c7). Business judgement is left to the red team. Written for task C21.

**What holds.** The CTIS recipe reproduces: **12,873** public trials, **4,194** ended. The annual flow reproduces exactly (**1,826** trials ended in 2025, **969** transitioned, **609** Germany-run, **115** Portugal-run; university 67, hospital 354, other non-commercial 113). The translation table reproduces exactly (Germany-run with a lay summary **600**, multi-country **495**; EU multi-country with a lay summary **855**, of which **667** with ≥2 documents, median **5**). The German academic on-time rates reproduce exactly (universities 18 of 22, university hospitals 21 of 28, other non-commercial 26 of 38). Every quoted price, law text and funding figure was found in its source, except one mislabel (Emory, below). The TED count (0 lay-summary notices; 9 "plain language summary" notices, all EFSA) reproduces. No fabrication.

## Critical issues (must fix)
None. No fix task added. The overdue counts differ from the critic's re-run (below), but the differences make the pool smaller, not larger, so the file's conclusion ("the overdue pool is small; no brief as framed") is strengthened rather than changed.

## Minor issues (for the researcher if the file is revised; not a task)
1. **Overdue counts reproduce only approximately (Details §2).** With the recipe as written (Category 1 adult-only excluded; deadline = end + 12 months, or end + 6 months if the trial includes 0–17-year-olds; due before 2026-11-18; CTIS sponsor-level `commercial` flag), the critic gets:

   | Count | File | Re-run 2026-11-19 |
   |---|---|---|
   | Category 1 adult-only trials excluded | 1,286 | 1,340 |
   | EU due | 1,621 | 1,591 |
   | EU on time / late / missing | 835 / 442 / 344 | 841 / 444 / 306 |
   | EU with neither summary (sponsors) | 331 (229) | 291 (200) |
   | Germany due / missing / neither | 610 / 87 / 85 | 605 / 82 / 80 |
   | Portugal due / missing / neither | 103 / 12 / 12 | 102 / 11 / 11 |

   Due counts agree within 2 %; "still missing" is 11 % lower in the re-run EU-wide and 6 % lower for Germany. The most likely cause is the Category 1 / age rule (the critic excludes 54 more trials; "+ 6 months" in §1 can be read as 6 or 18 months, and the file does not say which CTIS field it used for the trial category). A variant that keeps Category 1 trials whose 30-month embargo has passed gives Germany neither = 84, close to 85 but EU due 1,780. Record the exact category and age fields. The 2025 flow and translations use no deadline rule and match exactly, which supports this reading.
2. **Emory fee is mislabelled (Findings and §4 row 4).** The file says "$5,400 for registration plus upkeep". The [Emory memo](https://ocr.emory.edu/_includes/documents/emory-2025-industry-funded-study-fees.pdf) says "a one-time fee will apply for initial registration"; "updates, amendments, addressing ClinicalTrials.gov reviewer comments, and results reporting, if applicable, will also result in additional fees". The $5,400 also includes Emory's 35 % facilities-and-administration rate (appendix "With Facilities and Administrative Rate Applied"). So it is a **registration** fee only. Not used in the package arithmetic (which uses UCLA), so no number changes.
3. **Internal mismatch: "128 trials still missing" for academic hospitals (Findings) vs "132" in the §2 table.** One of the two is a different measure (probably "neither summary"); state which.
4. **"Weave Bio … (Oct 2025)"**: the opened page is dated 17 Oct 2025; supported. **"TrialAssure claims AI summaries for ~50,000 studies"**: the PRWeb page now returns 403 to the critic; it was checked in the C15 review, so it stays [B] via repo.
5. **Grade wording.** `[A, own count]` for the CTIS counts is fair for the data source, but given minor 1 the overdue rows are better read as "±10 %" than as exact. The EFGCP/EFPIA effort range (Feb 2022) and the Kolabtree rates (Aug 2020) are correctly flagged as >3 years old; the €2,877–8,631 band still rests on the 2022 effort estimate (stale-data caveat, not a fix).
6. **EMWA Spring 2027 (Amsterdam, 4–7 May)**: the cited EMWA page (WebFetch) shows the Autumn 2026 virtual conference (9–21 Nov 2026) and the Bologna local meeting (13 Nov 2026), but no Spring 2027 date. The file already tags the Amsterdam date `[UNVERIFIED]`; correct.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 12,873 public trials; 4,194 ended (`ctStatus` 8) | CTIS public API (search + retrieve) | match | Re-run 2026-11-19, 200 sorted pages, all 4,194 retrieved |
| Overdue: 1,621 due; 835 / 442 / 344; DE 85, PT 12 with neither | CTIS re-run | partially | 1,591; 841 / 444 / 306; DE 80, PT 11 (minor 1) |
| German universities 82 % (18/22), university hospitals 75 % (21/28) | CTIS re-run | match | Exact |
| 2025 flow 1,826 / 969 transitioned / 609 DE / 115 PT | CTIS re-run | match | Exact; top-50 584 vs 585 and other companies 708 vs 707 (keyword list) |
| Translations: 600 / 431 / 495 / 372 (DE); 855 / 667 / median 5 (EU) | CTIS re-run | match | 600, 495, 855, 667, 5 exact; German-language share not re-derived (needs title parsing) |
| "within one year … unless the trial includes paediatric participants … within 6 months"; Category 1 adult-only "published 30 months after the end of trial date"; "Results are expected for trials that have recruited participants" | [EMA CTIS portal guide](https://www.ema.europa.eu/en/documents/other/clinical-trial-information-system-ctis-public-portal-trial-results_en.pdf) | supported | Verbatim (PDF text, metadata 21 Aug 2026; curl 429, read via WebFetch download) |
| 116 of 234 on time (preprint) | [TranspariMED](https://www.transparimed.org/single-post/half-of-clinical-trials-of-medicines-in-europe-violate-new-transparency-law-new-study) | supported | Verbatim; preprint stated |
| Viracta "terminated its employees and will wind down operations", Feb 2025 | [Nasdaq/GlobeNewswire](https://nasdaq.com/press-release/viracta-therapeutics-announces-wind-down-operations-2025-02-05) | supported | Verbatim in page metadata; WebFetch 503 |
| Art. 37(4) CTR: one year, lay summary; Art. 94 penalties | [Regulation 536/2014](https://health.ec.europa.eu/system/files/2016-11/reg_2014_536_en_0.pdf) | supported | Verbatim |
| § 97 Abs. 2d Nr. 2 AMG: Art. 37(4) document "nicht, nicht richtig, nicht vollständig oder nicht rechtzeitig"; Abs. 3 "bis zu 25.000 Euro" | [buzer.de § 97 AMG](https://www.buzer.de/97_AMG.htm) | supported | Verbatim |
| "between 35 to 105 hours"; "Academic sponsor organisations have no central budget for experienced 'medical writing' staff"; "at least one language of the participants and English … the minimum" | [EFGCP/EFPIA report 2022](https://www.efpia.eu/media/636879/efgcp-efpia-report-glsp-workshop-14-15-21-february-2022-final-rev.pdf) | supported | Verbatim; >3 years old (flagged) |
| Median €82.2/h, 223 respondents | [EMWA survey](https://emwa.org/journal/freelancing/seventh-freelance-business-survey-the-freelance-landscape-2018-2023/) | supported | Verbatim (WebFetch; curl 403) |
| UCLA Option #1 $2,500 (ORA "will perform data entry"), Option #2 $1,000 (Zoom), registration $1,500; "Last updated: 11 Jun 2024" | [UCLA CTSI](https://www.researchgo.ucla.edu/clinicaltrialsgov-0) | supported | Verbatim |
| Emory $5,400 "registration plus upkeep" | [Emory memo, 10 Jul 2025](https://ocr.emory.edu/_includes/documents/emory-2025-industry-funded-study-fees.pdf) | partially | One-time registration fee incl. 35 % F&A; upkeep and results extra (minor 2) |
| "£200 per summary", 500–750 words, charities | [Richard Berks](https://richardberks.co.uk/services/lay-summaries/) | supported | Verbatim |
| Clinical writer "USD 40-60 per hour", experienced "above USD 80", regulatory "USD 100 and above"; 14 Aug 2020 | [Kolabtree](https://www.kolabtree.com/blog/how-much-does-it-cost-to-hire-a-freelance-medical-writer/) | supported | Verbatim; date in page metadata |
| § 11 JVEG €1.95 per 55 Anschläge; €2.15 if "besonders erschwert" | [buzer.de § 11 JVEG](https://www.buzer.de/11_JVEG.htm) | supported | €2.15 also applies to non-editable text; "Fachausdrücke" qualify as difficult |
| Weave Bio $20m Series A, $36m total, USVP lead, Oct 2025 | [Pulse 2.0](https://pulse2.com/weave-bio-20-million-series-a-closed-for-expanding-ai-native-regulatory-platform-for-global-drug-development) | supported | Dated 17 Oct 2025 |
| Indegene acquires Trilogy (Frankfurt), 27 Mar 2024, "Generative AI" | [Samedan](https://www.samedanltd.com/press-releases/indegene-acquires-trilogy-writing-consulting-gmbh-a-medical-writing-consultancy/) | supported | Verbatim |
| Peer AI $12.1m | [eeNews Europe](https://www.eenewseurope.com/en/peer-ai-raises-12-1m-to-speed-up-drug-approvals-with-agentic-ai) | supported | Verbatim |
| Yseop: Novartis dRx Capital, Eli Lilly; "more than 150 clinical trials" | [Yseop](https://yseop.com/news-and-press-releases/yseop-announces-strategic-investment-and-celebrates-milestone-of-150-clinical-trials-powered-by-generative-ai/) | supported | Verbatim |
| TrialAssure ~50,000 | [PRWeb](https://www.prweb.com/releases/trialassure-uses-artificial-intelligence-to-create-plain-language-summaries-for-50-000-studies-listed-on-clinicaltrialsgov-301960306.html) | unverifiable today | 403; checked in C15 review |
| Narrativa $1.3m (2021) | [PR Newswire](https://prnewswire.com/news-releases/narrativa-raises-an-additional-1-3m-to-help-pharma-companies-accelerate-the-fda-drug-approval-process-through-artificial-intelligence-natural-language-generation-301292601.html) | supported | Title |
| Quanticate: CTIS lay summaries, "Translation of summaries into local languages" | [Quanticate](https://www.quanticate.com/lay-summaries-services) | supported | Verbatim |
| Clinbay "at a cost-effective price" | [Clinbay](https://www.clinbay.com/layperson-summaries) | supported | Verbatim |
| "the EU CTR does not request translations" | [GLSP](https://health.ec.europa.eu/system/files/2021-10/glsp_en_0.pdf) | supported | Verbatim |
| Lei 9/2026, in force 5 Apr 2026; €5,000–750,000 for companies, "entre outras", incl. "incumprimento das obrigações de notificação" | [Abreu Advogados](https://abreuadvogados.com/wp-content/uploads/2026/03/NL-Novo-regime-dos-ensaios-clinicos-PT.pdf) | supported | Verbatim; late results not listed (file says unconfirmed) |
| DIA Europe 2027, Basel, 16–18 March | [DIA](https://connect.diaglobal.org/dia-europe-2027-newsletter) | supported | Verbatim |
| PtCRIN, Portuguese ECRIN partner | [ECRIN](https://ecrin.org/news/get-know-our-national-partner-ptcrin) | supported | Coimbra meeting is snippet-only (file says so) |
| EMWA Autumn 2026 virtual 9–21 Nov; Bologna 13 Nov 2026 | [EMWA](https://emwa.org/conference/spring-conference-2027/) | supported | WebFetch; Spring 2027 date not on page (minor 6) |

## Re-run counts
| Recipe | File | Re-run 2026-11-19 | Result |
|---|---|---|---|
| CTIS search, 2 × 100 pages sorted by decisionDate | 12,873 | 12,873 | match |
| `ctStatus` 8 | 4,194 | 4,194 | match |
| Overdue (Details §1–2) | see minor 1 | see minor 1 | partial mismatch (≤2 % due; 6–11 % missing) |
| 2025 flow (Details §3) | 1,826 / 969 / 609 / 115 | same | match |
| Lay-summary documents (Details §7) | 600 / 495 / 855 / 667 / median 5 | same | match |
| TED `FT~"lay summary"`, `"lay summaries"`, `"Laienzusammenfassung"`, `"plain language summary"` | 0 / 0 / 0 / 9 (EFSA) | 0 / 0 / 0 / 9 (all EFSA) | match |
| My-math: 35/105 × €82.2; 10,000/55 × €1.95 / €2.15; €360k and €1m / €6,000; shares of 707 and 239 | €2,877–8,631; €355 / €391; 60 / 167; 8.5 % / 23.6 %; 25 % / 70 % | same | match |
| Table sums in §2, §3, §7 | — | all rows add up | match |

## [UNVERIFIED] items
| Item | Treated as fact later? |
|---|---|
| Seelos Chapter 11 (snippet) | No; tagged in Findings and Gaps. |
| Citeline $3,000–3,500; Taylor & Francis $5,940; Artos; Certara; CISCRP; TrialSummaries | No; excluded from the package price. |
| Lay-summary length ~10,000 characters | Used in the translation math, but labelled as an assumption next to the result. Fair. |
| €6,000 package price in K3 | Labelled `[UNVERIFIED]` as a price anyone pays; K3 is presented as *my math*. Fair. |
| Portuguese fines for late results; German enforcement case | No. |
| EMWA Spring 2027 Amsterdam | No. |

Unsourced claims: none material. "Inference" labels are used for the customer and price conclusions.
