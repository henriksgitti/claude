# Pain mining: clinicians, nurses, practice & hospital staff (DE)
Task: A4 | Date: 2026-11-06 | Status: draft
Revised 2026-11-07 (task A14): critic fixes from `research/reviews/2026-11-06-pain-professionals.md`. Tender eligibility added (new section "Tender access check"), Harzklinikum re-labelled as clinical decision support with an MDR caveat, S3 rules updated from `research/hospital-billing-audits.md` (A11), nurse headcount and practice count replaced, leadership count corrected to 8 of 9.

Method: recipes from `research/sources-map.md`. Fetched with curl and converted to text locally. Also used: TED API v3 (contract notices only, `notice-type=cn-standard`, de-duplicated by buyer), Europe PMC REST, the medi-learn Discourse JSON API, and kununu employer pages. Grades follow `CLAUDE.md` rule 2. Online voices are quoted without usernames.

**Limits:**
- Reddit was not used (blocked, see A2).
- kununu shows only page 1 per employer. The other pages sit behind a sign-up wall, which I did not bypass. I therefore used kununu's own AI summaries ("KI-Zusammenfassung"), which are [C] and machine-written.
- Both forums are low-traffic. On krankenschwester.de I opened 3 threads and only scanned the titles of the rest.
- LinkedIn job counts proved unusable: "Kodierfachkraft" returned "4,000+ Open Roles", which points to fuzzy matching. StepStone no longer shows counts.

