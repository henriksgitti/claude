# Clinical-trial recruitment in Germany: site economics, vendors, Kapazitätsinitiative 2030
Task: A13 | Date: 2026-11-07 | Status: draft

Follow-up to I1/I2 in `research/pain-industry.md` and to the critic review `research/reviews/2026-11-06-pain-industry.md` (vendors snippet-only; CTMS count is not recruitment competition; site-side view missing). Methods: own count of all 12,788 public CTIS trials (CTIS public search API, pulled 2026-11-07); ClinicalTrials.gov v2 API; law text via buzer.de; the vfa/BPI/BVMA barometer decks (Oct 2025, Jan 2026, Sep 2026) and the Kapazitätsinitiative paper read in full; TED API v3 award notices; vendor websites fetched with curl. Grades follow `CLAUDE.md` rule 2.

## Findings
- **Germany is not short of trials. It is short of patients per trial.** In my CTIS count, Germany takes part in **668 of 1,356 (49.3 %)** new commercial EU trials authorised in 2025, and in 626 of 1,280 (48.9 %) in 2026 so far. Only Spain is higher (781, 57.6 %) [A, own count]. Yet the associations estimate Germany's share of trial participants worldwide at **"ca. 2,9 %" for 2024**, and say it is unchanged in 2026 [B] ([vfa Sep 2026 deck](https://www.vfa.de/download/studienstandort-barometer-sep-2026-praesentation.pdf)). *Inference:* the gap is in recruitment at each site, not in getting trials placed.
- **Sponsors and sites name different causes.** In oncology, 72 % of university sites and 68 % of large hospitals miss their recruitment plan by ≥25 %. "Fehlende Patienten" is the reason cited most often, and 59 % of companies then place fewer trials at that site [B] (Sep 2026 deck, sponsor/CRO survey). But in the associations' own **site survey (N=169, Jan 2026)**, only **4 % of practices, 9 % of university hospitals and 5 % of other hospitals** call patient identification a big hurdle. Staffing/funding is the big hurdle for 64 %, 74 % and 50 % of them. Missing digital systems is a big hurdle for 50 % of university hospitals [B] ([vfa Jan 2026 deck](https://www.vfa.de/download/studienstandort-barometer-jan-2026-praesentation.pdf), p. 14).
- **Hospital-data "patient-finder" software has not yet shown an effect in Germany.** A 2026 study tested two EHR-based recruitment support systems at six MIRACUM university hospitals (29 trials, 814 observation weeks). It found "neither a statistically significant immediate level change nor a statistically significant post-implementation slope change in weekly enrollments" [A] ([npj Digit Med 2026, PMID 42963362](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42963362%20AND%20SRC:MED&format=json&resultType=core)). The public infrastructure (MII/FDPG feasibility queries, NUM recruIT) is free to academic users.
- **The 5 % rule is now a cash incentive from 2027, with a high bar.** The BStabG (in force 30 Jul 2026) deleted the MFG's G-BA 5 % finding (§ 35a Abs. 3 S. 4–6 SGB V). It replaced it with § 130a Abs. 1c: new active substances launched from 1 Jan 2027 can be exempted by the BfArM from the new **8.5 % extra manufacturer discount** if ≥5 % of trial participants were at German sites. The exemption lasts 3 years and can be renewed [A] ([§ 130a SGB V, buzer](https://www.buzer.de/130a_SGB_V.htm); [BStabG Art. 1](https://www.buzer.de/gesetz/17632/a340690.htm)). 5 % is "fast das Doppelte" of today's average German share [B] ([vfa PM 28 Sep 2026](https://www.vfa.de/download/pg-010-2026.pdf)). The BfArM application portal is live [B] ([PZ, 22 Oct 2026](https://www.pharmazeutische-zeitung.de/hersteller-koennen-befreiung-von-zusatzabschlag-beantragen-171330/seite/2/)). No uptake figures exist yet.
- **The Kapazitätsinitiative 2030 is a lobby demand, not a programme.** BPI, BVMA and vfa propose a federal–state programme with three funding lines: staff, trial-office structures, and "Rekrutierungskapazität" (systematic patient identification, digital trial registers, regional hospitals and practices). It would come with a national capacity monitor and possibly a "Trial Nation Germany gGmbH". The paper names **no budget, no timeline and no government commitment**. Its only money reference is Sweden's Swetrial at "ca. 5.4 Mill. €" a year [B] ([paper, Sep 2026](https://www.vfa.de/kapazitaetsinitiative-klinische-forschung.pdf)).
- **Sponsors pay sites for patient identification, but no public per-patient fee exists.** The 2025 joint costing recommendations (MFT, VUD, KKS-Netzwerk, vfa, BPI, BVMA) list "Suche nach bzw. Identifizierung von potenziellen Studienteilnehmern (z. B. … Abfragen aus Klinikinformationssystem (KIS), Arztinformationssystem (AIS) …)" as a billable continuous activity, paid quarterly. Pre-contract screening for feasibility can be billed separately [B] ([Empfehlungen, Stand 5 May 2025](https://www.uni-marburg.de/de/fb20/bereiche/kks/aktuellesordner/nachrichten/klinische_pruefungen_empfehlungen_zur_gesamtleistungsrechnung_2-0.pdf)). Euro amounts per patient are not published `[gap]`.
- **Competition is consolidated and well funded, and a Munich startup already sells to practices.**
  - Clariness (Berlin roots; owns Viomedo/ClinLife since 2018) merged with SubjectWell in Jan 2026 under PE owner WindRose. It claims ">42,000 randomizations" and ">10,000 research sites" [B] ([Pulse 2.0](https://pulse2.com/clariness-and-subjectwell-merge-to-form-full-service-patient-recruitment-platform)).
  - TriNetX owns Clinerion (13,000+ sites, by its own site).
  - **MPIRIQ (Munich, founded 2024)** sells a practice-software-connected "Trial Navigator" to GPs and specialists at **€99–329 per month**, with a pharma data offer on the side [B] ([mpiriq.de/pricing](https://www.mpiriq.de/pricing)).

## Details

### 1. Trial counts: CTIS (EU) and ClinicalTrials.gov (global)
**CTIS own count [A].**
- Method: I pulled all 12,788 public CTIS trials via `POST euclinicaltrials.eu/ctis-public-api/search` (two sorted passes of 10,000 to get around the result cap, de-duplicated by CT number). I excluded the 4,653 trials transitioned from EudraCT (`isTransitioned=true`).
- "Year" = year of the first member-state decision. "Commercial" = sponsor type contains "Pharmaceutical company", "Industry" or "SME". 2026 = 1 Jan to 6 Nov.
- Caveat: CTIS shows only authorised trials. The first decision date approximates the start date.

| Year | New commercial trials | with DE | DE share | ES | FR | IT | PL | DE-only (single country) |
|---|---|---|---|---|---|---|---|---|
| 2023 | 904 | 445 | 49.2 % | 501 | 372 | 364 | 302 | 71 |
| 2024 | 1,417 | 672 | 47.4 % | 757 | 577 | 555 | 488 | 127 |
| 2025 | 1,356 | 668 | 49.3 % | 781 | 571 | 560 | 499 | 96 |
| 2026 YTD | 1,280 | 626 | 48.9 % | 720 | 539 | 507 | 470 | 100 |

- Germany has the most single-country commercial trials in the EU every year: 96 in 2025, against Spain 93, Belgium 45, France 29 [A, own count].
- Phase mix of commercial trials with DE in 2025: 288 Phase III, 175 Phase II, 100 Phase I (61 "other" + 39 first-in-human) [A, own count].
- Non-commercial trials: Germany takes part in 109 of 876 (12.4 %) in 2025, against France 246 (28.1 %) and Spain 166 (19.0 %) [A, own count]. *Inference:* CTIS covers only drug trials, and much German academic research is non-drug, so this partly reflects scope, not weakness alone.
- Applications to German authorities: PEI reports 809 applications for clinical trials in Germany in 2024 (805 in 2023) [B] ([Ärzteblatt, 29 Oct 2025](https://www.aerzteblatt.de/news/paul-ehrlich-institut-leichter-zuwachs-bei-antragen-auf-klinische-prufungen-3db64753-f916-4a99-ac0c-c419bae388b0)).

**ClinicalTrials.gov v2 API, queried 2026-11-07 [A].** Industry lead sponsor, interventional studies.
- Starts with a German site: 613 in 2024 and 622 of 5,912 in 2025 (10.5 %). 2026 so far: 387 of 5,885. The 2026 figure is not comparable: German sites are often added after first registration.
- Active (recruiting, active-not-recruiting or by invitation) with a German site: 2,397. Recruiting with a site in "Munich OR München": 307, of 1,115 recruiting in Germany. Caveat: city and country filters do not bind to the same site (see `research/sources-map.md`).
- *Inference, order of magnitude only:* ~24,000 German participants in 2024 (1st barometer, see `pain-industry.md` I1) spread over ~2,400 active industry trials is about 10 per trial. The two figures are from different time points.

**Barometer share figures [B].**
- The Sep 2026 deck: "Anteil Studienteilnehmender in Deutschland im Jahr 2024 … ca. 2,9 %" and "Stand 2026 steigt der Anteil … nicht" (p. 11).
- Fraunhofer/vfa PROUD: the share "stagniert bei rund 3,0 Prozent"; phase I trials −10 %, gene and cell therapy trials −39 % ([vfa PM 12 Oct 2026](https://www.vfa.de/download/pg-012-2026.pdf)).
- Method caveat stated by the associations: "Es gibt keine verlässliche Quelle, welche die tatsächliche Rekrutierung deutscher Studienteilnehmender liefert" (Sep 2026 deck, p. 10).

### 2. Where recruitment fails: sponsor view vs site view
**Sponsor/CRO survey, 3rd barometer (Aug–Sep 2026; 24 pharma companies + 25 CROs; published 28 Sep 2026) [B]** ([deck](https://www.vfa.de/download/studienstandort-barometer-sep-2026-praesentation.pdf), [PM](https://www.vfa.de/download/pg-010-2026.pdf)).
- Barometer +15 (January: +31); 12-month outlook +7 (January: +34). Large CROs expect a decline (−22). Pharma companies are positive (+42 current).
- Oncology:
  - 83 % of university sites make a high or very high contribution to recruitment.
  - 72 % of university hospitals and 68 % of large hospitals miss their plan by ≥25 %.
  - 37 % of group practices and 39 % of single practices recruit nobody.
- Cardiovascular/metabolic: recruitment is spread more widely across hospitals and practices. Most sites are 5–25 % below plan.
- Reasons sites gave for missing targets (sponsor-reported heat map, p. 16): "Fehlende Patienten sind der meistgenannte Grund – über alle Zentrumstypen." At university and large hospitals, "dominiert der Mangel an Studienpersonal". In outpatient settings, complex design and low funding add to this.
- Consequences in oncology: 77.8 % of companies analyse the barriers, 59.3 % place fewer trials at the site, 29.6 % place future trials only at known top recruiters, and 18.5 % place no further trials there.
- BStabG: 38 % expect more trial placement, but just as many expect "kritische Überprüfung einer Beteiligung Deutschlands". 61 % of small CROs expect such a review.

**Site survey, 2nd barometer (N=169 sites, 9–23 Jan 2026) [B]** ([deck](https://www.vfa.de/download/studienstandort-barometer-jan-2026-praesentation.pdf), pp. 11–19).
- Respondents: 46 % practices / practice networks, 38 % university hospitals, 13 % non-university hospitals.
- Staff: 53 % are hiring; "nur 13% glauben, dass sie die offenen Stellen in naher Zukunft besetzen können"; 68 % expect their staff needs to grow within 5 years. Hardest to fill: study coordinators and investigators.
- Digital: 57 % rate their digital systems as medium and 28 % as (very) low. "Nur 43% planen kurzfristige Investitionen" (62 % of large centres, 36 % of medium, 40 % of small). Planned investments go "am meisten in der Workflowautomatisierung und der Integration von Systemen".
- What would help most with digitisation: "1. Softwarelösungen und Tools 2. Personelle Ressourcen für Implementierung und Betrieb …".
- Patient recruitment: "Informationen zu Studienprogrammen sowie die Rekrutierung von Patienten werden von der Mehrheit als kein/geringes Hindernis wahrgenommen".

| Big or very big hurdle (share of sites) | Practice | University hospital | Non-university hospital |
|---|---|---|---|
| Staffing / funding | 64 % | 74 % | 50 % |
| Missing digital systems / processes | 17 % | 50 % | 32 % |
| Patient identification | 4 % | 9 % | 5 % |

By trial volume, patient identification is a big hurdle for 3 % (1–5 trials), 5 % (6–20) and 13 % (>20 trials) of sites (p. 14).

**Reading the two surveys together.** *Inference:*
- Sponsors' "fehlende Patienten" mostly means too few eligible patients in a site's catchment, plus optimistic feasibility. The deck itself says "Die Rekrutierungsplanung ist in der Onkologie durchgängig zu optimistisch".
- Sites do not see finding patients inside their own records as their problem; their problem is staff time.
- A tool that only searches the site's own EHR addresses neither. Tools that (a) widen the catchment (referrals from practices) or (b) save coordinator time fit the stated pain better.
- Both surveys are run by the same interest groups. The first barometer (Oct 2025) said "Digitalisierungsdefizite … gelten … als geringes Hemmnis" for sponsors (`pain-industry.md` I1). The Kapazitätsinitiative paper says the barometer names "Defizite der Digitalisierung" among "die größten Hemmnisse". The sponsor and site views differ.

**Independent evidence [A].**
- MIRACUM CTRSS evaluation (npj Digit Med, Oct 2026; 6 university hospitals, systems recruIT and KAS+): no significant pooled effect on weekly enrolment. Effects were "highly heterogeneous". The eligibility logic used mostly diagnosis, age and visit data; "laboratory values and structured observations were seldom available". The authors conclude that benefit depends on "iterative computable phenotyping and local workflow fit rather than a simple 'switch-on' effect" ([PMID 42963362](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42963362%20AND%20SRC:MED&format=json&resultType=core)).
- GP practices (Gesundheitswesen, Sep 2026; 62 respondents, 7.2 % response rate): the barriers are "high administrative and time burden (88.7%), insufficient remuneration (58.1%), and staff shortages (56.4%)". The proposed fixes include "simplified digital study logistics" ([PMID 42607998](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42607998%20AND%20SRC:MED&format=json&resultType=core)).
- Older reasons (DE/CH/CA interviews from 2015–16, >3 years old): "overoptimistic recruitment estimates, too narrow eligibility criteria" (Trials 2021, `pain-industry.md` I1).

**Capacity refusals.** The Kapazitätsinitiative paper cites a DGPharMed site survey: over two thirds of sites declined at least one more commercial trial in 2024/25 "auch aus Kapazitätsgründen" [B, second-hand]. The original survey was not found `[UNVERIFIED]`.

### 3. The 5 % rule: rules and uptake
| Version | Rule | Status |
|---|---|---|
| MFG (in force 30 Oct 2024) | For drugs launched from 1 Jan 2025, the G-BA states in its benefit assessment whether ≥5 % of trial participants were at German sites. Dossier module 3, section 3.6 must list recruitment by country and site (SAS extract). Only registered trials with completed recruitment count; non-interventional studies are excluded [A] ([G-BA Fachnews, 5 Dec 2024](https://www.g-ba.de/service/fachnews/160/); [MFG Art. 6](https://www.buzer.de/gesetz/16657/a319278.htm)) | **Deleted** by the BStabG (Art. 1: "§ 35a … Absatz 3 Satz 4 bis 6 wird gestrichen") [A] ([BStabG Art. 1](https://www.buzer.de/gesetz/17632/a340690.htm)) |
| BStabG (in force 30 Jul 2026) | From 1 Jan 2027, a new extra discount of **8.5 %** applies (§ 130a Abs. 1b). New active substances launched from 1 Jan 2027 can apply to the BfArM for exemption if the trial-participant share at German sites is "mindestens 5 Prozent" (§ 130a Abs. 1c). Apply no earlier than the marketing application; decision within 3 months; valid 3 years, renewable on application [A] ([§ 130a](https://www.buzer.de/130a_SGB_V.htm)) | In force; BfArM portal live (PZ, 22 Oct 2026) [B] |
| "Erweiterte Standortklausel" (proposal) | The expert commission recommends a German patient share of at least 2 %, rising to 4 %, as the precondition. Collective-agreement coverage, R&D and production would then reduce the discount further [B] ([vfa PM 29 Sep 2026](https://www.vfa.de/download/pg-011-2026.pdf)) | **No legal basis yet**; with BMG/BMWE; likely needs EU notification [B] (PZ, 22 Oct 2026) |

- Uptake: no count of G-BA "relevant share" findings (2025–Jul 2026) or BfArM exemptions was found `[gap]`.
- Math: 5 % ÷ 2.9 % = 1.72, so a company at today's average German share would need ~72 % more German patients in its programme.
- *Inference:* the rule gives sponsors a direct euro reason to buy German recruitment for drugs launching from 2027. The 8.5 % discount applies to every GKV sale for 3 years. But the vfa warns firms "könnten sich abwenden, wenn sich deren Konditionen als unerreichbar erweisen" [B] (PM 28 Sep 2026).

### 4. Kapazitätsinitiative Klinische Forschung 2030 [B]
Source: the 10-page paper by BPI, BVMA and vfa, "Berlin, München, September 2026" ([PDF](https://www.vfa.de/kapazitaetsinitiative-klinische-forschung.pdf)).
- **Ask:** "ein dauerhaft finanziertes Bund-Länder-Programm „Klinische Forschungskapazitäten 2030“", led by the Chancellery and linked to the pharma and medtech strategy. BMG and BMFTR would implement it, possibly through a joint gGmbH, using NUM structures.
- **Three funding lines:**
  1. Staff: coordinators, investigators, data management, trial pharmacies.
  2. Structures: "Professionelle Clinical Trial Offices, zentralisierte Vertragsanbahnung, Feasibility, Budgetierung …".
  3. "Rekrutierungskapazität …: Systematische Identifikation geeigneter Patientinnen und Patienten, digitale Studienregister und umfassende Einbindung regionaler Krankenhäuser und Praxen".
- **Monitoring:** a "Nationaler Kapazitätsmonitor": staff, vacancies, active and declined trials, time from site selection to initiation, recruitment per site. "Bislang fehlt eine solche belastbare bundesweite Kapazitätsstatistik."
- **Agency:** a possible "Trial Nation Germany gGmbH" for nationwide feasibility queries and "überregionale Feasibility- und Rekrutierungsnetzwerke".
- **Missing:** no euro amount, no start date and no ministry response. The paper is a proposal from interest groups.
- *Inference:* for a startup it is at best a future grant or tender channel (2027+). Its funding lines would also strengthen public, non-commercial alternatives (NUM, KKS, FDPG).

### 5. Site economics: who pays the site, and for what
- **Costing principle [B].** The joint recommendations (Stand 5 May 2025; MFT, VUD, KKS-Netzwerk, vfa, with BPI and BVMA) set out a full-cost, "Leistung/Gegenleistung" model.
  - Overheads are priced into hourly rates ("ein prozentualer Aufschlag … würde … zuwiderlaufen"). Example basis: 163 working days = 1,304 hours per year.
  - Non-binding "aus kartellrechtlichen Gründen".
  - Billable recruitment items: KIS/AIS queries, tumour-board presentations, informing the sponsor about non-inclusion reasons, campaigns and ads, paid "quartalsweise". Pre-contract feasibility screening can be billed in a separate contract ([PDF](https://www.uni-marburg.de/de/fb20/bereiche/kks/aktuellesordner/nachrichten/klinische_pruefungen_empfehlungen_zur_gesamtleistungsrechnung_2-0.pdf)).
- **Contracts [B].** The binding standard contract clauses (StandVKlV) apply from 18 Dec 2025, but they leave the amount of pay to the recommendations above (`pain-industry.md` I2).
- **Older conflict [B, 2013, >3 years old].** The vfa complained that university hospitals demanded overhead surcharges "of up to 60%" ([vfa position paper, 2013](https://www.vfa.de/embed/position-paper-cost-development-for-clinical-trials-in-germany)). The 2025 recommendations settle this on hourly rates.
- **Per-patient fees: not public.** No German source states a euro amount per enrolled patient (searched DE + EN, 4 queries). Investigator-sponsored RCTs (93 trials, 22 German): median total cost $645,824, and 69.7 % exceeded their budget by >50 %. These are academic costs, not site fees [A] ([J Clin Epidemiol 2024, PMID 39307405](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:39307405%20AND%20SRC:MED&format=json&resultType=core)).
- **What sites buy themselves (TED award notices) [A].** This is trial-management software, not recruitment tools. Barriers are high:

| Buyer | What | Winner | Value | Bids | Barriers |
|---|---|---|---|---|---|
| Universitätsklinikum Heidelberg | Web-based CTMS (560504-2025) | BSI Business Systems Integration AG | €2,272,781 | 1 | ≥100 staff in development, support and administration; reference from a KKS-network member (cn 76572-2024) |
| DZNE | CTMS + eTMF (692140-2025) | BSI (Switzerland) | not stated | 4 | — |
| DIfE Potsdam | Study, participant and sample management incl. "Rekrutierung der Probanden" (98115-2026) | IQVIA | €530,858.75 | 1 | "bereits am Markt etabliertes System"; references |
| Fraunhofer | CTMS (787981-2023) | Cloud9 Software BV | not stated | 3 | — |
| Universitätsklinikum Leipzig | CTMS + eTMF (487103-2024, cn) | award not found | — | — | "Siehe Vergabeunterlagen" |

### 6. Vendors in DACH: recruitment, feasibility, site tools
Company sites are [B]; performance figures are the vendors' own claims.

| Vendor (HQ) | What | Public evidence of scale, customers or funding | Source |
|---|---|---|---|
| **Clariness** (Berlin roots; ClinLife portal; owns Viomedo; trials24.com redirects to Clariness) | Full-service patient recruitment for sponsors and CROs; feasibility; retention | Acquired Viomedo, "the largest search engine for clinical trials in Germany" (Dec 2018). Merged with SubjectWell (WindRose) in Jan 2026: ">42,000 randomizations", ">10,000 research sites", 60+ countries. ClinLife DE page: "1.342.192 Patienten haben eine passende Studie gefunden", "2.567 Studienorte online" | [healthcapital.de, 3 Dec 2018](https://www.healthcapital.de/en/news/article/clariness-today-announced-it-has-acquired-viomedo-a-leading-online-platform-for-clinical-trials-and-1); [Pulse 2.0, 28 Jan 2026](https://pulse2.com/clariness-and-subjectwell-merge-to-form-full-service-patient-recruitment-platform); [clinlife.de](https://www.viomedo.com) (redirect) |
| **Trialbee** (Sweden) | Recruitment platform "Honey", pre-screening | "6,000+ Research Sites", "50 Countries", "1.6M+ Online Pre-Screeners completed Since 2021" | [trialbee.com](https://trialbee.com/) |
| **Inato** (Paris/US) | Sponsor–site marketplace; AI pre-screening and chart review | "25+ Sponsors", "6,000+ Research sites", 50+ countries; Sanofi case material | [inato.com](https://www.inato.com/) |
| **TriNetX** (US; owns Clinerion, Basel) | EHR-network feasibility and RWD | Network of "more than 13,000 clinical sites across 20+ countries". Clinerion had "10,340 healthcare organisations and trial sites in 24 countries" (2022) and was bought by Citeline (Feb 2023). clinerion.com now redirects to trinetx.com; the TriNetX takeover (Apr 2023) is snippet-level only | [trinetx.com](https://trinetx.com/); [startupticker, 1 Feb 2023](https://startupticker.ch/en/news/world-s-leading-clinical-intelligence-company-acquires-clinerion) |
| **MPIRIQ** (Munich, founded spring 2024) | Connects to practice software; AI pre-screening ("Trial Navigator"); referral network to study centres; RWD for pharma | Prices from 1 Aug 2026: Efficiency €99/month, Care Plus €159/month, Research Premium €329/month; setup from €599; 12–24-month terms. "+1.2 M doctor visits analysed". Funding ~$3.2M seed (Jun 2024; Speedinvest/HV Capital) is snippet-only `[UNVERIFIED]` | [mpiriq.de/pricing](https://www.mpiriq.de/pricing); [/study-centers](https://www.mpiriq.de/study-centers); [Munich Startup, 20 Mar 2026](https://www.munich-startup.de/en/news/mpiriq-ai-connects-healthcare-and-research) |
| **Climedo** (Munich) | eCOA/EDC with "Autonomous Data Capture" (takes over site data entry); eConsent, self-registration | "2 Mio.+ Patient:innen"; profitable before a late-2021 round; in 2024 it said pharma investment in AI "lässt oftmals auf sich warten" | [climedo.de](https://climedo.de/); [Munich Startup, 11 Apr 2024](https://www.munich-startup.de/news/update-interview-climedo) |
| **iduneo** (Hamburg) | AI trial matching for cancer patients / pharma recruitment | Member listing only; website returned 503 | [Life Science Nord](https://www.lifesciencenord.de/en/membership/member-directory/detail/iduneo-gmbh.html) |
| **Massive Bio** (US) | Oncology trial matching, German-language patient and physician pages | Product page only | [massivebio.com/de](https://massivebio.com/de/loesungen/) |
| **Rivia** (Zurich) | Trial data platform / agentic trial operations (not recruitment) | €13M round (Mar 2026); €3M seed (Jun 2024, Speedinvest) | [The Next Web, 18 Mar 2026](https://thenextweb.com/news/rivia-13m-agentic-ai-clinical-trials) |
| **BSI, IQVIA, Cloud9** | Site CTMS | TED awards (table §5) | TED |
| Public / academic: **MII FDPG**, **NUM recruIT** | Feasibility queries across >30 university data integration centres; FHIR/OMOP-based recruitment support | FDPG open to non-MII researchers in pilot mode since May 2023; recruIT rolled out in the NUM study network (Apr 2025) | [Ärzteblatt, 18 May 2023](https://www.aerzteblatt.de/nachrichten/143260/Medizininformatikinitiative-macht-Forschungsdatenportal-frei-zugaenglich); [TU Dresden, 16 Apr 2025](https://tu-dresden.de/med/mf/imb/das-institut/news/schneller-zur-studie-recruit-die-digitale-rekrutierungsplattform-innerhalb-des-num-studiennetzwerks) |

Snippet-only, not verified: Probando (probando.de unreachable), Carelane (€800k pre-seed, htgf.de 403), Ancora.ai (403) `[UNVERIFIED]`.

### 7. Online voices [C]
- **0 relevant signals.** medi-learn Discourse search ("Studie Rekrutierung", "Prüfarzt Studien", "Study Nurse", "Studienzentrale", "Patienten für Studie"): 0 relevant threads; hits were dissertations, careers and pay.
- **Reddit:** a `site:reddit.com` r/clinicalresearch search returned no reddit.com URLs (same as A2).
- **Jobs:** the Bundesagentur job API did not return JSON, so I have no job counts.
- Existing [C] items (CRO kununu pages) are in `pain-industry.md` I1.
- *Inference:* site-staff pain is documented by surveys, not by open forums.

### 8. What this means for scoring (inference)
- **K1 (buyer with proven spend): pass.** Sponsors and CROs pay recruitment vendors (Clariness's scale) and pay sites for identification work (joint recommendations). Sites buy CTMS (TED).
- **K2 (startup-accessible first sale ≤12 months): unclear.**
  - Sponsors buy recruitment through CRO and preferred-vendor lists, which global firms dominate.
  - Site tenders demand ≥100 staff and KKS references.
  - Practices buy small SaaS directly (MPIRIQ prices show it), but MPIRIQ already holds that Munich niche.
- **Most defensible angle in the evidence:** coordinator time, and recruitment outside university hospitals (practices, regional hospitals) feeding sites. Both match the Kapazitätsinitiative funding lines and the 5 % incentive.
- **Weakest angle:** a site-internal EHR "patient finder". Sites rate identification as a minor hurdle (4–13 %), the German evaluation shows no pooled effect, and free public tools exist.

## Gaps / [UNVERIFIED]
- Euro per-patient site fees and sponsor recruitment budgets for Germany: not public. Needs Stage D interviews (site budget managers, CRO feasibility leads).
- Uptake of the MFG 5 % finding (2025–Jul 2026) and of the BfArM exemptions (from 2027): no counts found.
- DGPharMed site survey (">two thirds declined a trial for capacity reasons"): cited second-hand only.
- MPIRIQ funding and customer count, Carelane, Ancora.ai, Probando, iduneo funding: snippet-only or blocked.
- The TriNetX–Clinerion deal: the date and structure are from search snippets; the Norstella page returned 403.
- The CTIS count uses the first decision date as start and excludes trials not yet authorised. Germany's per-trial patient numbers are not public in CTIS.
- Barometer surveys are interest-group surveys; the site survey's sampling (N=169) is not described in detail.
- Blocked hosts this run: forschen-fuer-gesundheit.de (WebFetch DNS; curl 403), htgf.de (403), probando.de (no response), ancora.ai (403), norstella.com (403), iduneo.com (503); Bundesagentur jobsuche API (no JSON).

## Sources
- https://euclinicaltrials.eu/ctis-public-api/search — CTIS public search API; own count of 12,788 trials (4,653 transitioned) by country, year and sponsor type, accessed 2026-11-07
- https://clinicaltrials.gov/api/v2/studies — industry interventional counts DE/global 2024–2026, Munich and active-trial counts, accessed 2026-11-07
- https://www.vfa.de/download/studienstandort-barometer-sep-2026-praesentation.pdf — 3rd barometer: +15, ~2.9 % share, oncology/CVM site shortfalls, reasons, consequences, BStabG views, accessed 2026-11-07
- https://www.vfa.de/download/studienstandort-barometer-jan-2026-praesentation.pdf — site survey N=169: staffing, digital and patient-identification hurdles, investment plans, accessed 2026-11-07
- https://www.vfa.de/download/pg-010-2026.pdf — press release 28 Sep 2026: Kapazitätsinitiative, 5 % rule "fast das Doppelte", methodology, accessed 2026-11-07
- https://www.vfa.de/kapazitaetsinitiative-klinische-forschung.pdf — Kapazitätsinitiative paper (Sep 2026): asks, funding lines, monitor, gGmbH, Swetrial, DGPharMed citation, accessed 2026-11-07
- https://www.vfa.de/studienstandort-barometer — barometer page (dates, sample 24 + 25), accessed 2026-11-07
- https://www.vfa.de/download/pg-011-2026.pdf — Standortklausel proposal 2 % → 4 %, accessed 2026-11-07
- https://www.vfa.de/download/pg-012-2026.pdf — PROUD update: share ~3.0 %, phase I −10 %, accessed 2026-11-07
- https://www.buzer.de/130a_SGB_V.htm — § 130a Abs. 1b (8.5 %) and Abs. 1c (5 % exemption) text, accessed 2026-11-07
- https://www.buzer.de/gesetz/17632/a340690.htm — BStabG Art. 1: § 35a Abs. 3 S. 4–6 deleted; § 130a Abs. 1c inserted, accessed 2026-11-07
- https://www.buzer.de/gesetz/16657/a319278.htm — MFG Art. 6: original G-BA 5 % rule in § 35a, accessed 2026-11-07
- https://www.buzer.de/130b_SGB_V.htm — current § 130b (Abs. 1c confidential price; no 5 % rule), accessed 2026-11-07
- https://www.g-ba.de/service/fachnews/160/ — G-BA implementation of the MFG 5 % rule (dossier module 3.6), accessed 2026-11-07
- https://www.pharmazeutische-zeitung.de/hersteller-koennen-befreiung-von-zusatzabschlag-beantragen-171330/seite/2/ — BfArM portal live; extended Standortklausel has no legal basis yet (22 Oct 2026), accessed 2026-11-07
- https://www.uni-marburg.de/de/fb20/bereiche/kks/aktuellesordner/nachrichten/klinische_pruefungen_empfehlungen_zur_gesamtleistungsrechnung_2-0.pdf — joint costing recommendations (5 May 2025), accessed 2026-11-07
- https://www.vfa.de/embed/position-paper-cost-development-for-clinical-trials-in-germany — vfa 2013 position: overhead claims "up to 60%", accessed 2026-11-07
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42963362%20AND%20SRC:MED&format=json&resultType=core — MIRACUM CTRSS evaluation (npj Digit Med 2026), accessed 2026-11-07
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42607998%20AND%20SRC:MED&format=json&resultType=core — GP-practice recruitment barriers survey (Gesundheitswesen 2026), accessed 2026-11-07
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:39307405%20AND%20SRC:MED&format=json&resultType=core — investigator-sponsored RCT costs CH/DE/UK (J Clin Epidemiol 2024), accessed 2026-11-07
- https://www.aerzteblatt.de/news/paul-ehrlich-institut-leichter-zuwachs-bei-antragen-auf-klinische-prufungen-3db64753-f916-4a99-ac0c-c419bae388b0 — PEI: 809 applications 2024, 805 in 2023, accessed 2026-11-07
- https://www.aerzteblatt.de/nachrichten/143260/Medizininformatikinitiative-macht-Forschungsdatenportal-frei-zugaenglich — FDPG open to non-MII researchers (pilot), >30 data integration centres, accessed 2026-11-07
- https://tu-dresden.de/med/mf/imb/das-institut/news/schneller-zur-studie-recruit-die-digitale-rekrutierungsplattform-innerhalb-des-num-studiennetzwerks — recruIT in the NUM study network, accessed 2026-11-07
- https://api.ted.europa.eu/v3/notices/search — TED awards: UK Heidelberg CTMS (560504-2025), DZNE (692140-2025), DIfE (98115-2026), Fraunhofer (787981-2023), UK Leipzig cn (487103-2024), Heidelberg cn criteria (76572-2024), accessed 2026-11-07
- https://pulse2.com/clariness-and-subjectwell-merge-to-form-full-service-patient-recruitment-platform — Clariness–SubjectWell merger (Jan 2026), scale figures, accessed 2026-11-07
- https://www.healthcapital.de/en/news/article/clariness-today-announced-it-has-acquired-viomedo-a-leading-online-platform-for-clinical-trials-and-1 — Clariness acquires Viomedo (Dec 2018), accessed 2026-11-07
- https://www.viomedo.com — redirects to clinlife.de; ClinLife patient and site counts, accessed 2026-11-07
- https://clariness.com/ — Clariness services and scale claims, accessed 2026-11-07
- https://trialbee.com/ — Trialbee scale claims, accessed 2026-11-07
- https://www.inato.com/ — Inato scale claims, accessed 2026-11-07
- https://trinetx.com/ — TriNetX network size; clinerion.com redirect target, accessed 2026-11-07
- https://startupticker.ch/en/news/world-s-leading-clinical-intelligence-company-acquires-clinerion — Citeline acquires Clinerion (Feb 2023), network size 2022, accessed 2026-11-07
- https://www.mpiriq.de/pricing — MPIRIQ prices (from 1 Aug 2026), accessed 2026-11-07
- https://www.mpiriq.de/study-centers — MPIRIQ referral network for study centres, accessed 2026-11-07
- https://www.mpiriq.de/pharma — MPIRIQ pharma/RWD offer, accessed 2026-11-07
- https://www.mpiriq.de/partners — "+1.2 M doctor visits analysed", accessed 2026-11-07
- https://www.munich-startup.de/en/news/mpiriq-ai-connects-healthcare-and-research — MPIRIQ founding 2024, model, goals, accessed 2026-11-07
- https://climedo.de/ — Climedo ADC/eCOA/EDC, accessed 2026-11-07
- https://www.munich-startup.de/news/update-interview-climedo — Climedo funding history, pharma AI investment hesitancy (Apr 2024), accessed 2026-11-07
- https://www.lifesciencenord.de/en/membership/member-directory/detail/iduneo-gmbh.html — iduneo profile, accessed 2026-11-07
- https://massivebio.com/de/loesungen/ — Massive Bio German product page, accessed 2026-11-07
- https://thenextweb.com/news/rivia-13m-agentic-ai-clinical-trials — Rivia €13M (Mar 2026), accessed 2026-11-07
