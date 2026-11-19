# Fact-check: ventures/trial-lay-summaries/brief.md after the C29 + C30 fix round (task C31)
Date 2026-11-19 | Verdict: **pass, with caveats** (no critical issue; rule 14: no new tasks) | Sources checked: 4 of 4 new URLs opened (BGH via lexetius, IHK Bonn PDF, DIA Europe 2027 registration, Lionbridge Croma-Pharma); the 34 unchanged URLs were all opened in this morning's review (`2026-11-19-trial-lay-summaries-brief.md`) and not re-opened. Plus: full CTIS re-run (4,202 ended trials; 3,388 ended 2025–26, using the lists written in section 5) and 13 lay-summary PDFs downloaded and read (text + PDF metadata).

Scope: only what changed in commit 3103abf (C29 + C30). Business judgement is the red team's job; this is about whether the numbers and quotes hold.

**What holds.**
- **All 10 fact-check fixes are in.** The 50,000-summaries mistake is gone (Bottom line, section 6 TrialAssure row, section 8 all now say the 2023 removal names no vendor). The citation swap is right (Biogen role → Informa; Merck KGaA / UCB / CSL Behring → CISCRP/EMWA). The Bottom line now includes the arXiv comprehension result, says which study the ">40 %" comes from, and that the EMA text is about product information. The "95.0 %" wording and the EMA deadline definition match the sources.
- **The new CTIS counts reproduce exactly** once the spaced "H e x a l AG" is counted as large (as section 5 says it should be). The table below has the details: 1,826 / 653 / 639 / 534; core **427**, of which **181** name no large CRO; DACH core 50 / 26; Germany core 23 / 16; T2 **178 of 231 = 77.1 %**, 2025–26 combined 347 / 466; the phase × country table cell for cell; 2026 DACH 99 trials / 72 sponsors / 92 without a public summary; 355 of 455 sponsors with one trial. A re-run of these numbers gives the same result.
- **T1 quotes and metadata are real.** In the PDFs I downloaded: iTeos (both trials) "SIRO Medical Writing Pvt. Ltd, a clinical research organization, prepared this summary"; Carrick "This summary was prepared by Syneos Health®" (Carrick's CTIS contractors are Labcorp Central Lab, Guardant, Alderley, so no Syneos; that holds); Imcheck "created by Ipsen with the assistance of a third-party writing service provider"; PPM Services "This summary was written by the sponsor"; Sintetica (2023-504477-21-01) "This document is based on CRO template tmp-0007, v. 1.0 … CROSS Research S.A."; Synartro "TMP-CO03-00-09"; iOmx (Martinsried) PDF Author = "OpenAI"; Cutiss and Diater (2024-513834-40-01) Author = "python-docx".
- **All new arithmetic recomputes.** Translation 11,799 / 55 × €1.95–2.15 × 4 = €1,673–1,845. Writer €335–838. Total €2,008–2,683, mid €2,346. Margins 23–43 % / 55–67 %. Package table: 103 / 60 / 312 / 99 / 286 / 167 packs, and every share in the table. TAM / SAM / reachable rows. 3 × €2.3k ≈ €7.0k. Day rate €658–822. Measured lengths of 9 PDFs I read (3,000–16,900 characters, most 10,000–14,000) fit a median of 11,799.
- **The new legal quotes are verbatim.** BGH I ZR 27/08 para. 27 ("aufgrund konkreter tatsächlicher Umstände ein sachliches Interesse …"), para. 30–31 (industry custom not enough), para. 32 ("allgemeiner Sachbezug … nicht ausreicht"). IHK Bonn (PDF of 8 May 2024): usefulness does not matter (OLG Hamm 4 U 189/09), "Kundenzufriedenheitsabfrage" (KG Berlin 5 U 35/20). DIA: Connect & Discover "EUR 179 per day", "*Plus VAT", "does not include access to the full DIA Europe scientific programme". Lionbridge Croma: AI-powered readability testing and re-authoring of the SSCP laypersons' part, published 18 Nov 2025.
- **No [UNVERIFIED] item is treated as fact.** The €3,500 / €6,000 prices are still labelled hypotheses. The "research call = advertising?" question is tagged. T1's AI-trace reading is labelled *inference* and says it "does not prove that the text was written by AI".

**Does any of this change CEO decision C28? No.** The researcher now recommends (a) drop. Every check here either confirms the numbers behind that or makes them slightly stronger (caveat 2).

## Critical issues (must fix)
None.

## Caveats for the CEO (rule 14: listed, not new tasks)
1. **"11 trials from greater Munich (postcodes 80–82)" (section 3, Germany row): the re-run gives 10.** Bavaria 13 matches. Postcodes of the 40 Germany-based trials are: 80 ×1, 81 ×2, 82 ×7. This morning's review also found 10 (12 if Holzkirchen is counted, but that is Hexal, which is now in the large list). It does not matter for the decision.
2. **One of the 4 "outside writer named" trials is really large-pharma practice.** The Imcheck summary (2024-514758-65-00) is Ipsen-branded: its footer reads "Ipsen General", and it says "created by Ipsen with the assistance of a third-party writing service provider". Ipsen is on the brief's own large-company list, so this is the Advanced Accelerator Applications case again (a subsidiary under another name). Independent small sponsors buying from an outside writing firm: **2 sponsors (3 trials)**, iTeos via SIRO and Carrick via Syneos. That supports the brief's conclusion more strongly.
3. **The BGH case is quoted for its rule, but the case itself ended the other way.** On its facts the court found presumed consent and overturned the ban on the calls (para. 26, 33: the people called "den Anrufen … positiv gegenüber gestanden haben"). The quoted rule is correct and the brief's "weak legal footing" is labelled inference and "not legal advice". Just don't read the case as "B2B cold calls were banned".
4. **DIA price range (section 9).** "Full-conference rates on the page run from €1,090 (young professional) and €2,050 (SME) up to €3,350". The page also lists €3,410 and €3,610 (standard rates for some categories, e.g. "Includes …" packages) and reduced rates of €300 (students) and €370 (patients). The €179 day pass, which is what the brief uses, is correct.
5. **"€0.63–1.09m a year for all of Europe and the US together" (Bottom line, bullet 2) is loose wording.** The 181 trials are EU-authorised trials by sponsors based anywhere (US 241, Spain 60, Germany 40, France 35, Switzerland 30, UK 26 … in the 639). US trials that do not run in the EU are not in it. Read it as "the EU trial market, whoever the sponsor is".
6. **T1's random sample cannot be rebuilt from the repo.** The seed is given, but the script and its ordering are not in the repo. So I checked the named documents rather than the draw. My T1 frame is 164 trials, not 165, and 107 multi-country trials, not 108, with a median of 4 lay-summary documents per trial (matches). Diater's "python-docx" author sits on trial 2024-513834-40-01. The English summary of Diater's other trial (2024-519527-14-00) has a named person as author. Which Diater trial was in the sample is not stated.
7. **Contractor-duty count.** "0 of 6,588 free-text duty entries mention a lay summary": my re-run over all duty entries of the 2025–26 trials (19,673, coded and free-text) also finds 0. The conclusion holds; the denominator depends on which field is counted.
8. **Carried over from this morning, still true:** no observed price for a lay summary (both prices are hypotheses); AI Act text read from a secondary site; GLSP and the CISCRP 2018 statement are >3 years old; who signs (CRO vs sponsor) remains inference. The brief lists all of these in "Gaps".

## Source check (new or changed claims only)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| B2B call needs "konkreter tatsächlicher Umstände"; "allgemeiner Sachbezug" not enough; industry custom not enough (para. 27, 31–32) | [BGH I ZR 27/08, lexetius](https://lexetius.com/2010,2788) | supported | Verbatim; the case itself found consent on its facts (caveat 3) |
| IHK: usefulness irrelevant (citing BGH I ZR 191/03, OLG Hamm 4 U 189/09); satisfaction-survey calls also need consent (KG Berlin 5 U 35/20); PDF May 2024 | [IHK Bonn PDF](https://www.ihk-bonn.de/fileadmin/dokumente/Downloads/Recht_und_Steuern/Wettbewerbsrecht/WerbungTelefonBriefE-Mail.pdf) | supported | PDF created 8 May 2024 |
| DIA Europe 2027, Basel, 16–18 Mar; Connect & Discover EUR 179/day + VAT, not full programme; €1,090 / €2,050 / up to €3,350 | [DIA registration](https://www.diaglobal.org/en/flagship/dia-europe-2027/about/register) | partially | Day pass and dates verbatim; range omits €3,410 / €3,610 / €300 / €370 (caveat 4) |
| Croma-Pharma: AI-powered readability testing and re-authoring of SSCP laypersons' part by Lionbridge; published 18 Nov 2025 | [Lionbridge](https://www.lionbridge.com/case-study/croma-pharma-case-study) | supported | `datePublished` 2025-11-18; "Austrian" / "mid-size" not on the page (common knowledge, low stakes) |
| 2023 removal of AI lay summaries, no vendor named (Bottom line, s. 8) | [CISCRP/EMWA](https://www.ciscrp.org/wp-content/uploads/2025/07/11-considerations-for-use-of-ai.pdf) | supported | Checked this morning; fix applied correctly |
| T1 quotes: SIRO (iTeos ×2), Syneos (Carrick), Ipsen + third-party writer (Imcheck), "written by the sponsor" (PPM), CROSS template tmp-0007 (Sintetica), TMP-CO03 (Synartro) | CTIS public documents (downloaded 2026-11-19) | supported | Imcheck is Ipsen-branded (caveat 2) |
| PDF Author "OpenAI" (iOmx), "python-docx" (Cutiss, Diater) | CTIS public documents, `pdfinfo` | supported | iOmx text also carries "Source URL used for template drafting: …", a typical chat-tool artefact (still inference) |
| Carrick summary by Syneos though no Syneos contractor | CTIS retrieve 2023-503903-27-00 | supported | Contractors: Labcorp Central Laboratory Services, Guardant Health, Alderley Analytical |

## Re-run counts (CTIS public API, 2026-11-19; recipe and lists from section 5)
| Count | File | Re-run | Result |
|---|---|---|---|
| Ended / 2025 / 2026 | 4,202 / 1,826 / 1,562 | 4,202 / 1,826 / 1,562 | match |
| 2025 large / other / non-commercial (sponsors) | 653 (90) / 639 (455) / 534 (293) | 653 (90) / 639 (455) / 534 (293) | match (Hexal spaced name moved to large, as section 5 says) |
| Large CRO named: large / other / non-commercial | 364 / 252 / 10 | 364 / 252 / 10 | match |
| Other by seat: US / EU-EEA / DE / DACH (CRO) | 241 (155) / 295 (48) / 40 (7) / 75 (24) | 241 (155) / 295 (48) / 40 (7) / 75 (24) | match |
| One-trial sponsors | 355 | 355 | match |
| Phase × countries (BE 60/1/0; Ph I 151/25/14; II–IV 107/64/217) | as file | as file | match |
| Core / core without large CRO | 427 / 181 | 427 / 181 | match |
| DACH core / without CRO; DE core / without CRO | 50 / 26; 23 / 16 | 50 / 26; 23 / 16 | match |
| T2 by countries 1 / 2 / 3+ (2025) | 39/318, 35/90, 178/231 (77.1 %) | same | match; US / EU / DACH sub-columns match |
| T2 2025–26 combined | 66/562, 61/149, 347/466 | same | match |
| 2026 DACH other: trials / sponsors / no public summary | 99 / 72 / 92 | 99 / 72 / 92 | match |
| Germany 2025 other: Bavaria / greater Munich | 13 / 11 | 13 / 10 | Munich off by 1 (caveat 1) |
| Non-commercial seats FR / NL / ES / DE | 128 / 81 / 51 / 51 | 128 / 81 / 51 / 51 | match |
| T1 frame (EU/EEA/CH other, lay summary, 2025–26) / multi-country / median docs | 165 / 108 / 4 | 164 / 107 / 4 | ~match (caveat 6) |
| Contractor duties mentioning lay summary | 0 | 0 | match |
| Section 5, 7, 10, 13 arithmetic | — | all recompute | match |

## [UNVERIFIED] items
| Item | Treated as fact later? |
|---|---|
| €3,500 / €6,000 pack price | No; hypotheses, tested by kill lines |
| 10-day turnaround; 21 % employer cost; 1,600 h | No; labelled assumptions next to the result |
| "Research call" = advertising under § 7 UWG | No; tagged, not legal advice |
| Lay protocol synopsis as second document | No; "upside not counted" |
| Weave Bio–Parexel/Takeda, Certara 200 PLS, EMWA >1,000, Lisbon roles, Reddit snippet, Citeline price | No |
| ISO 17100 audits, liability insurance cost, BioM/EMWA fees, Basel travel | No; listed in Gaps |
| Meaning of "python-docx" / "OpenAI" metadata | No; labelled inference with the caveat that it does not prove AI wrote the text |

Unsourced claims: none material. Fabrication check: no invented quotes or interviews; every T1 quote traced to a public CTIS document.