## Findings
- **Documentation and verification duties are the most consistently measured pain, but the size depends on who measures.**
  - DKI hospital survey (n=400, Sep 2025): physicians spend on average 3 h per working day on documentation, nurses 2.8 h. Converted to staff, that equals "knapp 66.300 von rund 176.800 ärztlichen Vollkräften (38 %)" and ~137,000 of ~391,000 nursing FTE (35 %). 88 % of hospitals say the load grew in the last 12 months [B] ([DKI 2025](https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf)).
  - An independent time-motion study (9 physicians, 216 h of observation) measured less: 93.1 min/day, i.e. 19.4 % of working time [A] ([DMW 2024, PMID 38977000](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38977000%20AND%20SRC:MED&format=json&resultType=core)).
  - Nursing chamber survey (n=528, Aug 2024): 45 % spend 2.5–5 h/day on documentation; 52 % say their software helps "wenig bis gar nicht" [B] ([Landespflegekammer via DKG](https://dkgev.de/fileadmin/default/Mediapool/1_DKG/1.7_Presse/07_Landespflegekammer_Umfrage_Entbuerokratiesierung.pdf)).
- **The most painful documentation is driven by money, not care.** Hospitals name these as the most time-consuming duties: answering Medizinischer Dienst (MD) queries and documenting to MD audit standards, quality-assurance checklists, staffing-ratio evidence (PpUGV/PPBV/PPP-RL), and ICD/OPS coding [B] ([DKI 2025](https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf)). Hospitals already buy help:
  - Charité tendered a framework contract for "Kodier-Unterstützungsleistungen" (outsourced coding support, 48 months) [A] ([TED 186365-2025](https://api.ted.europa.eu/v3/notices/search)).
  - Medizinische Universität Lausitz tendered "Kodiersoftware für fallbegleitende und automatisierte Kodierung" using "verschiedenen KI-Ansätzen" [A] ([TED 214386-2026](https://api.ted.europa.eu/v3/notices/search)).
  - **Neither tender is open to a newcomer.** Charité requires 3 references, "Mind. zwei Unternehmensreferenzen sind ein deutsches Universitätsklinikum" (2026 re-tender: each with ≥500 primary codings). Lausitz requires in-field turnover "pro Jahr mind. 1.000.000 EUR", use "in mindestens drei Universitätsklinika oder Maximalversorgern", and 50 staff [A] (TED selection criteria, see "Tender access check").
  - *Inference:* revenue protection gives this the clearest budget owner among staff-side problems, but for incumbents. A startup's first sale would have to come from smaller tickets (UK Frankfurt bought coding-revision software for €181,800 over 3 years, A11), private hospital groups that buy outside TED, or a partnership. The audit regime does tighten on 1 Jan 2027 under the enacted BStabG (A11).
- **Hospitals buy documentation tooling with public money, and that money is shifting.**
  - Since 2025, 22 hospital buyers have issued tenders with "Patientenportal" in the title (mostly KHZG FTB2). 8 hospital buyers tendered speech recognition [A] (TED, contract notices, de-duplicated by buyer).
  - Harzklinikum tendered a **clinical decision-support system** that includes LLM-drafted discharge letters ("Entscheidungsunterstützung medizinische Dokumentation – LLM-basierte Arztbriefschreibung", KHZG FTB4 = "klinischen Entscheidungsunterstützungssystemen"). The scope includes AI that should "in Echtzeit patientenindividuelle Hinweise zu möglichen Erkrankungen, Komplikationen oder Risiken" generate [A] ([TED 492877-2025](https://api.ted.europa.eu/v3/notices/search)). **Regulatory caveat [A]:** under MDR Annex VIII Rule 11, software "die dazu bestimmt ist, Informationen zu liefern, die zu Entscheidungen für diagnostische oder therapeutische Zwecke herangezogen werden, gehört zur Klasse IIa" or higher ([MDR 2017/745, EUR-Lex](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32017R0745)). MDCG 2019-11 rev. 1 (Jun 2025) says decision-support software that combines medical knowledge with patient-specific data to give recommendations is "qualified as medical devices", while systems that only store, transfer or format data are not ([MDCG 2019-11 rev. 1](https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=md_mdcg_2019_11_guidance_qualification_classification_software_en.pdf), pp. 25–26). *Inference:* a documentation-only tool (drafting, summarising) can likely stay outside the MDR, but adding patient-specific risk hints pulls the product into class IIa+ certification, i.e. a notified body (MDR timelines: see `pain-industry.md` I4).
  - KHZG purchase money is a **one-off fund in its tail**: €3bn federal, with Land applications due "bis zum 31. Dezember 2021" [A] ([§ 14a KHG](https://www.gesetze-im-internet.de/khg/__14a.html)). No successor programme was found (A9). The 2025–26 tenders spend money granted years ago; it is not a recurring budget.
  - From 2027, the KHZG penalty (up to 2 % per case) starts to weigh actual *use* of digital services: 20 % weight in 2027, rising to 80 % in 2031 [A] ([GKV-SV/DKG agreement](https://gkv-spitzenverband.de/media/dokumente/krankenversicherung_1/krankenhaeuser/abrechnung/zu___abschlaege/digitalisierung/DigitalisierungsabschlagsVb_mit_Anhaengen_1-4_20.08.2024.pdf)).
  - The flat 2.5 % nurse-relief top-up to the Pflegebudget (2025–26) will be clawed back from 2027. From 2027, Pflegebudget overruns are also no longer refinanced [A] ([§ 6a KHEntgG as amended by the BStabG, 24 Jul 2026](https://www.buzer.de/6a_KHEntgG.htm)).
  - *Inference:* hospitals face stronger pressure to make nursing efficient but have less earmarked money for it.
- **Practices drown in payer paperwork and unreliable IT.**
  - Requests from health-system institutions cost practices "mehr als zwei Millionen Arbeitsstunden" per year [B] ([KBV PM, Mar 2025](https://www.kbv.de/presse/pressemitteilungen/2025/entbuerokratisierung-entlastet-praxen-und-kostentraeger-formfreie-anfragen-heut-zettelwust-morgen-digital)).
  - KBV's 23 proposals would free "rund acht Arbeitstage à zehn Stunden pro Praxis" a year; the federal health ministry (BMG) has taken up 3 of them [B] ([KBV, Aug 2026](https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2026/08-20/kbv-unterstuetzt-massnahmen-des-bmg-zum-buerokratieabbau-und-fordert-weitere-entlastungen)).
  - More than half of practices report daily or weekly outages of the national health-data network (Telematikinfrastruktur, TI). Only 13 % communicate mostly digitally with hospitals [B] ([KBV PraxisBarometer 2025, n≈1,700](https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2025/10-16/praxisbarometer-2025-niedergelassene-bleiben-vorreiter-in-sachen-digitalisierung)).
- **Staff shortage is the dominant employee complaint, but the employer-review data points to leadership more than to software.**
  - Shortage: in kununu's AI summaries, "Personalmangel" appears for 7 of 9 hospital and care chains, and leadership/communication complaints for 8 of 9 (Charité: mixed). Documentation and IT do not surface in the summaries, but the summaries are machine-written and short, so absence is not evidence of absence [C] (kununu, see table).
  - Physicians: 49 % feel frequently overloaded, 28 % consider leaving patient care, 59 % rate physician staffing poor, and two-thirds are dissatisfied with workplace IT [B] ([MB-Monitor 2024, n=9,649, via zm-online](https://www.zm-online.de/news/detail/viele-aerztinnen-und-aerzte-gehen-ueber-ihre-grenzen-hinaus); [praktischArzt](https://www.praktischarzt.de/magazin/mb-monitor-2024/)).
  - Agency nursing is shrinking: 42,649 agency nurses in 2023, 31,503 (1.8 %) in Aug 2025 [A] ([BT-Drs. 21/5270](https://dserver.bundestag.de/btd/21/052/2105270.pdf)).
- **AI documentation works, but measured gains are modest and the space is crowded.**
  - A pre-post study (52 nurses, 14 long-term-care homes) found 15 minutes less documentation per morning shift with the voize speech assistant [A] ([JMIR 2026, PMID 41950503](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41950503%20AND%20SRC:MED&format=json&resultType=core)).
  - A US multisite cohort (8,581 clinicians): AI scribes saved 16.0 min of documentation per 8 scheduled patient hours, with no change in after-hours EHR time [A] ([JAMA 2026, PMID 41920565](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=DOI:%2210.1001/jama.2026.2253%22&format=json&resultType=core)).
  - voize raised a $50m Series A and says it is used in 1,100 facilities in DE/AT [B] ([HealthCapital](https://www.healthcapital.de/news/artikel/berlins-voize-raises-50m-for-nursing-ai)).
  - Practice phone AI: 10 vendors priced at €9–229/month [B] ([medizinio](https://medizinio.de/digitalisierung/telefonassistent-arztpraxis)).

## Summary table
Signals = independent items I opened (threads or employer pages counted once). Titles only = thread title seen, body not opened. WTP = willingness to pay.

| # | Problem | Who has it | Who pays / could pay | [A]/[B] items | [C] signals | WTP evidence | Strength (inference) |
|---|---|---|---|---|---|---|---|
| S1 | Clinical documentation load in hospitals (discharge letters, ward documentation) | ~176,800 physician FTE, ~391,000 nursing FTE in hospitals | Hospitals (KHZG FTB4 money, own IT budget) | 6 (DKI 2025, DMW 2024, MB-Monitor 2024, Landespflegekammer 2024, JAMA 2026, JAMIA 2026) | 2 threads opened (krankenschwester.de doc thread 2025; medi-learn) + titles | 8 hospital buyers of speech recognition; Harzklinikum CDSS + LLM discharge letters (KHZG, one-off money). Access: most speech-recognition tenders need 2–6 references (often with a named KIS such as ORBIS or iMedOne), Vivantes ≥€1m/yr in-field turnover; UK Saarland: "kein Mindestumsatz", 2 references + C5 for cloud | **High** pain; **crowded** (Microsoft/Nuance, Doctolib, myScribe, KIS vendors); modest measured gains; **low direct access**; CDSS features → MDR class IIa+ |
| S2 | Nursing documentation in long-term and home care | 446,425 employees in 15,549 home-care services + 817,711 in 16,505 residential care facilities (2023, all staff, not only nurses) [B] ([sozialpolitik-aktuell, Destatis data](https://www.sozialpolitik-aktuell.de/files/sozialpolitik-aktuell/_Politikfelder/Gesundheitswesen/Datensammlung/PDF-Dateien/abbVI54_55.pdf)) | Operators (cost passes into negotiated care rates); §8(8) SGB XI subsidy | 4 (JMIR 2026, Fraunhofer IML 2023, DBfK 2026, BEEP law) | 3 threads (2 opened: 2026 dictation, 2025 doc tasks; 1 founder probe) | voize 1,100 facilities, $50m | **High** pain; a well-funded leader already exists |
| S3 | MD audits, coding and billing-proof documentation in hospitals | Physicians, coders, medical controlling | Hospitals (revenue at stake) | 3 (DKI 2025, GKV-SV audit regime, § 275c) | 1 thread (medi-learn "Fallbegleitendes Kodieren", 2025) | Charité coding-services framework (48 mo; needs 2 university-hospital references); Lausitz AI coding tender (≥€1m/yr in-field turnover, 3 university/max-care sites, 50 staff); DKI 2026: median planned AI spend €40k/hospital (A11) | **High buyer budget, low direct startup access** via tender; incumbents known (Tiplu/LOGEX, ID Berlin, Dedalus; Munich startup calliora, A11); stricter audit quotas from 1 Jan 2027 enacted (BStabG, A11) |
| S4 | Practice paperwork: free-form payer/MD/agency requests, forms, audit threats | 191,875 physicians and psychotherapists in contract practice (end-2025, KBV data via [PZ](https://www.pharmazeutische-zeitung.de/mehr-aerzte-aber-weniger-zeit-fuer-patienten-163553/)) [B]; GPs most | Practices; insurers/MD as co-beneficiaries (BARMER/KBV/MD initiative) | 3 (KBV 2025, KBV 2026, KBV PraxisBarometer 2025) | 1 thread (medi-learn billing question 2025) | Low (practices are price-sensitive); payer-side initiative | Medium; partly fixable by policy (standard forms) |
| S5 | Phone and reception overload; medical assistant (MFA) shortage | Practices, MFAs | Practices (€9–229/month tools) | 3 (HNO-Verband survey 2024, BA 2026, Ärzteblatt 2025) | 0 opened | Active market at low prices | Medium pain; **crowded, low price** |
| S6 | TI outages, practice-software (PVS) lock-in, no digital link to hospitals | Practices; hospitals | gematik/vendors; practices | 2 (KBV PraxisBarometer 2025, MB-Monitor 2024) | 1 thread (medi-learn KIM 2024) | — | Pain high, but **not startup-addressable** (infrastructure) |
| S7 | Staffing, rostering and short-notice cover | Nurses, ward managers, physicians | Hospitals/care operators (rostering software; agency premiums no longer refinanced) | 4 (BT-Drs. 21/5270, § 6a KHEntgG, MB-Monitor, BA 2026) | 9 kununu employer pages; ~6 forum titles | ≥10 hospital buyers of rostering/time-tracking software. Access: references from operators with ≥500 FTE (Pfalzklinikum) or ≥600 beds (Klinikverbund Südwest, plus €10m comparable turnover), 3 references (Chemnitz) | Pain high; mature software market; root cause is headcount; **no direct access** |
| S8 | Discharge and transition coordination (finding follow-up care) | Hospital social services, case managers | Hospitals (bed blocking), KHZG FTB2 | 3 (RWI 2024, KBV PraxisBarometer 2025, TED notices) | 0 opened | Helios group framework (KHZG certificate + reference from a hospital group with ≥2,000 beds + KIS references); 5 hospital buyers (UK Dresden: ≥€500k/yr in-field turnover, 3 reference hospitals; UK Magdeburg: 3 references, ISO 27001) | Medium–high; overlaps A3 P2/P7; capacity is the root cause; **no direct access** |
| S9 | Leadership, communication, retention | All staff | Employers | 2 (MB-Monitor, DBfK 2026) | 9 kununu summaries (8/9 critical of leadership, Charité mixed) | — | High pain; **not a product problem** (inference) |
| S10 | Onboarding foreign-trained staff (recognition, language) | Hospitals and care operators | Employers | 2 (Destatis 2026, BA 2026) | 0 opened | Recruiter fees `[UNVERIFIED]` | Low evidence; process times not found |

## Details

### S1 Clinical documentation load in hospitals
- **[B] DKI flash survey for DKG (Sep 2025, 400 hospitals, "Repräsentativbefragung"):**
  - Physician FTE: mean 3 h/day on documentation (median 3, quartiles 2–3.5).
  - Nursing FTE: mean 2.8 h/day.
  - 81 % of hospitals have clinically trained staff working only on documentation/admin.
  - 34 % hired extra physicians or nurses and 51 % extra admin staff, mainly because of the hospital reform (KHVVG).
  - Freeing 1 h/day would equal "22.097 Ärzte" and 48,938 nursing FTE ([DKI](https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf)).
  - Caveat: these are self-estimates by hospital management (400 hospitals answering for their staff) for their lobby association. The 38 %/35 % FTE equivalents are arithmetic on that self-estimate; do not use them for sizing.
- **[A] Counter-measure, DMW 2024:** direct observation of 9 physicians over 216 h at one urban hospital: 93.1 ± 23.4 min/day (19.4 %) on documentation; internists 120.2 min (25 %). Direct patient-related time was 33.8 min (7 %), or 80.7 min including surgery ([PMID 38977000](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38977000%20AND%20SRC:MED&format=json&resultType=core)). Small sample, but measured, not self-estimated.
- **[B] MB-Monitor 2024 (9,649 employed physicians, ~90 % in hospitals):** two-thirds "eher unzufrieden" or "unzufrieden" with workplace IT ([praktischArzt](https://www.praktischarzt.de/magazin/mb-monitor-2024/)). The "3 h/day admin" figure attributed to MB-Monitor appeared only in search snippets `[UNVERIFIED]`.
- **[A] Hospital purchasing (TED, contract notices since 2025-01-01, de-duplicated by buyer):**
  - Speech recognition, 8 hospital buyers: BG Klinikum Hamburg, Mittweida, Rems-Murr, Dietrich-Bonhoeffer-Klinikum, UK Saarland, Emmendingen, Vivantes ("Cloudbasierte Spracherkennung zur medizinischen Anwendung"), Klinikum Region Hannover.
  - Clinical decision support incl. AI discharge letters: Harzklinikum, "Entscheidungsunterstützung medizinische Dokumentation – LLM-basierte Arztbriefschreibung", funded as KHZG FTB4 ("§19 Abs. 1 Nr. 4 KHSFV": "klinischen Entscheidungsunterstützungssystemen"), 36 months. The scope includes real-time "patientenindividuelle Hinweise zu möglichen Erkrankungen, Komplikationen oder Risiken". Eligibility: at least one reference proving "die erfolgreiche Implementierung des vollumfänglichen Beschaffungsgegenstandes in einer deutschen Klinik" ([TED 492877-2025](https://api.ted.europa.eu/v3/notices/search)). MDR caveat: see Findings (Rule 11 → class IIa+ for the decision-support part).
- **[A] Evidence of effect is modest:**
  - US multisite cohort: −16.0 min of documentation per 8 scheduled patient hours, no change in after-hours EHR time ([JAMA 2026](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=DOI:%2210.1001/jama.2026.2253%22&format=json&resultType=core)).
  - Randomised crossover of two ambient scribes (n=136 analysed): both reduced burnout, and the time difference between tools was 3.19 min/day ([JAMIA 2026, PMID 41729180](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41729180%20AND%20SRC:MED&format=json&resultType=core)).
  - German hospital network (ScanProCare!): normal wards saved 9,235 h/year of documentation, but "some tasks became more time-consuming" ([Stud Health Technol Inform 2025, PMID 41041759](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41041759%20AND%20SRC:MED&format=json&resultType=core)).
- **[C] Voices:**
  - In a 2025 krankenschwester.de thread asking nurses which documentation tasks cost the most time, replies named double documentation and rigid electronic records:
    - "Was nervt ist Doppeldoku"
    - "Das System ist weit weniger intelligent als angekündigt"
    - On rates/doses on paper: "häufig vergessen, unleserlich, kein Platz" ([thread](https://www.krankenschwester.de/forum/themen/frage-an-pflegekraefte-welche-doku-aufgaben-kosten-euch-am-meisten-zeit.150717/)).
  - Counter-voice in the same thread: "Eine herkömmliche Dokumentation in Papierform ist jederzeit konkurrenzfähig."
  - 2026 dictation thread: "Cloud-Server-Software ist auf den Klinik-Rechnern untersagt" ([thread](https://www.krankenschwester.de/forum/themen/diktiersoftware-fuer-die-pflegerische-dokumentation-was-nutzt-ihr.151070/)).
- *Inference:* the pain is real and budgeted, but the buyer is the hospital IT/KIS stack. Cloud restrictions and incumbent vendors (Microsoft/Nuance Dragon in tenders; myScribe and Doctolib named in search snippets `[UNVERIFIED]`) make this a hard wedge for a newcomer.

### S2 Nursing documentation in long-term and home care
- **[A]** voize pre-post time-motion study (52 registered nurses, 14 LTC facilities, 770 h observed): adjusted −15 min (SE 3.36) of documentation per morning shift ([JMIR 2026](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41950503%20AND%20SRC:MED&format=json&resultType=core)). Single-group design. Conflicts checked (full text via Europe PMC, PMC13061367): the first author "is employed by voize GmbH"; the other four authors (Charité geriatrics) declare none; funded by the federal research ministry (PYSA project). Treat as manufacturer-associated.
- **[B] Fraunhofer IML whitepaper (Sep 2023; survey Feb–Mar 2021, 74 nurses, care homes):** self-reported 52 min of documentation per shift vs 109 min measured by sensors ([IML](https://www.iml.fraunhofer.de/content/dam/iml/presse/whitepaper/32_Whitepaper_Pflegedokumentation_in_Krankenh%C3%A4usern.pdf)). **Data >3 years old.**
- **[B] DBfK "Pflege, wie geht es dir?" 2026** (not representative; >3,000 respondents): among care-business owners (n=134), 87 % name bureaucracy as their top 2026 issue, 80 % refinancing of high costs, 71 % digitalisation and 67 % staff shortage. DBfK comments that digitalisation is "eher als Belastung empfunden, nicht als Unterstützung" ([DBfK](https://www.dbfk.de/media/docs/newsroom/pressemitteilungen/2026/Pflege-wie-geht-es-dir-2026.pdf)).
- **[B] Competitor:** voize, $50m Series A (Balderton, Nov 2025), 1,100 facilities in DE/AT, 75,000 nurses (company figures via [HealthCapital](https://www.healthcapital.de/news/artikel/berlins-voize-raises-50m-for-nursing-ai)).
- **[A/B] Policy can shrink the problem:** the care-bureaucracy law (BEEP), passed 6 Nov 2025, limits care documentation "auf das notwendige Maß" and simplifies forms and MD inspections ([BMG](https://www.bundesgesundheitsministerium.de/presse/pressemitteilungen/befugniserweiterungsgesetz-bundestag-06-11-25.html)).
- **[C]**
  - A 2026 home-care nurse reports speech input in her cloud app works "insgesamt gut", but sentence boundaries are not recognised ([thread](https://www.krankenschwester.de/forum/themen/diktiersoftware-fuer-die-pflegerische-dokumentation-was-nutzt-ihr.151070/)).
  - 3 of the 6 recent posts in the EDV and documentation subforums come from people building tools ("Ich arbeite gerade an einer kleinen Idee…"; "beschäftige mich beruflich mit Sprachtechnologie"; "Progressive Pflegesoftware – Ich brauche eure Unterstützung!" [title only]) ([subforum](https://www.krankenschwester.de/forum/subforen/edv-im-pflegebereich-pflegeinformatik.61/)). *Inference:* founders are already crowding this space.

### S3 MD audits, coding and billing-proof documentation in hospitals
- **[B]** DKI's list of the most time-consuming duties "mit kaum erkennbarem Nutzen", in its order: MD queries/MD-proof documentation; QA checklists/G-BA requirements; staffing instruments (PpUGV, PPBV, PPP-RL); proof of length-of-stay necessity; ICD/OPS coding incl. OPS complex codes; redundant entry due to missing IT ([DKI 2025](https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf)).
- **[A] Purchasing:**
  - Charité: framework for "Kodier-Unterstützungsleistungen" (CPV health services, 48 months), notices in 2025 and again 2026.
  - MUL Lausitz: "System für fallbegleitende und automatisierte Kodierung … unter Einsatz von verschiedenen KI-Ansätzen", 60 months ([TED 186365-2025, 213191-2026, 214386-2026](https://api.ted.europa.eu/v3/notices/search)).
- **[A] Rules:** audit quotas per hospital per quarter under § 275c SGB V; GKV-SV publishes quarterly statistics ([GKV-SV](https://www.gkv-spitzenverband.de/krankenversicherung/krankenhaeuser/krankenhaeuser_abrechnung/kh_pruefung_statistik/pruefquoten_und_statistik.jsp)). Audit volumes and repayment sums were **not extracted** (XLSX files not opened).
- **Rules 2027, corrected by A11 [A]** (`research/hospital-billing-audits.md`): the "sample audits from 2027" were a KHVVG *draft* and are **not** in the enacted law; single-case audits stay. The enacted BStabG rewrites § 275c SGB V from 1 Jan 2027: quotas up to 5 % / 20 % / 40 % depending on the share of audits passed (today max. 15 %), and €500 per reduced invoice. A11's static simulation puts ~7 in 10 hospitals in the 40 % tier. The earlier snippet figures (KHVVG samples; 10 %→15 %) are superseded.
- **[C]** On case-accompanying coding, a junior internist writes that the coder's questions are often ones "die ich … selber noch nicht beantworten kann" and "medizinisch unsinnig" ([medi-learn, Apr 2025](https://forum.medi-learn.de/t/fallbegleitendes-kodieren/99622)).
- *Inference:* every audited euro is hospital revenue, so willingness to pay is direct, and it fits the CEO's automation profile. But hospitals already pay coders, medical controllers and coding software, and AI coding is already a tendered product category with incumbents (A11). A newcomer must beat that stack and cannot win the large tenders directly (see "Tender access check").

### S4 Practice paperwork
- **[B]** BARMER, KBV, KVWL and MD Westfalen-Lippe run a joint initiative on "formfreie Anfragen": "mehr als zwei Millionen Arbeitsstunden" per year. These requests must be answered "manuell und ohne Praxisverwaltungssystem". KVWL: "Zwei Monate im Jahr ist eine Praxis ausschließlich mit Bürokratie beschäftigt" ([KBV, 31 Mar 2025](https://www.kbv.de/presse/pressemitteilungen/2025/entbuerokratisierung-entlastet-praxen-und-kostentraeger-formfreie-anfragen-heut-zettelwust-morgen-digital)).
- **[B]** KBV: 23 proposals, ~€400m/year savings, ~8 ten-hour workdays per practice. The BMG adopted 3, including a €300 de-minimis threshold for cost-efficiency audits ([KBV, 20 Aug 2026](https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2026/08-20/kbv-unterstuetzt-massnahmen-des-bmg-zum-buerokratieabbau-und-fordert-weitere-entlastungen)).
- **Stale [B]:** the 2016 Bureaucracy Index put the load at 52m hours/year for ~150,000 office-based physicians ([Ärzteblatt, 22 Nov 2016](https://www.aerzteblatt.de/news/niedergelassene-aerzte-wenden-52-millionen-stunden-fuer-buerokratie-auf-3bccf9be-2a59-4087-b2db-15e97d46e935)). Context only; **>3 years old**.
- **[C]** A 2025 medi-learn thread on billing a time-based fee code twice shows rule uncertainty ("In unserer Praxis gibt es dazu gegensätzliche Meinungen") ([thread](https://forum.medi-learn.de/t/kodierung-von-mehrfachleistungen/99844)).
- *Inference:* insurers co-own the problem. A request-handling layer between payers and practice software could sell to insurers or the MD rather than to price-sensitive practices. Standard forms (policy) may shrink it.

### S5 Phone/reception overload and MFA shortage
- **[B]** ENT physicians' association survey: "fast zwei Drittel der Praxen" lost staff in 12 months and "jede zweite Praxis suche dringend nach Personal". Consequences: fewer services (67.2 %), longer waits (47.7 %) ([Ärzteblatt, 3 Jul 2024](https://www.aerzteblatt.de/themen/medizinische-fachangestellte/jeder-zweiten-hno-praxis-fehlt-personal-ca8e3832-4066-4283-873c-61c700aca121)). Single specialty.
- **[B]** BA 2025 shortage analysis: 157 shortage occupations, with "vor allem Pflege- und Gesundheitsberufe" among the strongest ([BA, 2026](https://www.arbeitsagentur.de/presse/2026-32-fachkraefte-bleiben-knapp-zuwanderung-gewinnt-weiter-an-bedeutung)). An MFA shortage score of 2.0 (borderline) is `[UNVERIFIED]` (snippet).
- **[B] Market:** 10 AI phone-assistant vendors at €9–229/month, including Doctolib (formerly aaron.ai) ([medizinio](https://medizinio.de/digitalisierung/telefonassistent-arztpraxis)). A GP association representative: "keine Schnittstelle unserer IT-Systeme mit dem KI-Telefonassistenten". The consumer association vzbv demands transparency ([Ärzteblatt, 28 Aug 2025](https://www.aerzteblatt.de/themen/praxismanagement/diskussion-um-ki-assistenten-in-arztpraxen-13b8abd7-946e-42f5-ae09-235973e167e3)).
- *Inference:* proven willingness to pay, but a commoditising, crowded market. Avoid as a core idea.

### S6 TI outages, PVS lock-in, practice–hospital gap
- **[B]** PraxisBarometer 2025 (IGES for KBV, ~1,700 practices):
  - >50 % report daily or weekly TI outages.
  - Satisfaction with e-prescription and digital sick notes "fast 80 Prozent".
  - 87 % receive electronic doctor's letters, but only 13 % communicate mostly digitally with hospitals.
  - 85 % expect "großen Nutzen" from a digital hospital discharge letter.
  - PVS switching is blocked by long contracts, cost and fear of data loss ([KBV](https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2025/10-16/praxisbarometer-2025-niedergelassene-bleiben-vorreiter-in-sachen-digitalisierung)).
- **[C]** On using KIM (the TI secure-messaging service) with hospitals: "die KH hier in der Umgebung sagen, sie könnten es nicht nutzen"; each KIM address costs "6,55€ zzgl. MWSt pro Monat" (user claim) ([medi-learn, Apr 2024](https://forum.medi-learn.de/t/kim-dienst-nutzt-ihr-ihn-fuer-arztbriefe-etc/98837)).
- *Inference:* infrastructure pain owned by gematik and the vendors. The addressable slice is the hospital→practice discharge-letter flow (links to S8).

### S7 Staffing, rostering, short-notice cover
- **[A] BT-Drs. 21/5270 (7 Apr 2026):**
  - 1,767,799 employees in nursing occupations (Aug 2025), of which 31,503 agency workers (1.8 %). Peak was 42,649 (2.5 %) in 2023. Bavaria: 3,174 (1.3 %).
  - IW survey of ~4,000 agency nurses: motives are pay, "Einfluss auf die Dienstpläne" and appreciation ([Bundestag](https://dserver.bundestag.de/btd/21/052/2105270.pdf)).
- **[A]** § 6a KHEntgG: agency pay above the collective-agreement rate and placement fees are excluded from the Pflegebudget. From 2027, Pflegebudget cost overruns ("Mehrkosten") are no longer reimbursed ([buzer.de consolidated text, BStabG version](https://www.buzer.de/6a_KHEntgG.htm)).
- **[A] Purchasing (TED, contract notices since 2025):** ≥10 hospital buyers of rostering/time-tracking software: Klinikum St. Georg, UK Dresden, Kliniken Lörrach, Klinikum Chemnitz, Mühlenkreiskliniken, Hufeland Klinikum, Pfalzklinikum, UK Münster, Klinikum Bremerhaven, Klinikverbund Südwest.
- **[B]** MB-Monitor 2024: 59 % rate physician staffing poor; 42 % report posts cut in the last 2 years ([praktischArzt](https://www.praktischarzt.de/magazin/mb-monitor-2024/)).
- **Counter-evidence [B]:** DBfK 2026 finds satisfaction with "Arbeitszeiten und Dienstplangestaltung … konstant recht hoch". The problems are workload and appreciation ([DBfK](https://www.dbfk.de/media/docs/newsroom/pressemitteilungen/2026/Pflege-wie-geht-es-dir-2026.pdf)).
- **[C] Thread titles (bodies not opened unless stated):** "Nachtdienst alleine für 49 Bewohner – wie geht ihr damit um?" (Feb 2026); "Vertretungsdienst ohne Zustimmung" (Feb 2025, 16 replies); "5 Jahre Gehaltsstillstand: Wenn der erfahrene Mitarbeiter weniger wert ist als die Leasingkraft" (Jan 2026); "Überlastung, Teamchaos und fehlende Einarbeitung" (Feb 2026, opened) ([krankenschwester.de](https://www.krankenschwester.de/forum/subforen/arbeitsrecht-gesundheitsrecht-krankenpflegegesetz.26/)).
- *Inference:* rostering software is a mature, tendered category with incumbents. Staff shortage cannot be solved by software alone.

### S8 Discharge and transition coordination (staff side)
- **[B]** RWI study (insurer data 2011–2019, published Nov 2024): patients needing a care-home place stay "drei bis vier zusätzliche Tage" in hospital (+~40 % length of stay), about €400 extra billed per patient, and bed blocking. Patients with higher care grades wait longest ([idw/RWI](https://idw-online.de/de/news843152); [Ärzteblatt](https://www.aerzteblatt.de/nachrichten/155841/Mangel-an-Pflegeheimplaetzen-laesst-auch-Klinikkosten-steigen)). **Data period >3 years old.**
- **[A] Purchasing:**
  - Helios: framework for "eine zentrale Entlassmanagement-Plattform für die Standorte der Helios-Kliniken" ([TED 24618-2025](https://api.ted.europa.eu/v3/notices/search)).
  - Also UK Dresden, UK Magdeburg (cloud discharge/transition platform, 2026), Lahn-Dill-Kliniken and MUL Lausitz.
- *Inference:* this overlaps with A3 P2/P7. Hospitals pay because of bed blocking. Competitors exist (e.g. Recare, named in a snippet `[UNVERIFIED]`).

### S9 Leadership, communication, retention (kununu)
kununu employer pages, 2026-11-06. "Personalmangel" etc. refers to the kununu AI-summary text I read (first ~6 paragraphs). [C], machine-written. **Caveat:** "—" means the summary does not mention the topic. The summaries are short and machine-written, so "—" is not evidence that staff do not complain about it. Leadership is criticised in 8 of 9 (Charité mixed).

| Employer | Reviews | Score | Staff shortage named | Rostering named | Leadership/communication criticised | Documentation/IT named |
|---|---|---|---|---|---|---|
| Helios Kliniken | 2,855 | 3.1 (sector avg 3.6) | yes | — | yes | — |
| Asklepios Kliniken | 2,688 | 3.4 | yes | — | yes | — |
| Sana Kliniken | 1,272 | 3.6 | yes | — | yes | — |
| AMEOS Gruppe | 905 | 2.9 | yes | yes ("willkürliche Dienstplanänderungen") | yes | — |
| Charité | 782 | 3.9 | — | — | mixed | — ("ticketbasierte Kommunikation") |
| München Klinik | 314 | 3.2 | staff cuts | yes ("unflexibles Schichtsystem") | yes | — |
| Alloheim Gruppe | 2,351 | 2.9 | yes | — | yes | — |
| Kursana | 705 | 3.4 | yes | — | yes | — |
| Victor's Group | 1,296 | 3.2 | yes | — | yes | — |

Sources: `https://www.kununu.com/de/<slug>/kommentare?automated=summary` for helios-kliniken, asklepios-kliniken, sana-kliniken, ameos, charite-universitaetsmedizin-berlin, muenchen-klinik, alloheim-senioren-residenzen, kursana, pro-seniore (→ Victor's Group). The Korian summary did not parse. Schön Klinik, Vivantes and LMU Klinikum slugs returned 404.
- **[B]** MB-Monitor: 28 % consider leaving patient care (25 % in 2022); part-time share 36 % (15 % in 2013) ([zm-online](https://www.zm-online.de/news/detail/viele-aerztinnen-und-aerzte-gehen-ueber-ihre-grenzen-hinaus)).
- **[C]** A junior surgeon: "mindestens 12 Stunden am Tag", 24-h shifts lasting "28 bis 30h" ([medi-learn, Feb 2024](https://forum.medi-learn.de/t/albtraum-chirurgie-uniklinik/98586)). Unrecorded overtime: "Überstunden werden im ersten halben Jahr nicht aufgeschrieben" ([medi-learn, Nov 2022](https://forum.medi-learn.de/t/der-tausendste-thread-zu-ueberstunden/96970)).
- *Inference:* the largest staff pain in employee reviews is management quality, which a software startup cannot fix. Do not let documentation tools borrow this pain as evidence.

### S10 Onboarding foreign-trained staff
- **[A]** Destatis: 32,000 recognitions of nursing qualifications in 2025, the most common recognised profession. Physicians: 13,900. Bavarian state-law data for 2024–25 are substituted with 2023 values ([Destatis, Aug 2026](https://www.destatis.de/DE/Presse/Pressemitteilungen/2026/08/PD26_295_212.html)).
- **[B]** Nursing employment vs June 2024: −5,000 German nationals, +46,000 foreign nationals ([BA, 2026](https://www.arbeitsagentur.de/presse/2026-32-fachkraefte-bleiben-knapp-zuwanderung-gewinnt-weiter-an-bedeutung)).
- `[UNVERIFIED]` Processing times and recruiter fees: not found.

### Tender access check (A14)
Eligibility read from the TED v3 field `selection-criterion-description-lot` on 2026-11-07 [A] ([TED API](https://api.ted.europa.eu/v3/notices/search)). One notice per buyer, except Charité (two notices). "Accessible?" is my judgement for a newly founded company with no revenue and no references (inference).

| Item | Tender (TED) | Buyer | Key eligibility (quoted or paraphrased) | Accessible to a startup? |
|---|---|---|---|---|
| S3 | 186365-2025 / 213191-2026 | Charité | 3 references on primary coding in German hospitals; "Mind. zwei … deutsches Universitätsklinikum", one "Maximalversorger"; 2026: each ≥500 codings | **No** |
| S3 | 214386-2026 | MUL Lausitz | In-field turnover "pro Jahr mind. 1.000.000 EUR"; solution live "in mindestens drei Universitätsklinika oder Maximalversorgern" with Dräger PDMS and ORBIS interfaces; ≥50 staff; ISO 9001 | **No** |
| S1 | 492877-2025 | Harzklinikum | ≥1 reference of full implementation "in einer deutschen Klinik"; CDSS scope (MDR) | **No** |
| S1 | 18610-2025 | BG Klinikum Hamburg | ≥6 references, incl. ≥300 licences in healthcare and 5 cloud references (Nuance update) | **No** |
| S1 | 198989-2025 | Rems-Murr-Kliniken | "Mindestens 3 Referenzen … im Wert von min. 500.000 €"; liability €5m | **No** |
| S1 | 508395-2025 | UK Saarland | "Es ist kein Mindestumsatz erforderlich"; 2 productive references (≥2 of: university/max-care site, ≥100 active users, …); ISO 27001; C5 attestation for cloud | **Hard** (needs 2 live hospital references) |
| S1 | 676942-2025 | KKH Emmendingen | Turnover with comparable work ≥€300,000 in the last 3 years; 3 references, one on iMedOne; ISO 27001 | **No** |
| S1 | 766808-2025 | Vivantes | In-field turnover "mindestens EUR 1.000.000,00 je Jahr"; 3 hospital speech-recognition references, 2 with ORBIS | **No** |
| S1 | 143223-2025, 297132-2025, 545790-2026 | Mittweida, Dietrich-Bonhoeffer, KRH Hannover | Turnover and reference declarations; thresholds not in TED fields | Unknown |
| S7 | 839796-2025 | Klinikverbund Südwest | 5 references (≥600 beds, ≥2,500 users, cloud); comparable turnover "10 Mio. € netto" in 2024 | **No** |
| S7 | 429035-2026 | Pfalzklinikum | 3 references from health-sector operators with ≥500 FTE | **No** |
| S7 | 726622-2025 | Klinikum Chemnitz | ≥3 comparable reference projects (reference clients of a stated minimum staff size); ISO 27001 or equivalent | **No** |
| S7 | 486151-2025, 549966-2025 | UK Münster, Bremerhaven | Turnover and reference declarations; thresholds in documents | Unknown |
| S8 | 24618-2025 | Helios | "KHZG-Zertifikat des [BAS]"; reference from a hospital group "über mindestens 2.000 Betten"; KIS references (CGM Medico, ORBIS, i.s.h.med, iMedOne) | **No** |
| S8 | 139657-2025 | UK Dresden | "Mindestumsatz in Höhe von EUR 500.000,00" a year in comparable work; ≥3 reference hospitals in DE | **No** |
| S8 | 451599-2026 | UK Magdeburg | ≥3 references in 3 years, ≥2 at hospitals with ≥300 beds; ISO 27001 scored | **No** |

*Inference:* none of the hospital tenders used as WTP evidence in S1, S3, S7 or S8 is open to a company without live hospital references; UK Saarland (no turnover minimum) is the softest. These tenders prove buyer budgets, not startup access. Realistic first sales: below-threshold purchases (Bavaria direct award ≤€100k net, see `research/reviews/2026-11-07-redteam-scoring.md`), private hospital groups that buy outside TED, or co-selling with a KIS vendor. Thresholds for the "Unknown" rows sit in tender documents that were not read.

### Payment context relevant to all items (for A7/A9)
- **[A] KHZG penalty (§ 5 Abs. 3h KHEntgG):** up to 2 % per inpatient case if digital services (FTB 2–6) are not provided. The weight of *use* rises from 0 % (2025–26) to 20 % (2027), 40 % (2028), 50 % (2029), 60 % (2030) and 80 % (2031). The usage threshold rises from >60 % to >80 % ([agreement, 20 Aug 2024](https://gkv-spitzenverband.de/media/dokumente/krankenversicherung_1/krankenhaeuser/abrechnung/zu___abschlaege/digitalisierung/DigitalisierungsabschlagsVb_mit_Anhaengen_1-4_20.08.2024.pdf)). *Inference:* this creates demand for adoption and usage of tools already bought, not only for new purchases.
- **[B] Counter:** DKG wants the penalty abolished. The hospital digital maturity score rose from 33.3 (2021) to 55.0 (2026), but operating costs remain unfunded ([DKG, 17 Jun 2026](https://www.dkgev.de/fileadmin/Mediapool/1_DKG/1.7_Presse/1.7.1_Pressemitteilungen/2026/2026-06-17_PM_DKG_zum_Digitalradar.pdf)).
- **[A] Pflegebudget (§ 6a KHEntgG, BStabG version):**
  - A flat 2.5 % uplift for nurse-relief measures (2025, no proof required).
  - The 2027 base is reduced by 86 % of that amount; half the remaining amount is removed in 2028 and all of it in 2029.
  - Admin, logistics and technical tasks are excluded from the Pflegebudget ([buzer.de](https://www.buzer.de/6a_KHEntgG.htm)).

## Gaps / [UNVERIFIED]
- **[C] base is thin.** Reddit not used. krankenschwester.de and medi-learn are low-traffic: 3 + 5 threads opened, the rest titles only. kununu is limited to AI summaries; page 2+ require sign-up (not bypassed). Facebook nursing groups and DocCheck community are login-walled.
- Not reachable or not tried this run: facharzt.de, pflegeboard.de, altenpflegeforum.de (blocked per A2); Capterra DE reviews of KIS/PVS/care software not pulled (next step for competitor weaknesses).
- **Job ads:** LinkedIn counts are unreliable (fuzzy matching: "Kodierfachkraft 4,000+"). StepStone shows no counts. Not used as evidence.
- **MD audit volumes, repayment sums, 2027 rules and coding/CDI incumbents:** now covered by A11 (`research/hospital-billing-audits.md`); the snippet-only claims were corrected in S3.
- **Tender documents not read:** thresholds for the "Unknown" rows in the tender access table. Below-threshold hospital purchases are invisible in TED.
- **MDR qualification of an AI discharge-letter tool:** the Rule 11 / MDCG reading in S1 is my application of the guidance to one tender text; a regulatory expert or notified body would have to confirm it for a concrete product.
- **MB-Monitor "3 h/day admin":** snippet only. VmF (MFA association) 2025 survey: not found. Zi practice-panel admin hours: only older data (snippet).
- **§ 8 Abs. 8 SGB XI subsidy uptake:** not found (also open in A10).
- **Stale (>3 years):** Fraunhofer IML survey data (2021), RWI data period (2011–2019), 2016 Bureaucracy Index.
- **Bias:** DKI/DKG, KBV and DBfK are interest groups. Their self-estimates (3 h/day) exceed the one measured German study (93 min/day). Treat 3 h as an upper-end figure.

## Sources
All accessed 2026-11-06 via curl unless noted.
- https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf — DKI 2025: hours, FTE equivalents, top burdens, hiring [B]
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38977000%20AND%20SRC:MED&format=json&resultType=core — DMW 2024 time-motion study [A]
- https://dkgev.de/fileadmin/default/Mediapool/1_DKG/1.7_Presse/07_Landespflegekammer_Umfrage_Entbuerokratiesierung.pdf — nursing chamber survey Aug 2024 [B]
- https://www.zm-online.de/news/detail/viele-aerztinnen-und-aerzte-gehen-ueber-ihre-grenzen-hinaus — MB-Monitor 2024 key figures [B]
- https://www.praktischarzt.de/magazin/mb-monitor-2024/ — MB-Monitor 2024: IT dissatisfaction, staffing, post cuts [B]
- https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2025/10-16/praxisbarometer-2025-niedergelassene-bleiben-vorreiter-in-sachen-digitalisierung — PraxisBarometer 2025 [B]
- https://www.kbv.de/presse/pressemitteilungen/2025/entbuerokratisierung-entlastet-praxen-und-kostentraeger-formfreie-anfragen-heut-zettelwust-morgen-digital — >2m hours of free-form requests [B]
- https://www.kbv.de/praxis/tools-und-services/praxisnachrichten/2026/08-20/kbv-unterstuetzt-massnahmen-des-bmg-zum-buerokratieabbau-und-fordert-weitere-entlastungen — 23 proposals, €400m, 8 days/practice [B]
- https://www.aerzteblatt.de/news/niedergelassene-aerzte-wenden-52-millionen-stunden-fuer-buerokratie-auf-3bccf9be-2a59-4087-b2db-15e97d46e935 — 2016 Bureaucracy Index (stale) [B]
- https://www.aerzteblatt.de/themen/medizinische-fachangestellte/jeder-zweiten-hno-praxis-fehlt-personal-ca8e3832-4066-4283-873c-61c700aca121 — ENT practices MFA shortage, Jul 2024 [B]
- https://www.aerzteblatt.de/themen/praxismanagement/diskussion-um-ki-assistenten-in-arztpraxen-13b8abd7-946e-42f5-ae09-235973e167e3 — AI phone assistants debate, Aug 2025 [B]
- https://medizinio.de/digitalisierung/telefonassistent-arztpraxis — 10 phone-assistant vendors, prices [B, vendor-adjacent]
- https://www.arbeitsagentur.de/presse/2026-32-fachkraefte-bleiben-knapp-zuwanderung-gewinnt-weiter-an-bedeutung — BA shortage analysis 2025 [B]
- https://dserver.bundestag.de/btd/21/052/2105270.pdf — agency nursing 2020–2025 [A]
- https://www.buzer.de/6a_KHEntgG.htm — § 6a KHEntgG consolidated (BStabG, 24 Jul 2026) [A]
- https://gkv-spitzenverband.de/media/dokumente/krankenversicherung_1/krankenhaeuser/abrechnung/zu___abschlaege/digitalisierung/DigitalisierungsabschlagsVb_mit_Anhaengen_1-4_20.08.2024.pdf — KHZG penalty schedule 2025–2031 [A]
- https://www.dkgev.de/fileadmin/Mediapool/1_DKG/1.7_Presse/1.7.1_Pressemitteilungen/2026/2026-06-17_PM_DKG_zum_Digitalradar.pdf — DigitalRadar 2026, DKG position [B]
- https://www.gkv-spitzenverband.de/krankenversicherung/krankenhaeuser/krankenhaeuser_abrechnung/kh_pruefung_statistik/pruefquoten_und_statistik.jsp — audit-quota regime and statistics page [A]
- https://www.dbfk.de/media/docs/newsroom/pressemitteilungen/2026/Pflege-wie-geht-es-dir-2026.pdf — DBfK survey 2026 [B]
- https://www.iml.fraunhofer.de/content/dam/iml/presse/whitepaper/32_Whitepaper_Pflegedokumentation_in_Krankenh%C3%A4usern.pdf — care-home documentation 52 vs 109 min (2021 data) [B]
- https://www.bundesgesundheitsministerium.de/presse/pressemitteilungen/befugniserweiterungsgesetz-bundestag-06-11-25.html — BEEP law content [A]
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41950503%20AND%20SRC:MED&format=json&resultType=core — voize LTC time-motion study [A]
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=DOI:%2210.1001/jama.2026.2253%22&format=json&resultType=core — JAMA 2026 AI-scribe cohort [A]
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41729180%20AND%20SRC:MED&format=json&resultType=core — JAMIA 2026 ambient-scribe crossover RCT [A]
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41041759%20AND%20SRC:MED&format=json&resultType=core — ScanProCare! smart workflows [A]
- https://www.aerzteblatt.de/themen/kuenstliche-intelligenz/ki-schreibassistenzen-verschaffen-mehr-zeit-bei-der-dokumentation-fd883789-1b3d-4c8f-bd66-5f167ea72890 — Ärzteblatt on JAMA scribe study, 7 Apr 2026 [B]
- https://www.healthcapital.de/news/artikel/berlins-voize-raises-50m-for-nursing-ai — voize Series A, 1,100 facilities [B]
- https://idw-online.de/de/news843152 — RWI: care-home shortage extends hospital stays [B]
- https://www.aerzteblatt.de/nachrichten/155841/Mangel-an-Pflegeheimplaetzen-laesst-auch-Klinikkosten-steigen — same, 19 Nov 2024 [B]
- https://www.destatis.de/DE/Presse/Pressemitteilungen/2026/08/PD26_295_212.html — recognitions of foreign qualifications 2025 [A]
- https://api.ted.europa.eu/v3/notices/search — selection criteria (`selection-criterion-description-lot`) of 186365-2025, 213191-2026, 214386-2026, 492877-2025 (incl. `description-lot`), 24618-2025, 18610-2025, 143223-2025, 198989-2025, 297132-2025, 508395-2025, 676942-2025, 766808-2025, 545790-2026, 139657-2025, 451599-2026, 486151-2025, 549966-2025, 726622-2025, 839796-2025, 429035-2026 [A], accessed 2026-11-07
- https://api.ted.europa.eu/v3/notices/search — TED contract notices (cn-standard, DEU, since 2025-01-01): title~Spracherkennung (21 notices), Patientenportal (38), Entlass (6), Zeitwirtschaft (8), Kodier (2); FT queries Dienstplan, Kodierung, künstliche Intelligenz with hospital terms; notice details 492877-2025, 186365-2025, 214386-2026, 24618-2025 [A]
- https://www.kununu.com/de/{helios-kliniken,asklepios-kliniken,sana-kliniken,ameos,charite-universitaetsmedizin-berlin,muenchen-klinik,alloheim-senioren-residenzen,kursana,pro-seniore}/kommentare?automated=summary — scores, review counts, AI summaries [C]
- https://www.krankenschwester.de/forum/ — subforums 64, 61, 86, 54, 26 (title scan); threads 150717, 151070, 151008 opened [C]
- https://forum.medi-learn.de/ (Discourse JSON: search.json; threads 99622, 99844, 98837, 98586, 96970 opened) [C]
- https://www.linkedin.com/jobs/search?keywords=Kodierfachkraft&location=Germany (and 10 other roles) — counts judged unreliable, not used [—]
- WebSearch, snippet only (not opened, not used as fact): MB-Monitor 3 h admin; VmF surveys; Zi practice-panel hours; MFA shortage score; ambulant care bureaucracy surveys; §8(8) SGB XI uptake; KHVVG audit reform and BStabG audit-quota draft; Recare/myScribe/Doctolib scribe; DBfK 2016 roster survey.
- https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32017R0745 — MDR Annex VIII Rule 11 (decision-support software class IIa+) [A], accessed 2026-11-07
- https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=md_mdcg_2019_11_guidance_qualification_classification_software_en.pdf — MDCG 2019-11 rev. 1 (Jun 2025): decision-support software qualifies as MDSW; information systems do not [A], accessed 2026-11-07
- https://www.gesetze-im-internet.de/khg/__14a.html — KHZG fund €3bn, applications by 31 Dec 2021 [A], accessed 2026-11-07
- https://www.sozialpolitik-aktuell.de/files/sozialpolitik-aktuell/_Politikfelder/Gesundheitswesen/Datensammlung/PDF-Dateien/abbVI54_55.pdf — staff in home-care services (446,425) and residential care (817,711), 2023, Destatis data [B], accessed 2026-11-07
- https://www.pharmazeutische-zeitung.de/mehr-aerzte-aber-weniger-zeit-fuer-patienten-163553/ — 191,875 physicians/psychotherapists in contract practice end-2025 (KBV data) [B], accessed 2026-11-07
- https://www.ebi.ac.uk/europepmc/webservices/rest/PMC13061367/fullTextXML — voize study conflicts of interest and funding [A], accessed 2026-11-07
- `research/hospital-billing-audits.md` (A11) — 2027 audit rules, incumbents, UK Frankfurt ticket size (internal cross-reference)
