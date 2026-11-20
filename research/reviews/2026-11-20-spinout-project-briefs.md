# Fact-check: ventures/spinout-cofounder/project-briefs.md (C32)
Date 2026-11-20 | Verdict: **pass (minor fixes)** | Sources checked: 42 of 42 (40 downloaded and grepped; Euronews and GEN blocked curl, read via WebFetch) + 1 extra (EMA EPAR Elevidys)

Scope: the only file in `research/` or `ventures/` changed since its latest fact-check (commit 8d2ba2b, C32). Task C33. No business judgment here (red team's job).

## Critical issues (must fix)
None. No fabrication: no interviews, quotes or feedback without a traceable URL. All quoted text found verbatim in the cited source. All grant sums, dates, funding rounds, pipeline counts and the EBM fee reproduce.

## Minor issues (first round; no fix task, research is paused; researcher may apply them if the file is touched again)
1. **Wrong report label, Findings bullet 3.** "ki-alz-2's own final report puts drug companies, CROs and research sites first". The TIB PDF is the final report of the **concept phase (ki-alz, 1 Oct 2023–30 Sep 2024)**, created 14 May 2025. It is not a ki-alz-2 (feasibility phase) report; that phase's results are not public. The Details section labels it correctly ("concept-phase report"). Fix: "the concept-phase final report (2025)".
2. **Genevant–Takeda: "Most of these sums are milestones" is inference, not source.** The Pharmaceutical Technology article says Genevant "will be eligible for up to $303m upfront, as well as potential milestone payments, apart from royalties". The $303m and the Mar 2022 date hold; the milestone share is not stated there. The Repair Bio deal does support "upfront and contingent milestone payments". Label the sentence *inference*.
3. **Elevidys status is out of date.** "got a negative CHMP opinion in the EU in July 2025" is true (Roche, 25 Jul 2025), but EMA now lists Elevidys as **Refused**: opinion 24/07/2025, refusal of marketing authorisation 24/09/2025 ([EMA EPAR](https://www.ema.europa.eu/en/medicines/human/EPAR/elevidys) [A]). Use the regulator as source and say "refused in the EU (Sep 2025)".
4. **KIARA ad paraphrase is narrower than the ad.** Findings: the ad "asks for medtech sales, a hospital network and VC fundraising experience". The ad asks for "Experience in medtech, healthtech, or other complex B2B healthcare markets" with a track record in customer discovery, validation, strategy, acquisition, partnerships or revenue growth; a DACH/European healthcare network; VC and grant fundraising. It also says "Based in Germany (or willing to relocate)" and "German language proficiency is a strong advantage". These two location/language lines are missing from the brief and matter for a CEO who lives in Lisbon until Sep 2027.
5. **Small unsourced facts:** Caresyntax "Berlin/Boston" and icometrix "Leuven" are not in the cited articles. Harmless, but unsourced.
6. **Nvelop:** GEN calls the $100m a **seed** round, launched 9 Apr 2024 (WebFetch summary adds that the money was raised earlier). "$100m, Apr 2024" is fine; "seed" would be more precise.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| ki-alz-2 dates 1 Oct 2024–30 Sep 2026, €599,632.80; concept €119,993.29; "under realistic hospital conditions", "basis for a spinoff" | GO-Bio ki-alz | supported | verbatim |
| Rauchmann lead, Perneczky team; "Pharma, CROs, Forschung"; "kurzfristig über Pilotpartnerschaften …"; SaaS/licensing; class IIa | TIB report | supported | concept-phase report, PDF created 14 May 2025 (see issue 1) |
| 1.8m with dementia end 2025; 357,000 new 65+ (2023) | DAlzG factsheet | supported | |
| From 1 Apr 2026 lecanemab billed with EBM codes; GOP 11602 €53.76 | KBV | supported | 422 points / €53.76 |
| G-BA no added benefit lecanemab (19 Feb 2026); basis for price talks | Alzheimer Europe | supported | "possible withdrawal" is from PZ, not this page; both cited together, fine |
| 1,000–2,000 treated (neurologist estimate); talks ongoing; manufacturer may leave market | PZ 4 Nov 2026 | supported | |
| Donanemab no added benefit (16 Apr 2026) | PZ | supported | |
| mediaire €12m, 13 Nov 2024, >350 hospitals and clinics | HTGF | supported | |
| GE HealthCare to buy icometrix, undisclosed sum, side-effect module | MedTech Dive 11 Sep 2025 | supported | Leuven not in source (issue 5) |
| neotiv €10m, Nov 2022, CE class I | Capricorn | supported | >3 yrs, flagged |
| Roche Elecsys pTau217 CE mark, "both primary and secondary care" | Euronews 12 May 2026 | supported | via WebFetch (curl 406) |
| Rule 11 class IIa wording; non-MDSW vs MDSW modules; rev.1 June 2025 | MDCG 2019-11 rev.1 | supported | verbatim |
| STV-C8 results, mice lungs, pig dystrophin, Nature 2 Sep 2026, spin-off plan, people | Helmholtz Munich | supported | |
| EDGE €3,054,897, 1 Nov 2025–31 Oct 2028, Duchenne, "efficacy and safety analyses … clinical testing" | GO-Bio EDGE | supported | |
| "prepare for the founding of a startup", 1 Dec 2025 | Helmholtz IDG | supported | |
| GO-Bio next 15 Mar / 15 Sep; phase II company "as a rule" founded after phase I | GO-Bio next | supported | |
| Follow-on "VIP+, EXIST research transfer, KMU-innovativ or GO-Bio next" | GO-Bio initial | supported | |
| ATMP, CAT | EMA | supported | |
| Genevant–Takeda up to $303m, Mar 2022 | Pharm. Technology | partially | milestone share is inference (issue 2) |
| Genevant–Repair up to $107m per product; mid-to-high single-digit royalties; Sep 2024 | Repair Bio | supported | 26 Sep 2024 |
| 4,487 / 2,217 gene / 1,370 RNA therapies; CAR-T 66 % of GM cell therapies | Citeline Q2 2026 | supported | report dated July 2026 |
| Elevidys negative CHMP opinion Jul 2025 | Roche | supported, outdated | refused 24 Sep 2025 (issue 3) |
| Aera $193m Series A+B, Feb 2023, human proteins | BioSpace | supported | 16 Feb 2023 |
| Nvelop $100m, Apr 2024, VLPs | GEN | supported | via WebFetch (curl 403); seed (issue 6) |
| RadioGene-2 patent application, commercialise for pharma research, spin-off + contract manufacturer | GO-Bio RadioGene | supported | |
| Mice, renal clearance, specific binding; Morath, Fritschle, Weber; clinical trials needed; "laufen derzeit"; imuveo named; 13 Jun 2025; Nat Biomed Eng 2025 | TUM release | supported | |
| § 31 StrlSchG permit unless notifiable under § 32 | gesetze-im-internet | supported | |
| ImaginAb non-exclusive licence and supply to Leucid Bio, Apr 2023 | Pharm. Technology | supported | 13 Apr 2023 |
| ImaginAb $12.8m, Jun 2021 | BioSpace | supported | 3 Jun 2021 |
| imuveo founded 2022, €1.6m EFT, CD2 PET tracer | TUM Venture Labs | supported | |
| FormulAIte EFT since July 2026, 03EFBY0380, ALINA, 5 milestones, partner invitation, team | Merkel lab | supported | |
| ~€1m FormulAIte, ~€1.2m cevovec, "three researchers and one business specialist", cevovec business-development member | LMU 20 Jul 2026 | supported | Rika Neumann named for cevovec |
| ERC PoC €150,000, 1 Jan 2027–30 Jun 2028 | CORDIS | supported | |
| Mana.bio $19.5m seed Oct 2023, a16z Bio + Health co-lead | BioSpace, Calcalist | supported | |
| KIARA ad: product, live OR pilot, €35k claim with sources, profile; PDF created 25 Jun 2026 | ad PDF | supported | metadata reproduces; paraphrase narrow (issue 4) |
| KIARA and LUXONNIC still listed | LMU IEC jobs | supported | |
| KIARA project Aug 2022–Jul 2025, BMBF, consortium, lamp cameras, draft report checked and approved | Fraunhofer HHI | supported | |
| ~16.5m inpatient operations 2023 | KBV | supported | "rund 16,5 Millionen Eingriffe"; could be [A] (KBV citing Destatis), [B] is conservative |
| Caresyntax $180m Aug 2024, $100m equity, Smart OR Box | SiliconANGLE | supported | Berlin/Boston not in source (issue 5) |
| Theator $15.5m Series A, Feb 2021 | Insight Partners | supported | 9 Feb 2021 |
| Helmholtz Enterprise 2026-2 winners not listed | Helmholtz | supported | page shows "Batch I 2026" only |

Grades: correct overall. GO-Bio, CORDIS, MDCG, EMA, KBV-EBM, StrlSchG [A]; university, company, news [B]. No [C] evidence used; no market sized.

Re-run counts: no App Store / ClinicalTrials.gov / TED recipe applies. Citeline pipeline counts and the KIARA PDF date reproduce.

Inference labels: all forward-looking statements (fit, revenue timing, seat status, first-12-month work, "about 5 months open") are marked *inference*. Exception: issue 2.

## [UNVERIFIED] items
| Item | Built on later? |
|---|---|
| No price per ki-alz analysis | No; drives question 2 only |
| No billing code for AI scan analysis, hospital pays from own budget | No; KIARA's parallel statement is labelled inference |
| No price for tracer supply or licences | No |
| No public price for contract formulation work | No |
| KIARA €35,000 per surgeon per year (company claim) | No; not used in Findings or the table |
| Business-seat status in ki-alz-2, SYNTRA/EDGE, RadioGene-2 | Table says "Unknown"; correct |

Stale data (>3 years) is flagged in place: neotiv 2022, Aera 2023, Mana.bio 2023, Genevant–Takeda 2022, ImaginAb 2021/2023, Theator 2021. Nature papers not opened; disclosed.
