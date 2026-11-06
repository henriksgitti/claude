# Pain mining: pharma, clinical research, payers, medtech, public health (DE/EU)
Task: A5 | Date: 2026-11-06 | Status: draft

Method: recipes from `research/sources-map.md`. Pages fetched with curl and converted to text locally. Also used:
- TED API v3: contract notices only (`notice-type=cn-standard`), de-duplicated by buyer, descriptions read via the `description-lot` field.
- ClinicalTrials.gov v2 API (own counts), Europe PMC REST, kununu employer pages, Capterra DE.

Grades follow `CLAUDE.md` rule 2. Online voices are quoted without usernames.

**Limits:**
- Reddit was not used (blocked, see A2).
- Industry pain barely shows up in open forums. Elsmar Cove, the main medical-device QA forum, returned 403. medi-learn has only old career threads on pharma, the MD (Medizinischer Dienst, the insurers' medical review service) and public-health work. The krankenschwester.de search needs a session token. The [C] base for this file is therefore thin, and most problems rest on [A]/[B] only.
- Job-ad counts were not used (unreliable, see lessons).

## Findings
- **German clinical-trial sites miss recruitment targets, and Germany is losing trial share.**
  - Pharma/CRO barometer (Aug 2026, 24 pharma companies + 25 CROs): "72 Prozent der Unikliniken unterschreiten ihre geplante Rekrutierung um mindestens 25 Prozent"; at maximum-care and teaching hospitals the share is 68 %. The barometer's outlook fell from +34 to +7 [B] ([Ärzteblatt, 28 Sep 2026](https://www.aerzteblatt.de/news/studienstandort-barometer-unternehmen-erwarten-deutlich-weniger-dynamik-fe211b4a-8308-442b-b27a-e09eaec85e05)).
  - Germany's share of trial participants worldwide fell from about 4.5 % (2014) to 3.0 % (2024). Participants recruited in Germany fell from about 33,000 to about 24,000 [B] ([vfa/Vintura barometer, Oct 2025](https://www.vfa.de/download/studienstandort-barometer-okt-2025-praesentation.pdf)).
  - Own ClinicalTrials.gov count (registry data [A], my math): industry interventional trials with a German site fell from 715 (2015, 15.4 % of 4,636) to 622 (2025, 10.5 % of 5,912). Spain overtook Germany in 2021.
  - EU-wide: trial authorisations fell 13.5 %, from an average of 1,989/yr (2013–19) to 1,721/yr (2022–25) [A] ([Lancet Reg Health Eur 2026](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42861283%20AND%20SRC:MED&format=json&resultType=core)).
  - Of 347 trials approved in 2016 (UK, CH, DE, CA), 31.1 % were discontinued, most often for poor recruitment (45.4 % of those) [A] ([JAMA Netw Open 2025](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:40899933%20AND%20SRC:MED&format=json&resultType=core)).
  - The industry associations now call for a "Kapazitätsinitiative Klinische Forschung 2030": study staff, permanent site structures, and "digitale Möglichkeiten zur Identifikation geeigneter Studienteilnehmender" [B] (Ärzteblatt, above).
- **Policy is fixing approval speed, but not site capacity.**
  - Since 2024 the Medical Research Act (MFG) allows 26-day approval for single-country trials, and standard contract clauses (StandVKlV) apply from 18 Dec 2025 [B] (vfa barometer 2025).
  - The EU Biotech Act proposal (16 Dec 2025) would cut multinational trial approval from 106 to 76 days [B] ([Jones Day, May 2026](https://www.jonesday.com/en/insights/2026/05/the-proposed-european-biotech-act-100-days-on)).
  - Companies rank "Personalausstattung in Studienzentren" and "Juristische Vertragsverhandlungen" as the top hurdles. They rate digitalisation and data access as minor ("geringes Hemmnis") [B] (vfa barometer 2025).
  - *Inference:* the remaining gap is site staff time and patient finding. Regulatory approval is no longer the main bottleneck.
- **Statutory insurers outsource high-volume paper invoice processing, and from 2027 their admin budgets are capped.**
  - AOK Hessen tendered intake and checking of invoices from "sonstige Leistungserbringer" (other providers: aids, home nursing, therapy, transport). Volume: 19,257,000 invoices and 50,802,000 scanned sheets over 4 years [A] ([TED 761998-2025](https://api.ted.europa.eu/v3/notices/search)).
  - DAK outsourced billing checks for home nursing: "ca. 890 Mio. Euro pro Abrechnungsjahr und ca. 2,0 Mio. Belege" [A] (TED 396194-2026).
  - In total, 9 payer buyers tendered invoice/receipt processing since 2025 [A] (TED).
  - From 2027, each insurer's admin spending may only grow with the per-insured income rate [A] ([§ 4 Abs. 5 SGB V](https://www.buzer.de/4_SGB_V.htm)).
  - In a survey of 32 insurers covering ~60 % of the insured, 97 % call AI indispensable because of the retirement wave, but expect few short-term savings [B] ([Lünendonk, Aug 2026](https://luenendonk.de/wp-content/uploads/2026/08/LUE_Digitale_Transformation_in_der_GKV_PI_f.pdf)).
- **The MD buys AI for its assessments.**
  - Long-term-care assessments: more than 3 million in 2025 [B] ([MD Bund, Jul 2026](https://md-bund.de/fileadmin/dokumente/Pressemitteilungen/2026/2026_07_15/_26-07-15_FIN_PM_Report_Pflegebeduerftigkeit.pdf)), up from 1.52m in 2014 ([vdek](https://www.vdek.com/magazin/ausgaben/2025-04/modernisierung-pflegebegutachtung.html)).
  - MD Rheinland-Pfalz tendered a "KI-unterstützten Gutachtens in der Einzelfallbegutachtung Pflege" (proof of concept, then roll-out). MD Nordrhein tendered AI support for malpractice reviews ("Begutachtung vermuteter Behandlungsfehler") [A] (TED 343840-2025, 762721-2026).
- **Medtech: certification under the EU device regulations (MDR/IVDR) is slow and costly. EU fixes are underway.**
  - Average MDR certification takes 19.5 months for the quality-management system (QMS) and 21.8 months for the technical documentation. 90 % of first-year certification cost is the manufacturer's own staff [B] ([MedTech Europe, Jan 2025](https://medtecheurope.org/wp-content/uploads/2025/01/mte-ivdr-mdr-survey-report-highlights-final.pdf)).
  - DACH survey (245 manufacturers): 53 % cut R&D projects because of MDR/IVDR, and more than 40 % no longer launch innovations in the EU [B] ([BVMed/MedicalMountains/SPECTARIS/VDGH, Oct 2025](https://www.bvmed.de/download/mdr-ivdr-umfrage-auswertung-2025.pdf)).
  - The Commission proposed a targeted MDR/IVDR revision on 16 Dec 2025 [B] ([Mason Hayes & Curran](https://www.mhc.ie/latest/insights/eu-commission-proposes-reform-of-the-medical-devices-regulation)).
- **Weak buyers (counter-evidence):**
  - Public health: the federal "Pakt für den ÖGD" (€4bn, 2021–26) is to end in 2026 without follow-up funding [B] ([Ärzteblatt, Feb 2026](https://www.aerzteblatt.de/news/pakt-fur-offentlichen-gesundheitsdienst-soll-ende-des-jahres-auslaufen-56bc8c97-3fb3-46ea-9ef9-1de7cbb06d5e)).
  - Pharmacovigilance: case volume is flat (+0.5 % in 2025) [A] ([EMA](https://www.ema.europa.eu/en/documents/report/2025-annual-report-eudravigilance-european-parliament-council-commission_en.pdf)).
  - Insurer staff rate their employers positively on kununu, so this is a process-cost problem rather than a staff-pain problem [C].

## Summary table
Signals = independent items I opened. WTP = willingness to pay. "Buyers" = distinct TED contract-notice buyers since 1 Jan 2025.

| # | Problem | Who has it | Who pays / could pay | [A]/[B] items | [C] signals | WTP evidence | Strength (inference) |
|---|---|---|---|---|---|---|---|
| I1 | Trial sites under-recruit; DE losing trial share | Sponsors (pharma, biotech), CROs, site staff; patients without trial access | Sponsors and CROs (per-patient and recruitment budgets); MFG 5 % incentive | 8 (barometer 2025 + 2026, CT.gov count, Lancet RH Eur 2026, JAMA Netw Open 2025, Trials 2021, EFPIA/IQVIA 2024, TIRS 2026) | Weak: 3 CRO kununu pages (pressure, overtime, travel); 4 of 457 krebs-kompass titles mention a trial, all from 2011–17 | Industry asks for digital patient identification; DKFZ CRO framework tender; 65 CTMS products on Capterra DE | **High** pain and founder fit; buyer = sponsors; competition crowded (global vendors) |
| I2 | Site start-up load: staff shortage, contracts, budgets, system training | Site staff (study nurses, investigators), CRO start-up teams | Sponsors/CROs; sites (overhead) | 4 (barometer 2025, StandVKlV, Trials 2024, ACT/SCRS 2023) | 1 kununu page (ICON: "unzählige unbezahlte Überstunden") | Contracts and approvals partly fixed by law (StandVKlV, MFG, Biotech Act) | Medium; part is being solved by policy |
| I3 | EU HTA joint clinical assessment (JCA) + AMNOG dossiers: many PICOs (population/intervention/comparator/outcome questions), tight timelines | Pharma market-access teams, especially small and mid-sized biotechs | Pharma (outsourced to consultancies and CROs) | 4 (pharmaphorum 2026, EFPIA 2025, GKV-SV AMNOG, Reg. 2021/2282 scope via sources) | 0 | Consultancies sell JCA services (EVERSANA, Parexel, IQVIA) | Medium; ~58 JCAs max in 2026 → niche, high value per dossier; crowded with incumbents |
| I4 | MDR/IVDR certification time and cost for medtech SMEs | Device and IVD makers (93 % of BVMed's sector are SMEs) | Manufacturers | 4 (MedTech Europe 2025, BVMed et al. 2025, BVMed Herbstumfrage 2025, MDR revision proposal) | 0 (Elsmar blocked) | 90 % of cost is internal staff → tools and consultants | Medium–high pain, **policy risk**: the revision may shrink the pain |
| I5 | Insurer invoice/receipt processing for other providers (§ 302 SGB V) still paper-heavy and outsourced | Insurer claims departments (93 statutory insurers) | Insurers (admin budget, capped from 2027) | 6 (TED x9 buyers, BMG finances 2025, § 4(5) SGB V, Lünendonk 2026, GKV-SV admin costs, Telekom/caery) | 3 kununu pages (BARMER, DAK, AOK PLUS: mostly positive; workload in places) | **9 buyers**; AOK Hessen 19.3m invoices/4 yrs; DAK €890m/yr through an outsourcer | **High WTP**, clear buyer; incumbent BPO vendors unknown (gap) |
| I6 | MD assessment workload (care-level and malpractice reviews) | 15 regional MDs; applicants waiting | MDs (financed by insurers) | 3 (MD Bund 2026, vdek 2025, TED x3 buyers) | 1 kununu page (MD Bayern: "Arbeitsverdichtung", "fehlende Nachbesetzungen") | MD RLP PoC→roll-out; MD Nordrhein AI malpractice review; MD Bayern chatbot | Medium–high; few buyers (15); format may change with the care reform (PNOG) |
| I7 | PKV claims checking (>70m invoices/yr) and a new physician fee schedule (GOÄ) from 2028 at the earliest | Private insurers' claims teams | Private insurers | 2 (PKV statement 2025, PKV/BÄK GOÄ PR 2026) | 0 | — (private buyers, no tenders) | Low–medium evidence; rule change in 2028 could force system updates (inference) |
| I8 | Research access to German claims/EHR data (FDZ Gesundheit) | Pharma real-world-evidence teams, researchers | Pharma, academia | 2 (§ 303e SGB V, PZ 2026) | 0 | 53 applications by Feb 2026 | Opportunity rather than pain; electronic patient record (ePA) data only from 2026/27 |
| I9 | Public-health office (ÖGD) digitalisation after the pact ends | Local health offices (Gesundheitsämter) | Länder/municipalities | 2 (Ärzteblatt 2026, Ärzteblatt ÖGD congress) | 0 | Funding cliff end of 2026 | **Weak buyer** |
| I10 | Pharmacovigilance case processing | Pharma safety teams | Pharma | 1 (EMA EudraVigilance 2025) | 0 | — | Low: flat volume, mature vendors |

## Details

### I1 Trial recruitment shortfall and declining German trial share
- **[B] Studienstandort-Barometer, 3rd wave (BPI, BVMA, vfa; Aug 2026; 24 pharma companies + 25 CROs, weighted by trial activity):**
  - Overall index fell "von +31 im Januar auf +15 im August 2026"; the 12-month outlook fell "von +34 auf +7".
  - Germany's share of participants recruited worldwide: "Für 2024 wird der Anteil auf etwa 2,9 Prozent geschätzt."
  - Bottleneck: site recruitment, especially in oncology. 83 % of university sites contribute a high share of recruitment, but 72 % of them miss their plan by ≥25 %.
  - Quote on the 2024 Medical Research Act (MFG): "Von der positiven Wirkung des Medizinforschungsgesetzes … ist nur noch wenig zu merken" ([Ärzteblatt](https://www.aerzteblatt.de/news/studienstandort-barometer-unternehmen-erwarten-deutlich-weniger-dynamik-fe211b4a-8308-442b-b27a-e09eaec85e05)).
  - Caveat: an industry survey run by interest groups.
- **[B] Barometer, 1st wave (Vintura for vfa/BVMA, survey Jul 2025, 38 companies):**
  - Participants recruited in Germany: "ca. 24 Tsd. (2024), gesunken von ca. 33 Tsd. (2014); -4,2 % p.a.". Abroad: "ca. 1 Mil. (2024) gestiegen von ca. 750 Tsd. (2014)".
  - Hurdles ranked: Personalausstattung in Studienzentren, juristische Vertragsverhandlungen, regulatorische Hürden, Personalausstattung bei Pharmafirmen und CROs.
  - "Digitalisierungsdefizite und mangelnde Datenvernetzung gelten laut Befragung als geringes Hemmnis" ([PDF](https://www.vfa.de/download/studienstandort-barometer-okt-2025-praesentation.pdf)).
  - Counter-signal for a pure software play (inference): sponsors do not see digital tools as their main gap. By Sep 2026, however, digital patient identification is part of the associations' demand list.
- **[A, own count] ClinicalTrials.gov v2 API, queried 2026-11-06.** Filter: industry lead sponsor, interventional, start date within the year; "DE" = at least one German site.

  | Start year | DE | Spain | All | DE share |
  |---|---|---|---|---|
  | 2015 | 715 | 527 | 4,636 | 15.4 % |
  | 2019 | 692 | 686 | 4,981 | 13.9 % |
  | 2021 | 721 | 829 | 6,400 | 11.3 % |
  | 2023 | 636 | 698 | 5,730 | 11.1 % |
  | 2025 | 622 | 699 | 5,912 | 10.5 % |

  - Math: 715 → 622 is −13.0 % (93/715).
  - Caveats: CT.gov only (EU-only trials may be missing); late registrations can raise the recent years.
- **[A] EU level:**
  - Lancet Reg Health Eur 2026 (25,320 trials in CTIS/EudraCT): −13.5 %, "predominantly observed in non-commercial and phase IV trials".
  - IQVIA for EFPIA (Aug 2024): the EEA share of commercial trials fell from 22 % (2013) to 12 % (2023), and "patient recruitment times in Europe may be impacting the attractiveness of Europe as a trial location" [B] ([PDF](https://www.efpia.eu/media/3edpooqp/assessing-the-clinical-trial-ecosystem-in-europe.pdf)).
- **[A] Recruitment failure:**
  - JAMA Netw Open 2025: 108 of 347 RCTs discontinued (31.1 %), 49 of them (45.4 %) for poor recruitment. Industry trials were less often discontinued for poor recruitment (aOR 0.32).
  - Qualitative study in DE/CH/CA (Trials 2021, PMID 34823582): the most frequent reasons were "overoptimistic recruitment estimates, too narrow eligibility criteria, lack of engagement of recruiters". Interviews date from 2015–16, so the data are >3 years old.
  - German Parkinson workshop (J Neural Transm 2026, PMID 42925427) names "suboptimal patient recruitment pathways" and "slow and bureaucratic regulatory procedures".
- **[C] Voices:**
  - CRO employees on kununu, rated well below average: ICON "2,8 von 5" (58 reviews), Parexel "3,2" (127). IQVIA's AI summary: "Karrieremöglichkeiten und Gehalt zählen zu den schwächsten Punkten" ([kununu IQVIA](https://www.kununu.com/de/iqvia/kommentare); [ICON](https://www.kununu.com/de/icon-clinical-research/kommentare)).
  - ICON reviews on page 1: "Hohe Reisetätigkeit … extremer Druck und unzählige unbezahlte Überstunden"; "Das Team war unter starkem Druck".
  - These complaints are about work pressure. Recruitment tools are not mentioned.
  - Patient side: only 4 of 457 thread titles on krebs-kompass (8 subforums, pages 1–3) mention a study, all 2011–2017. Excerpt: "kenne mich mit Studien bisher überhaupt nicht aus" ([thread](https://www.krebs-kompass.de/showthread.php?t=60921)). *Inference:* patients rarely search for trials in forums. Trial access runs through physicians.
- **Competition (B/C):**
  - Capterra DE lists "65 Ergebnisse" in clinical-trial-management software, with Castor EDC among the top-rated ([Capterra](https://www.capterra.com.de/directory/30458/clinical-trial-management/software)).
  - Recruitment vendors in DACH (Trialbee, Viomedo, Trials24, Probando) appeared only in search snippets `[UNVERIFIED]`.

### I2 Site start-up and site workload
- **[B] Contracts:** StandVKlV (binding standard contract clauses for commercial drug trials) applies from 18 Dec 2025. The 2025 barometer reports they "entfalten derzeit noch nicht ihr volles" effect, and big CROs rate contract and budget negotiations as "besonders große Hürde" ([vfa](https://www.vfa.de/download/studienstandort-barometer-okt-2025-praesentation.pdf)).
- **[B] Approvals:**
  - The MFG allows approval of single-country trials "innerhalb von 26 Tagen".
  - EU Biotech Act proposal: multinational 106 → 76 days; substantial modifications 96 → 47 days. The FAST-EU pilot (23 Member States) runs since Jan 2026. The Commission cites "113 days on average for multinational clinical trials, compared with 60 days in other regions" ([Jones Day](https://www.jonesday.com/en/insights/2026/05/the-proposed-european-biotech-act-100-days-on)). Primary text COM(2025)1022 not opened `[UNVERIFIED]` beyond this summary.
- **[A] CTR/CTIS burden:**
  - Three EU trials reported "increased document burden, barriers to submitting important modifications, and debilitating technical hurdles" ([Trials 2024, PMID 38167484](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38167484%20AND%20SRC:MED&format=json&resultType=core)).
  - TIRS 2026 finds "substantial administrative workload and persistent operational heterogeneity" ([PMID 42837073](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42837073%20AND%20SRC:MED&format=json&resultType=core)).
- **[B] Site technology training (US-led survey, 2023, >3 years old by survey date):** "40% of sites are spending an average of 5-15 hours per month per trial on technology training" ([Applied Clinical Trials](https://www.appliedclinicaltrialsonline.com/view/addressing-current-challenges-in-the-site-landscape)).

### I3 EU HTA (JCA) and AMNOG dossiers
- **[B] JCA one year on (pharmaphorum, 2026):**
  - The JCA started 12 Jan 2025 for oncology drugs and ATMPs (advanced therapy medicinal products), extends to orphan drugs in 2028 and to all new drugs by 2030.
  - A consultant quote: "JCA has been a very resource-intensive process". "The 100-day timeline to respond … in the real world, it is less than that".
  - "57% of 2025 LOIs were submitted late" (LOI = letter of intent to the HTA secretariat).
  - 2026 plan: "~ 58 JCAs", including ~35 oncology and ~15 ATMP.
  - Added complexity: "subgroup analyses that may previously have been requested only by Germany may now need to be submitted for multiple countries" ([pharmaphorum](https://pharmaphorum.com/market-access/europes-new-hta-reality-jca-one-year)).
- **[B] EFPIA (2025):** "the interplay between population and comparator … are the key drivers of the number of PICOs"; PICO scoping "lacks clarity and transparency" ([EFPIA](https://www.efpia.eu/news-events/the-efpia-view/blog-articles/from-guidance-to-implementation-efpia-s-reflections-on-eu-hta-scoping-pico-exercises/)).
- **[A/B] AMNOG (GKV-SV):** "Von 2011 bis zum 31.12.2024 wurden 507 neue Wirkstoffe einer frühen Nutzenbewertung … unterzogen", 922 negotiations, 23 opt-outs, and 74 drugs left the market ([GKV-SV](https://www.gkv-spitzenverband.de/gkv_spitzenverband/presse/fokus/amnog_verhandlungen/s_thema_amnog_verhandlungen.jsp)).
- *Inference:* the market is small in count (dozens of JCAs a year EU-wide) but high value per dossier. Incumbents (global CROs and market-access consultancies) already sell JCA services. A startup would need deep HTA expertise, which the founder profile lacks.

### I4 MDR/IVDR certification burden
- **[B] MedTech Europe survey (Apr–May 2024, 211 manufacturers; published Jan 2025):**
  - MD QMS certification takes 19.5 months on average, technical documentation 21.8 months. More than 50 % of that time sits in "pre-review" and "certificate issuance".
  - For 50 % of MD respondents, at least one certificate was "significantly delayed or closed negatively" because the clinical evaluation was challenged.
  - First-year cost split: 90 % personnel, 7 % notified-body fees.
  - The EU as first launch market fell by 33 % (large firms) and 19 % (SMEs) ([PDF](https://medtecheurope.org/wp-content/uploads/2025/01/mte-ivdr-mdr-survey-report-highlights-final.pdf)).
- **[B] DACH survey (Oct 2025; 245 manufacturers, 209 headquartered in DE):**
  - 53 % reduced R&D projects because of MDR/IVDR.
  - More than 40 % no longer launch innovative products in the EU.
  - 64 % of orphan-device makers have discontinued products ([PDF](https://www.bvmed.de/download/mdr-ivdr-umfrage-auswertung-2025.pdf)).
- **[B] Sector structure:** "93 Prozent der MedTech-Unternehmen sind KMU" ([BVMed Herbstumfrage 2025](https://www.bvmed.de/download/zusammenfassung-der-ergebnisse-der-bvmed-herbstumfrage-2025.pdf)).
- **[B] Policy:** the Commission's targeted revision (16 Dec 2025) would remove the 5-year certificate validity limit, allow lower classifications, and streamline change notifications ([MHC](https://www.mhc.ie/latest/insights/eu-commission-proposes-reform-of-the-medical-devices-regulation)). The primary text was not opened (eur-lex is bot-checked) `[UNVERIFIED]` beyond this summary.
- *Inference:* the pain is real and documented, but the revision may remove part of it within 2–3 years, and the work is regulatory expertise rather than workflow. Kill risk for a startup that only sells "MDR compliance".

### I5 Insurer invoice processing (§ 302 SGB V) and the admin cap
- **[A] TED, contract notices since 1 Jan 2025, payer buyers, titles on invoice/receipt processing (9 buyers):**
  - BIG direkt gesund: "Annahme, Aufbereitung, Prüfung und Zahlungsvorbereitung aller Rechnungen … der Sonstigen Leistungserbringer nach § 301 und § 302 SGB V" (189396-2025).
  - BAHN-BKK: support for billing processing (269243-2025).
  - AOK Baden-Württemberg: scan service (673984-2025).
  - AOK Hessen: external receipt management for invoice checking (761998-2025). Volumes for 2026–30: "19.257.000 Summe Einzelrechnungen", "50.802.000 Summe Blätter" (≈4.8m invoices and ≈12.7m sheets a year; my division by 4). Areas: Hilfsmittel, häusliche Krankenpflege, Pflegeversicherung, Heilmittel, Fahrkosten, Reha-Sport, Hebammenhilfe.
  - hkk: pharmacy billing under § 300 (379963-2026).
  - DAK-Gesundheit: "Abrechnungsprüfung HKPF, AKI und HHhi", outsourced "an einen Dienstleister … ca. 890 Mio. Euro pro Abrechnungsjahr und ca. 2,0 Mio. Belege, DTA-Quote 97,5 %" (396194-2026). DTA = electronic data transfer. *Inference:* even at 97.5 % electronic data, checking is still outsourced.
  - AOK NordWest via gkv informatik: "Externe Belegannahme und -verarbeitung für die Rechnungsprüfung" (481787-2026).
  - AOK Rheinland/Hamburg: external scan services (518174-2026).
  - Pronova BKK: scan client software (177834-2026).
  - Related automation buys: UiPath licences (BKK mkk, 483613-2025), Automic automation (KKH, 688078-2026), "KI-unterstützte Enterprise Search Engine" (TK, 252303-2025), AI infrastructure (gkv informatik, 76741-2025), dental case-management software (mhplus BKK, Salus BKK).
- **[A] Spending growth in exactly these areas (BMG, 2025 results):**
  - Heilmittel (therapy) +10.4 % (+€1.4bn), "das dritte Jahr in Folge oberhalb von 10 Prozent".
  - Medizinische Behandlungspflege (home nursing care) +12.6 % (+€1.3bn).
  - Fahrkosten (patient transport) +8.9 % (+€852m).
  - Admin costs +4.7 % to ~€13.3bn. Insurers' reserves were 0.18 monthly expenditures, below the 0.2 legal minimum ([BMG](https://www.bundesgesundheitsministerium.de/presse/pressemitteilungen/finanzentwicklung-gkv-2025)).
  - 2024 net admin costs: €12.63bn, €169.54 per insured, 3.86 % of spending ([GKV-SV](https://www.gkv-spitzenverband.de/gkv_spitzenverband/presse/fokus/verwaltungskosten_kk.jsp)).
- **[A] Admin cap from 2027:** "Ab dem Haushaltsjahr 2027 dürfen sich die Verwaltungsausgaben einer Krankenkasse … nur nach Maßgabe der … durchschnittlichen Veränderungsrate je Versicherten erhöhen". IT-security spending is exempt ([§ 4 Abs. 5 SGB V](https://www.buzer.de/4_SGB_V.htm)). The government expects ~€100m savings in 2027 [B] ([krankenkasseninfo](https://www.krankenkasseninfo.de/ratgeber/nachrichten/krankenkassen-muessen-bei-verwaltung-und-werbung-sparen-62674.html)).
- **[B] Insurer survey (Lünendonk, spring 2026, 32 insurers):**
  - "Nahezu alle befragten Kassen (97 %) sehen Künstliche Intelligenz als unverzichtbar an … Angesichts der bevorstehenden Ruhestandswelle".
  - "Mit kurzfristigen Kostensenkungen rechnen die Kassen dagegen kaum".
  - 78 % see politics as a brake on digitalisation ([PDF](https://luenendonk.de/wp-content/uploads/2026/08/LUE_Digitale_Transformation_in_der_GKV_PI_f.pdf)).
- **[B] Competitor entering:** Telekom + caery automate "Leistungsprüfung, Abrechnung und Auszahlung" for insurers. caery claims up to €10bn/yr potential (vendor claim, not evidence) ([Telekom, Sep 2026](https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken)).
- **[C] Insurer staff (kununu AI summaries):**
  - BARMER (1,127 reviews), DAK (778) and AOK PLUS (425) all have "positives Gesamtbild".
  - Pain mentions are local: "Personalmangel, verstärkte Kontrolle sowie Benchmarking-Druck" (BARMER); "Konkurrenzdenken durch hohe Arbeitsbelastung" (AOK PLUS) ([BARMER](https://www.kununu.com/de/barmer/kommentare); [DAK](https://www.kununu.com/de/dak-gesundheit/kommentare); [AOK PLUS](https://www.kununu.com/de/aok-plus/kommentare)).
- *Inference:* clear, recurring, public budget (4-year contracts, millions of documents), and an admin cap that pushes insurers from people to automation. Open questions: who the current outsourcers are (award notices not yet read) and whether insurers buy from startups or only through gkv informatik / BITMARCK / AOK Systems.

### I6 MD assessment workload
- **[B]** "über 3 Millionen Pflegebegutachtungen … im Jahr 2025" ([MD Bund](https://md-bund.de/fileadmin/dokumente/Pressemitteilungen/2026/2026_07_15/_26-07-15_FIN_PM_Report_Pflegebeduerftigkeit.pdf)). The number of people needing care doubled since 2014 to >5.6m. The MD wants flexible formats ("ob ein Interview per Telefon oder Video sinnvoll ist"), which "bedarf … der Anpassung gesetzlicher Regelungen" ([vdek](https://www.vdek.com/magazin/ausgaben/2025-04/modernisierung-pflegebegutachtung.html)).
- **[A] TED:**
  - MD Rheinland-Pfalz: "Proof of Concept (PoC) eines KI-unterstützten Gutachtens in der Einzelfallbegutachtung Pflege … zunächst in Bezug auf die Mobilitätsbewertung", with options for all modules and a roll-out (343840-2025).
  - MD Nordrhein: AI to "umfangreiche medizinische Unterlagen automatisiert analysieren … Gutachtenentwürfen unterstützen" for malpractice reviews (762721-2026).
  - MD Bayern: chatbot and AI search (63363-2025).
- **[C]** MD Bayern on kununu (204 reviews): "Zeitdruck und wachsende Arbeitsverdichtung"; "steigende Arbeitsbelastung durch fehlende Nachbesetzungen" ([kununu](https://www.kununu.com/de/mdk-medizinischer-dienst-der-krankenversicherung-in-bayern/kommentare)).
- *Inference:* a real buyer exists, but there are only 15 MDs plus MD Bund, and public procurement is slow. The overlap with A3 P1 (care-benefit navigation) is worth noting: the MD's own data say 59.6 % of applicants choose Pflegegeld and organise care themselves.

### I7 PKV claims and the new fee schedule
- **[B]** "Jedes Jahr werden mehr als 70 Millionen Rechnungen zur Erstattung eingereicht"; 6,891 ombudsman complaints in 2024 ([PKV](https://www.pkv.de/verband/presse/meldungen/pkv-stellungnahme-zu-finanztip-umfrage-ueber-kostenerstattung/)).
- **[B]** The physician fee-schedule reform (new GOÄ): the BÄK/PKV draft was updated on 31 Jul 2026, and "ein Inkrafttreten der neuen GOÄ zum 1. Januar 2028 erreichbar" ([PKV](https://www.pkv.de/verband/presse/pressemitteilungen/goae-entwurf-erfolgreiche-aktualisierung-als-basis-fuer-ein-zuegiges-verordnungsverfahren/)).
- Gap: no automation rates or vendor data found. Customer-side pain (slow reimbursement) is only a Finanztip survey that PKV disputes as non-representative. `[UNVERIFIED]`

### I8 Research data access (FDZ Gesundheit)
- **[A]** Access is purpose-based: "Nutzungsberechtigt sind natürliche und juristische Personen im Anwendungsbereich der Verordnung (EU) 2016/679", so companies can apply ([§ 303e SGB V](https://www.buzer.de/303e_SGB_V.htm)).
- **[B]** The portal opened in Oct 2025. By Feb 2026: 82 institutions registered, 53 applications. "Bisher sind allerdings nur pseudonymisierte Abrechnungsdaten … verfügbar" ([PZ](https://www.pharmazeutische-zeitung.de/53-antraege-auf-datennutzung-fuer-forschung-163005/)).
- *Inference:* an enabler for I1 (feasibility, patient finding), not a pain in itself.

### I9 Public health (ÖGD)
- **[B]** Federal statement on the pact: "angesichts der angespannten Haushaltslage des Bundes ist eine Fortsetzung des Paktes für den ÖGD nicht zu begründen". BVÖGD warns of "das Aus für laufende und geplante Digitalisierungsprojekte" ([Ärzteblatt, Feb 2026](https://www.aerzteblatt.de/news/pakt-fur-offentlichen-gesundheitsdienst-soll-ende-des-jahres-auslaufen-56bc8c97-3fb3-46ea-9ef9-1de7cbb06d5e)).
- **[B]** The pact funded €4bn for 2021–26 and created "Mehr als 5.000 Stellen" ([Ärzteblatt](https://www.aerzteblatt.de/news/appell-von-amtsaerzten-pakt-fuer-den-oegd-ueber-2026-hinaus-verstetigen-9f2e7090-b4f9-440f-ad7e-56b5932a608b)).
- *Inference:* the pain rises but the budget falls. Not a good first market.

### I10 Pharmacovigilance
- **[A]** "In 2025, nearly 1.8 million ICSRs" (individual case safety reports) after authorisation were collected, "a 0.5% increase compared to 2024" ([EMA](https://www.ema.europa.eu/en/documents/report/2025-annual-report-eudravigilance-european-parliament-council-commission_en.pdf)).
- *Inference:* a mature, vendor-served process with flat volume. Low priority.

### Founder fit (inference, for A7/B1)
- I1/I2 match the stated interest (drug development, clinical research) and the "AI for workflow" sweet spot. The buyer (sponsors/CROs) has budget, but the industry itself does not rank digital tools as the main gap, and global vendors are many.
- I5/I6 have the clearest public willingness to pay found in Stage A so far (multi-year tenders with volumes). The buyer is the statutory health system, which matches the "payers" interest. Procurement and IT-integration barriers are high.

## Gaps / [UNVERIFIED]
- **[C] base:**
  - Reddit, LinkedIn and Elsmar Cove are inaccessible, and German forums have almost no industry talk.
  - I3, I4, I7–I10 have zero [C] signals.
  - *Inference:* B2B pain lives in closed channels (LinkedIn, conferences, associations). This needs interviews in Stage D.
- **Incumbents:**
  - Who won the § 302 processing tenders (award notices not read).
  - DACH trial-recruitment vendors (snippet only `[UNVERIFIED]`).
  - Sponsor per-patient recruitment prices in DE (not found).
- **Primary EU texts not opened (eur-lex bot check):** HTA Regulation 2021/2282 (scope dates taken from pharmaphorum and EFPIA), the MDR revision proposal and the Biotech Act proposal (law-firm summaries only).
- **Data limits:**
  - The ClinicalTrials.gov count is CT.gov only. CTIS-based German counts were not pulled.
  - Two key sources are interest-group surveys (barometer, BVMed) and should be paired with registry data where possible (done for I1 only).
  - Older data (>3 years): the Trials 2021 interview data (2015–16) and the SCRS 2023 training figure.
- **Not found:** GKV staff age structure and retirement numbers (Lünendonk mentions a "Ruhestandswelle" without numbers) `[UNVERIFIED]`; MD staffing numbers; PKV automation rates.

## Sources
- https://www.aerzteblatt.de/news/studienstandort-barometer-unternehmen-erwarten-deutlich-weniger-dynamik-fe211b4a-8308-442b-b27a-e09eaec85e05 — Barometer Aug 2026: index, 72 % of university sites under-recruit, Kapazitätsinitiative 2030, accessed 2026-11-06
- https://www.vfa.de/download/studienstandort-barometer-okt-2025-praesentation.pdf — DE share 4.5 %→3.0 %, 33k→24k participants, MFG/StandVKlV, ranked hurdles, accessed 2026-11-06
- https://clinicaltrials.gov/api/v2/studies — own counts of industry interventional trials by start year and country, accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42861283%20AND%20SRC:MED&format=json&resultType=core — Lancet Reg Health Eur 2026, EU trials −13.5 %, accessed 2026-11-06
- https://www.raps.org/resource/study-europe-s-share-of-clinical-trials-is-declining-amid-shift-toward-asia.html — summary of the same study, accessed 2026-11-06
- https://www.efpia.eu/media/3edpooqp/assessing-the-clinical-trial-ecosystem-in-europe.pdf — IQVIA/EFPIA Aug 2024, EEA share 22 %→12 %, recruitment times, accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:40899933%20AND%20SRC:MED&format=json&resultType=core — JAMA Netw Open 2025, 31.1 % discontinued, 45.4 % poor recruitment, accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:34823582%20AND%20SRC:MED&format=json&resultType=core — Trials 2021, reasons for recruitment failure (DE/CH/CA), accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38167484%20AND%20SRC:MED&format=json&resultType=core — Trials 2024, CTR/CTIS burden, accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42837073%20AND%20SRC:MED&format=json&resultType=core — TIRS 2026, CTR implementation workload, DE vs ES, accessed 2026-11-06
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:42925427%20AND%20SRC:MED&format=json&resultType=core — J Neural Transm 2026, German Parkinson trial barriers, accessed 2026-11-06
- https://www.jonesday.com/en/insights/2026/05/the-proposed-european-biotech-act-100-days-on — Biotech Act CTR timelines 106→76 days, FAST-EU pilot, accessed 2026-11-06
- https://www.appliedclinicaltrialsonline.com/view/addressing-current-challenges-in-the-site-landscape — SCRS 2023 site technology training hours, accessed 2026-11-06
- https://www.capterra.com.de/directory/30458/clinical-trial-management/software — 65 CTMS products listed, accessed 2026-11-06
- https://www.kununu.com/de/iqvia/kommentare ; https://www.kununu.com/de/parexel-international1/kommentare ; https://www.kununu.com/de/icon-clinical-research/kommentare — CRO employee reviews (summary/page 1), accessed 2026-11-06
- https://www.krebs-kompass.de/showthread.php?t=60921 ; https://www.krebs-kompass.de/showthread.php?t=69735 ; https://www.krebs-kompass.de/showthread.php?t=54471 — the only trial threads in 457 titles scanned (2011–2017), accessed 2026-11-06
- https://pharmaphorum.com/market-access/europes-new-hta-reality-jca-one-year — JCA one year: resource load, 100-day timeline, 57 % late LOIs, ~58 JCAs 2026, accessed 2026-11-06
- https://www.efpia.eu/news-events/the-efpia-view/blog-articles/from-guidance-to-implementation-efpia-s-reflections-on-eu-hta-scoping-pico-exercises/ — PICO scoping concerns, accessed 2026-11-06
- https://www.gkv-spitzenverband.de/gkv_spitzenverband/presse/fokus/amnog_verhandlungen/s_thema_amnog_verhandlungen.jsp — AMNOG 507 substances, 922 negotiations, opt-outs, accessed 2026-11-06
- https://medtecheurope.org/wp-content/uploads/2025/01/mte-ivdr-mdr-survey-report-highlights-final.pdf — MDR timelines and cost structure, accessed 2026-11-06
- https://www.bvmed.de/download/mdr-ivdr-umfrage-auswertung-2025.pdf — DACH MDR/IVDR survey 2025, accessed 2026-11-06
- https://www.bvmed.de/download/zusammenfassung-der-ergebnisse-der-bvmed-herbstumfrage-2025.pdf — 93 % SMEs, sector figures, accessed 2026-11-06
- https://www.mhc.ie/latest/insights/eu-commission-proposes-reform-of-the-medical-devices-regulation — MDR/IVDR targeted revision 16 Dec 2025, accessed 2026-11-06
- https://api.ted.europa.eu/v3/notices/search — TED notices 189396-2025, 269243-2025, 673984-2025, 761998-2025, 379963-2026, 396194-2026, 481787-2026, 518174-2026, 177834-2026, 343840-2025, 762721-2026, 63363-2025, 483613-2025, 688078-2026, 252303-2025, 76741-2025, 484262-2026, 680181-2026, 450104-2025, accessed 2026-11-06
- https://www.bundesgesundheitsministerium.de/presse/pressemitteilungen/finanzentwicklung-gkv-2025 — GKV 2025 results by spending area, admin costs, reserves, accessed 2026-11-06
- https://www.gkv-spitzenverband.de/gkv_spitzenverband/presse/fokus/verwaltungskosten_kk.jsp — admin costs 2024 (€12.63bn, €169.54/insured), accessed 2026-11-06
- https://www.buzer.de/4_SGB_V.htm — § 4 Abs. 5 SGB V admin cap from 2027, accessed 2026-11-06
- https://www.krankenkasseninfo.de/ratgeber/nachrichten/krankenkassen-muessen-bei-verwaltung-und-werbung-sparen-62674.html — BStabG admin/advertising cap, expected savings, accessed 2026-11-06
- https://luenendonk.de/wp-content/uploads/2026/08/LUE_Digitale_Transformation_in_der_GKV_PI_f.pdf — insurer survey 2026 (AI, retirement wave, ePA), accessed 2026-11-06
- https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken — competitor in insurer claims automation, accessed 2026-11-06
- https://www.aok.de/pp/gg/daten-und-analysen/krankengeld/ — Krankengeld €21.63bn 2025 (context), accessed 2026-11-06
- https://www.kununu.com/de/barmer/kommentare ; https://www.kununu.com/de/dak-gesundheit/kommentare ; https://www.kununu.com/de/aok-plus/kommentare ; https://www.kununu.com/de/mdk-medizinischer-dienst-der-krankenversicherung-in-bayern/kommentare — payer/MD employee review summaries, accessed 2026-11-06
- https://md-bund.de/fileadmin/dokumente/Pressemitteilungen/2026/2026_07_15/_26-07-15_FIN_PM_Report_Pflegebeduerftigkeit.pdf — >3m care assessments 2025, Pflegegeld share, accessed 2026-11-06
- https://www.vdek.com/magazin/ausgaben/2025-04/modernisierung-pflegebegutachtung.html — assessment growth since 2014, MD reform wishes, accessed 2026-11-06
- https://www.pkv.de/verband/presse/meldungen/pkv-stellungnahme-zu-finanztip-umfrage-ueber-kostenerstattung/ — >70m PKV invoices/yr, complaint figures, accessed 2026-11-06
- https://www.pkv.de/verband/presse/pressemitteilungen/goae-entwurf-erfolgreiche-aktualisierung-als-basis-fuer-ein-zuegiges-verordnungsverfahren/ — GOÄ draft update, 2028 target, accessed 2026-11-06
- https://www.buzer.de/303e_SGB_V.htm — FDZ data access for natural and legal persons, accessed 2026-11-06
- https://www.pharmazeutische-zeitung.de/53-antraege-auf-datennutzung-fuer-forschung-163005/ — FDZ 53 applications, claims data only, accessed 2026-11-06
- https://www.aerzteblatt.de/news/pakt-fur-offentlichen-gesundheitsdienst-soll-ende-des-jahres-auslaufen-56bc8c97-3fb3-46ea-9ef9-1de7cbb06d5e — ÖGD pact ends 2026, accessed 2026-11-06
- https://www.aerzteblatt.de/news/appell-von-amtsaerzten-pakt-fuer-den-oegd-ueber-2026-hinaus-verstetigen-9f2e7090-b4f9-440f-ad7e-56b5932a608b — ÖGD pact €4bn, >5,000 posts, accessed 2026-11-06
- https://www.ema.europa.eu/en/documents/report/2025-annual-report-eudravigilance-european-parliament-council-commission_en.pdf — ICSR volume +0.5 % in 2025, accessed 2026-11-06
