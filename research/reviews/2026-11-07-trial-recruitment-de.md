# Fact-check: research/trial-recruitment-de.md (A13)
Date: 2026-11-07 | Verdict: pass (minor fixes) | Sources checked: 33 of 41 listed URLs/APIs opened or re-run; the rest not opened (see below)

Method: re-ran the CTIS and ClinicalTrials.gov counts, re-queried TED, re-opened the vfa decks/press releases/paper, buzer law texts, Europe PMC records, vendor pages. Numbers were normalised before matching.

## Critical issues (must fix)
None. No fabricated quote, no unsourced interview. Counts reproduce.

## Issues to fix (non-critical)
1. **Unverified deal stated as fact in Findings.** Findings bullet: "TriNetX owns Clinerion (13,000+ sites, by its own site)". Details §6 and Gaps say the TriNetX takeover is "snippet-level only". The one opened source (startupticker, 1 Feb 2023) says **Citeline (Norstella)** bought Clinerion. trinetx.com does not mention Clinerion; only the clinerion.com redirect to trinetx.com/contact-us is observed. The "13,000 sites" is TriNetX's own network, not Clinerion's. Treat as `[UNVERIFIED]`. The statement also propagates into `research/pain-industry.md` I1/"Competition [B] (verified in A13)", which then calls it verified.
2. **Selective comparison.** "Germany has the most single-country commercial trials ... 96 in 2025, against Spain 93, Belgium 45, France 29". The Netherlands has 55 (more than Belgium/France). "Every year" holds (re-run: 2023 71 vs 55; 2024 127 vs 79; 2026 100 vs 82), but the list of runners-up skips the third place.
3. **Munich count drifts.** "Recruiting with a site in 'Munich OR München': 307, of 1,115 recruiting in Germany". Re-run today: 314 (1,115 matches). Likely a data update; state the date or use "~300".
4. **Misstated base.** "Investigator-sponsored RCTs (93 trials, 22 German) ... 69.7 % exceeded their budget by >50 %". PubMed abstract: 46 of the **66 RCTs with an available budget** (69.7 %), not of 93.
5. **Second-hand claim correctly flagged but used in text.** DGPharMed ">two thirds declined" is in Gaps as `[UNVERIFIED]`/second-hand; the paper does say it (kap.pdf). Fine, but keep it out of any sizing.
6. **Inference "8.5 % discount applies to every GKV sale for 3 years".** § 130a Abs. 1c: the exemption lasts 3 years (renewable). Abs. 1b has no 3-year limit; the discount applies as long as there is no exemption. Rephrase.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| CTIS 12,788 trials, 4,653 transitioned | CTIS API (re-run) | **supported, exact** | totals match both |
| CTIS table 2023–2026 (DE/ES/FR/IT/PL, DE-only), phase mix, non-commercial 109/876, FR 246, ES 166 | CTIS API (re-run, same exclusion and year rules) | **supported, exact** | all 4 rows and 2025 detail identical |
| CT.gov: DE starts 613 (2024), 622/5,912 (2025), 387/5,885 (2026); active DE 2,397; recruiting DE 1,115 | CT.gov v2 (re-run) | supported | Munich 307 vs 314 today |
| Germany 2.9 % of participants 2024; unchanged 2026; no reliable source quote | vfa Sep 2026 deck p. 3, 10, 11 | supported | deck footnote: share is "abgeschätzt" from CT.gov + Clarivate survey |
| 72 % / 68 % miss plan, 37 % / 39 % recruit nobody, 59 % place fewer, 77.8/59.3/29.6/18.5 %, +15, +7, -22, 38 %, 61 %, 24 + 25 respondents | vfa Sep 2026 deck | supported | |
| "Fehlende Patienten" most-cited reason | deck p. 15 | supported | |
| Site survey N=169, 46/38/13 %, hurdles 64/74/50, 17/50/32, 4/9/5, by volume 3/5/13 % | vfa Jan 2026 deck p. 11–14 (opened p. 14 as image) | supported | CRO column (n=5, 20 % identification) is omitted; fine, tiny n |
| 53 % hiring, 13 % can fill, 68 % expect growth, 57 % / 28 % digital, 43 % invest, 62/36/40 | Jan deck | supported | |
| MIRACUM CTRSS: 6 hospitals, 29 trials, 814 weeks, no significant change | Europe PMC 42963362 (npj Digit Med, 30 Oct 2026) | supported | quotes match |
| GP survey: 62 respondents, 7.2 %, 88.7/58.1/56.4 % | Europe PMC 42607998 | supported | |
| J Clin Epidemiol 2024: 93 RCTs, median $645,824 | Europe PMC 39307405 | supported | 69.7 % base misstated (issue 4) |
| § 130a Abs. 1b 8.5 % from 1 Jan 2027; 1c exemption at ≥5 %, application after marketing application, decision in 3 months, 3 years, renewable | buzer § 130a | supported | |
| BStabG deletes § 35a Abs. 3 S. 4–6 | buzer BStabG Art. 1 | supported | |
| G-BA module 3.6 / Tabelle 3.11 | G-BA Fachnews 160 | supported | |
| BfArM portal live; extended Standortklausel has no legal basis | PZ 22 Oct 2026 | supported | |
| Standortklausel 2 % rising to 4 %; base discount 15.5 % | vfa PM 29 Sep 2026 | supported | |
| "fast das Doppelte"; "könnten sich abwenden" | vfa PM 28 Sep 2026 | supported | |
| PROUD: ~3.0 %, phase I -10 %, gene/cell -39 % | vfa PM 12 Oct 2026 | supported | |
| Kapazitätsinitiative: 3 funding lines, monitor, gGmbH, Swetrial 60m SEK (≈ €5.4m), DGPharMed >2/3, "Berlin, München, September 2026" | vfa paper | supported | paper gives "60 Millionen SEK (ca. 5.4 Mill. €)" |
| Costing recommendations: KIS/AIS queries, quarterly, no overhead %, 163 days/1,304 h, non-binding for antitrust reasons, separate feasibility contract | Marburg PDF (5 May 2025) | supported | |
| PEI 809 / 805 applications | Ärzteblatt | supported | |
| TED: 560504-2025 BSI €2,272,781 1 bid; 692140-2025 BSI Switzerland 4 bids no value; 98115-2026 IQVIA €530,858.75; 787981-2023 Cloud9 3 bids; 76572-2024 criteria (≥100 staff, KKS reference); 487103-2024 "Siehe Vergabeunterlagen" | TED API | supported | bid counts from `received-submissions-type-val` |
| Clariness–SubjectWell Jan 2026, ">42,000 randomizations", ">10,000 research sites", WindRose | Pulse 2.0 | supported | "Berlin roots" not checked |
| Viomedo "largest search engine for clinical trials in Germany" (Dec 2018) | healthcapital | supported | |
| ClinLife 1.342.192 patients / 2.567 sites | clinlife.de | supported | |
| Trialbee 6,000+ sites / 50 countries / 1.6M pre-screeners; Inato 25+ sponsors / 6,000+ sites | vendor sites | supported | vendor claims |
| TriNetX 13,000+ sites; Clinerion 10,340 orgs / 24 countries (2022), Citeline Feb 2023 | trinetx.com; startupticker | supported as figures | ownership claim: see issue 1 |
| MPIRIQ €99/159/329, setup €599, 24/12-month terms, "from 1 August 2026", +1.2M visits | mpiriq.de | supported | |
| MPIRIQ founded spring 2024, Munich | Munich Startup | supported | $3.2M seed is `[UNVERIFIED]` in text |
| Climedo ADC, "2 Mio.+", profitable before late-2021 round, AI investment "lässt oftmals auf sich warten" | climedo.de; Munich Startup | supported | |
| Rivia €13M (Mar 2026), €3M seed Jun 2024 | TNW | supported | |
| FDPG open to non-MII in pilot, >30 DIZ; recruIT 16 Apr 2025 | Ärzteblatt; TU Dresden | supported | |
| vfa 2013 position paper "up to 60 %" overhead | vfa PDF | unverifiable | PDF not readable as text this run |

Not opened: Probando, Carelane, Ancora, iduneo (blocked; flagged in text), Massive Bio, Norstella, vfa Oct 2025 deck in full.

## [UNVERIFIED] items
- Listed in the file: DGPharMed survey (second-hand), MPIRIQ funding, Carelane/Ancora/Probando/iduneo funding, TriNetX–Clinerion deal. None is used for sizing. **Exception:** the TriNetX–Clinerion ownership is stated as fact in the Findings (issue 1).

## Other checks
- Grades: own CTIS/CT.gov counts tagged [A]; vfa/BPI/BVMA decks [B] (interest-group surveys: correct, caveat stated). Vendor claims [B] with "vendor claim" note. Fine.
- Stale data: 2013 vfa paper marked >3 years old; Clinerion 2022 figure dated. Fine.
- No quote without URL. [C] section honestly reports 0 signals.
