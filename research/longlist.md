# Long list: 30 healthcare problems (DE/DACH first)
Task: A7 | Date: 2026-11-07 | Status: draft

Method: merged the 36 raw problems in `research/pain-patients.md` (P1–P11), `research/pain-professionals.md` (S1–S10), `research/pain-industry.md` (I1–I10) and `archive/cancer-problem-statement.md` (A–E), using the deep dives `research/hospital-billing-audits.md` (A11), `research/payer-processing.md` (A12), `research/trial-recruitment-de.md` (A13), `research/reimbursement-routes.md` (A9/A15) and `research/trends.md` (A1). Result: 30 problems (one new: L10) and 6 items excluded or merged (table below). Key facts from the earlier files are carried over with their sources and grades, and were not re-opened in A7. Sources marked **(A7)** were opened in this session. Scoring fields (signer, budget line, wedge, first-sale route, buyer count) come in A18; scores come in B1.

## Findings
- **All 30 problems meet the Stage A bar**: each has ≥2 independent evidence items and ≥1 graded [A]/[B] (L19: 1 [B] + 3 opened [C] app feeds; L18, L24, L25, L30 and L11 have exactly 2). The [C] layer (online voices) is thin for most rows, because Reddit and several caregiver forums are blocked (A2). Only L01, L05, L06, L09, L16, L19, L20 and L21 have ≥2 opened [C] signals. Pain intensity therefore rests mostly on [A]/[B] surveys and statistics.
- **Proven spend exists in 15 rows, but direct startup access is rare.** Of the 34 tender notices checked in A14, only one (MD Rheinland-Pfalz AI PoC) is open to a new company. Hospital, insurer and MD tenders ask for €250k–€10m turnover, university-hospital/GKV references or ISO/C5 certificates [A] (TED, see `pain-industry.md` and `pain-professionals.md` "Tender access check"). *Inference:* A18 must find a direct-award, private-buyer or channel route for each row, or the row fails knock-out K2.
- **The strongest rows combine a dated rule change, a budget and founder fit** (inference, for B1 to test):
  - L07/L22: hospital billing audits. Stricter quotas start 1 Jan 2027 (enacted). MD-IT has an €88m AI framework (startups only as subcontractor or consortium member). Incumbents: Tiplu/LOGEX and calliora (Munich).
  - L26: trial recruitment. Sponsors pay. From 2027, ≥5 % of trial participants at German sites can earn an exemption from the 8.5 % extra discount. But sites name staff, not patient finding, as their main hurdle, and vendors have consolidated.
  - L05: long-term-care documentation. PNOG fund from H2 2027 (bill). § 113e money from 2028 (bill). voize ($50m) leads.
- **Patient- and family-side problems are the largest by headcount, but the payer is weakest.** This covers L01–L04 and L14–L19. Statutory budgets exist (relief budget, screening benefits), but payers are in a €15bn deficit year (2027), and DiPA cannot pay for navigation-only apps [A] (`reimbursement-routes.md`). Of 31 Innovation Fund navigator projects, "In most cases, no effect was observed" [A] ([PMID 41419645](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41419645%20AND%20SRC:MED&format=json&resultType=core)).
- **New German data added in A7:**
  - Colorectal screening: participation was 7.75 % (averaged over stool test and colonoscopy), against an EU minimum of 45 %. Documented follow-up after a positive stool test was only 12.9 % (target 85 %; a lower bound because of documentation gaps) [A] ([G-BA evaluation report, 16 Mar 2026](https://www.g-ba.de/downloads/17-98-6102/2026-03-16_oKFE-Evaluationsbericht-Darmkrebs_GFL_2021-2024.pdf)).
  - Pharmacies spend on average 20.1 h/week managing drug shortages [B] ([ABDA ZDF 2026](https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_55_56_57_Management_von_Lieferengpaessen.pdf)).
  - Hybrid DRGs (§ 115f SGB V) are to be deleted and replaced by short-stay flat rates in 2028 [A] ([BT-Drs. 21/8629](https://dserver.bundestag.de/btd/21/086/2108629.pdf)).
  - Live-in care: 100,000–210,000 carers on any given day [A] ([BMG report, Nov 2024](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/5_Publikationen/Pflege/Berichte/241127_Abschlussbericht_Live_Ins_bf.pdf)).

## Long list
Legend:
- **Who pays (status):** *proven* = tender, contract, price list or observed purchase; *budget* = statutory benefit or budget line exists, purchase not observed; *plausible* = inference; *unclear* = no payer found.
- **Evidence:** number of independent [A]/[B] items (of which [A]) / opened [C] signals.
- **Source rows:** IDs in the A3–A5 files and the cancer file.

| # | Problem (one line) | Who has it | Who pays (status) | Evidence [A/B] ([A]) / [C] | Source rows → files |
|---|---|---|---|---|---|
| **Long-term care and families** ||||||
| L01 | Families cannot navigate home-care benefits (care grade, relief budget, respite care), so entitlements go unused | ~4.9m people cared for at home + family carers | Pflegekassen (*budget*: €131/month relief budget, § 7a counselling); families; DiPA excludes navigation-only apps | 8 (4) / 4 | P1 → `pain-patients.md`, `reimbursement-routes.md` |
| L02 | Families cannot find care capacity (home-care service, short-term/day care, care-home place) | Same + hospital discharge cases | Families (*proven* self-pay €3,364/month in care homes); Pflegekassen | 6 (1) / 0 | P2 → `pain-patients.md`, `trends.md` |
| L03 | Family carers are overloaded and cut working hours | Families of 3.1m care recipients cared for mainly by relatives | *Unclear*: employers (inference), Pflegekassen | 4 (1) / 0 (18 titles) | P3 → `pain-patients.md` |
| L04 | 24-h live-in care runs in a legal grey zone with no reliable data | Households of high-need elderly; 100k–210k live-in carers | Families (*proven* self-pay €2,800–3,500/month + agency fees) | 3 (1) / 0 | P11 → this file (A7) |
| L05 | Documentation and admin load in long-term and home care; care homes lag on digital tools and the TI | 446,425 home-care + 817,711 care-home staff; ~32,000 facilities | Operators (*proven*: voize 1,100 facilities; § 8 Abs. 8 grant €143.3m paid 2019–24); PNOG fund 2027+ and § 113e 2028+ (*bills*) | 7 (5) / 2 | S2 → `pain-professionals.md`, `reimbursement-routes.md`, `trends.md` |
| **Hospitals** ||||||
| L06 | Physicians and nurses spend hours a day on clinical documentation (letters, ward notes) | ~176,800 physician FTE, ~391,000 nursing FTE | Hospitals (*proven*: 8 speech-recognition buyers, KHZG one-off money) | 6 (3) / 2 | S1 → `pain-professionals.md` |
| L07 | Hospitals lose revenue in MD billing audits; quotas rise to up to 40 % from 2027 | 1,603 hospital IKs; medical controlling, coders | Hospitals (*proven*: Charité/Lausitz tenders; DKI: mean €236k/yr audit staff, median €40k planned non-staff spend) | ≥8 (≥5) / 1 | S3 → `hospital-billing-audits.md`, `pain-professionals.md` |
| L08 | Discharge and transitions fail: follow-up care not found, medication lists missing, bed blocking | 17.7m inpatients (2025), older polypharmacy patients; social services | Hospitals (*proven*: Helios framework + 4 other buyers, KHZG FTB2); Kassen (pilots only) | 7 (4) / 1 | P7 + S8 → `pain-patients.md`, `pain-professionals.md` |
| L09 | Staff shortage forces short-notice cover; agency premiums no longer refinanced | Ward managers, nurses, physicians | Hospitals/operators (*proven*: ≥10 rostering-software buyers) | 6 (3) / 9 kununu | S7 → `pain-professionals.md` |
| L10 | Rules for outpatient-capable procedures keep changing (Hybrid DRG 2024–27, short-stay flat rates 2028), and hospitals and practices must rebuild billing and processes each year | Hospitals, surgical practices; ~1m hybrid-DRG cases in 2026 | Hospitals/practices (*plausible*: grouper and billing software is mandatory; no purchase observed in A7) | 5 (2) / 0 | **New (A7)** → this file |
| L11 | Onboarding foreign-trained nurses and physicians is slow (recognition, language) | Hospitals, care operators | Employers (*plausible*; recruiter fees `[UNVERIFIED]`) | 2 (1) / 0 | S10 → `pain-professionals.md` |
| **Practices and access** ||||||
| L12 | Practices drown in free-form payer and agency requests and forms | 191,875 contract physicians/psychotherapists | Practices (price-sensitive); insurers/MD co-own the problem (*plausible*) | 3 (0) / 1 | S4 → `pain-professionals.md` |
| L13 | Phones and reception are overloaded; medical assistants (MFA) are scarce | Practices, MFAs | Practices (*proven*: AI phone tools at €9–229/month) | 4 (0) / 0 | S5 → `pain-professionals.md` |
| L14 | Patients wait weeks for specialist appointments; booking and steering are fragmented | GKV insured; worst for those in poor health | KVs (116117), Kassen (*budget*: €2.9bn TSVG fees); patients use free apps | 5 (1) / 1 app feed | P4 → `pain-patients.md`, `trends.md` |
| L15 | Psychotherapy waiting times are long (contested size) | People with mental illness, children | GKV, self-pay (*unclear* volume) | 3 (0) / 0 | P5 → `pain-patients.md` |
| **Patients: specific conditions and services** ||||||
| L16 | Cancer patients lack orientation and coordination between diagnostic and treatment steps | 566,587 new cancer cases/yr in DE (GLOBOCAN 2024) + relatives | Kassen (*proven* in-house: BARMER navigator programmes); hospitals (inference) | 3 (2) / 5 | P8 + cancer E → `pain-patients.md`, `archive/cancer-problem-statement.md`, this file |
| L17 | Few eligible people take up cancer screening, and follow-up of positive results is poorly documented | Insured ≥50 (colorectal); ~5.5m current/ex-smokers (lung, since Apr 2026) | GKV (*budget*: statutory screening benefits; Kassen send the invitations) | 4 (2) / 0 | cancer A + B (US data) → replaced with DE data in this file (A7) |
| L18 | Rare-disease patients wait years for a diagnosis | ~4m people in DE | GKV (rare-disease centres, genome sequencing pilot); pharma (patient finding, inference) | 2 (2) / 0 (2 titles) | P9 → `pain-patients.md`, this file |
| L19 | Insurer ePA/ident apps frustrate users at login and identification | ~73m with an ePA, ~8 % active | Kassen and their IT vendors (*plausible*); identity rules set by gematik/BSI | 1 (0) / 3 app feeds | P10 → `pain-patients.md`, `trends.md` |
| L20 | Drug shortages harm chronic patients and cost pharmacies ~20 h/week | Chronic patients; 16,601 pharmacies | Pharmacies (*plausible*), wholesalers, manufacturers | 5 (0) / 2 | P6 → `pain-patients.md`, this file |
| **Payers and the MD** ||||||
| L21 | Insurers process §302 invoices from other providers largely on paper and outsource them | 92 statutory insurers' claims departments | Insurers (*proven*: 9 buyers, 13 awards to incumbents; admin cap from 2027) | 8 (6) / 3 kununu | I5 → `payer-processing.md`, `pain-industry.md` |
| L22 | MDs and insurers cannot handle the 2027 hospital-audit volume with current processes | 15 MDs (2,148 physician FTE), insurer hospital-bill teams | MD-IT (*proven*: €88m AI framework, bids due 2 Dec 2026); TK (*proven*: QuantCo DRG scoring) | 6 (5) / 0 | I6 (part) → `payer-processing.md`, `hospital-billing-audits.md` |
| L23 | MD care-need assessments have doubled in volume (>3m in 2025) | 15 MDs; applicants waiting | MDs, financed by insurers (*proven*: MD RLP AI PoC, open to startups; MD Nordrhein) | 6 (5) / 1 kununu | I6 (part) → `pain-industry.md`, `payer-processing.md` |
| L24 | Private insurers check >70m invoices a year, and a new fee schedule (GOÄ) is planned for 2028 | PKV claims teams | Private insurers (*plausible*, no tenders) | 2 (0) / 0 | I7 → `pain-industry.md` |
| L25 | Public-health offices must keep digital projects running after federal pact money ends in 2026 | ~375 local health offices `[UNVERIFIED]` count | Länder/municipalities (*budget falling*) | 2 (0) / 0 | I9 → `pain-industry.md` |
| **Pharma, clinical research, medtech** ||||||
| L26 | German trial sites miss recruitment targets; Germany's share of trial participants is ~2.9 % | Sponsors, CROs, site staff; patients without trial access | Sponsors/CROs (*proven*: sites are paid for patient identification; MPIRIQ €99–329/month; vendor market) | ≥12 (≥6) / weak | I1 + cancer C → `trial-recruitment-de.md`, `pain-industry.md` |
| L27 | Trial-site start-up is slow: contracts, budgets, CTIS documents, system training | Study nurses, investigators, CRO start-up teams | Sponsors/CROs; sites (overhead) (*plausible*) | 5 (2) / 1 | I2 → `pain-industry.md` |
| L28 | EU joint clinical assessments (JCA) and AMNOG dossiers need many PICOs under tight deadlines | Pharma market-access teams, small biotechs | Pharma (*proven*: consultancies and CROs sell JCA services) | 4 (1) / 0 | I3 → `pain-industry.md` |
| L29 | MDR/IVDR certification takes ~20 months and costs SMEs R&D projects | Device and IVD makers (mostly SMEs) | Manufacturers (*proven*: consultants, staff) | 5 (1) / 0 | I4 → `pain-industry.md` |
| L30 | Real-world-data access via the FDZ Gesundheit is new and hard to use (claims data only so far) | Pharma RWE teams, researchers | Pharma, academia (*plausible*) | 2 (1) / 0 | I8 → `pain-industry.md` |

## Excluded or merged (not on the list)
| Raw item | Decision | Reason |
|---|---|---|
| S6 TI outages, PVS lock-in | Excluded | High pain, but infrastructure owned by gematik and practice-software vendors; a startup cannot fix it from outside (`pain-professionals.md` S6) |
| S9 Leadership, communication, retention | Excluded | Not a product problem (kununu summaries: 8 of 9 employers criticised on leadership) |
| I10 Pharmacovigilance | Excluded | Only 1 [A] item; flat volume (+0.5 % in 2025) and mature vendors |
| Cancer D (financial toxicity, 48 %) | Excluded | US data, `[UNVERIFIED]`; no DE evidence found |
| Cancer A/B (US lung and colorectal screening) | Replaced by L17 | US data replaced with German G-BA programme data (A7) |
| Cancer C (trial enrolment 7.1 %), Cancer E (time to treatment) | Merged into L26 and L16 | Same problem with German evidence; the US figures stay `[UNVERIFIED]` |
| P7 + S8 (discharge, patient and staff side) | Merged into L08 | Same process, same buyer (hospital) |
| I6 (MD workload) | Split into L22 (hospital audits) and L23 (care assessments) | Different budget, buyer unit and tender (MD-IT framework vs MD regional PoCs) |

## Details: evidence per problem
Grades as in the source files. "→" = file with full sources.

**L01 Home-care benefit navigation**
- Only "3 Prozent der Anspruchsberechtigten" use statutory care counselling [A] ([GKV-SV § 7a report, Jun 2026](https://www.gkv-spitzenverband.de/media/dokumente/pflegeversicherung/beratung_und_betreuung/pflegeberatung/2026-06_Bericht_des_GKV-Spitzenverbandes_7a_Absatz_9_SGB_XI.pdf)).
- 38.4 % of Pflegegeld recipients used the relief budget (2022) [B] ([AOK G+G](https://www.aok.de/pp/gg/magazine/gesundheit-gesellschaft-07-2024/pflegebetrag/)).
- Counter-evidence: the main reasons for non-use are "fehlender Bedarf" and preference [B] ([WIdO 2026](https://www.wido.de/fileadmin/user_upload/20260511_WIdO-PM_WIdOmonitor_Pflegende_Angehoerige.pdf)).
- DiPA excludes navigation-only apps [A] ([§ 40a SGB XI](https://www.gesetze-im-internet.de/sgb_11/__40a.html)).
- → `pain-patients.md` P1.

**L02 Care capacity**
- 91 % of 150 home-care services turned away new clients [B] (DEVAP, Jan 2023, **>3 years old**).
- Shortfall of 280,000–690,000 carers by 2049 [A] (Destatis).
- *Inference:* the root cause is staff; software can only match supply and demand.
- → `pain-patients.md` P2, `trends.md`.

**L03 Carer overload**
- 45.2 % of part-time carers cut their hours; 46.9 % of employed carers are "hoch belastet" [B] (WIdO 2026).
- No statutory budget for carer support beyond SPV benefits.
- → `pain-patients.md` P3.

**L04 Live-in care (A7 update)**
- BMG final report (27 Nov 2024): "Zur Zahl der Haushalte mit „Live-In-Care“ in Deutschland liegen keine gesicherten Erkenntnisse vor". On any given day there are 100,000–210,000 carers, and with rotation 200,000–420,000 a year, "hohe Dunkelziffer" [A] ([BMG](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/5_Publikationen/Pflege/Berichte/241127_Abschlussbericht_Live_Ins_bf.pdf)).
- Consumer centre: "Eine 24-Stunden-Betreuung durch eine einzige Person ist legal nicht möglich". Cost is €2,800–3,500/month, plus agency fees [B] ([Verbraucherzentrale](https://www.verbraucherzentrale.de/wissen/gesundheit-pflege/pflege-zu-hause/auslaendische-betreuungskraefte-wie-geht-das-legal-10601)).
- Older estimate: 60,000–250,000 people [B] (bpb 2015, **stale**).
- *Inference:* strong private willingness to pay, but labour-law exposure for any intermediary.

**L05 Long-term-care documentation and digitisation**
- voize: −15 min documentation per morning shift [A] (JMIR 2026; first author employed by voize).
- Only 50 % of care facilities had an activated TI card by Apr 2026 [A] (Berlin Senate answer).
- The § 8 Abs. 8 grant paid €143.3m in 2019–24, ≈37 % of the pool [A] (BAS).
- PNOG fund: €1.6bn for 2027–31 (bill). § 113e: from 2028 (bill).
- → `pain-professionals.md` S2, `reimbursement-routes.md`, `trends.md`.

**L06 Hospital clinical documentation**
- DKI: physicians spend 3 h/day on documentation (self-estimate) [B]. A time-motion study measured 93.1 min/day [A].
- AI scribes save 16.0 min per 8 patient hours [A] (JAMA 2026).
- Crowded: Microsoft/Nuance, KIS vendors. Decision-support features → MDR class IIa+ [A].
- → `pain-professionals.md` S1.

**L07 Hospital billing audits**
- In 2025: 1,138,534 MD reports, 48.9 % of audited invoices reduced; ~€1.58bn revenue at risk (my math in A11) [A] (GKV-SV statistics).
- From 1 Jan 2027: quotas up to 5/20/40 %, uncapped below 50 %, €500 penalty [A] (BStabG).
- Simulation: ~1,100 of 1,603 hospital IKs land in the 40 % tier [A data, A11 math].
- Incumbents: Tiplu/LOGEX, ID Berlin, Dedalus; calliora (Munich, $6m pre-seed) [B].
- → `hospital-billing-audits.md`.

**L08 Discharge and transitions**
- Only 79 % of patients could clarify all questions about the time after discharge [B] (AOK survey 2025).
- Patients waiting for a care-home place stay 3–4 extra days [B] (RWI 2024; data 2011–19, **>3 years old**).
- Helios tendered a central discharge platform [A] (TED 24618-2025).
- → `pain-patients.md` P7, `pain-professionals.md` S8.

**L09 Staffing and rostering**
- 31,503 agency nurses (1.8 %) in Aug 2025 [A] (BT-Drs. 21/5270).
- From 2027, Pflegebudget overruns are no longer refinanced [A] (§ 6a KHEntgG).
- Counter-evidence: satisfaction with rostering is "konstant recht hoch" [B] (DBfK 2026).
- → `pain-professionals.md` S7.

**L10 Rules for outpatient-capable procedures keep changing (new, A7)**
- Volume: the 2026 catalogue grew from about 270,000 to about one million hybrid-DRG cases. The late hybrid decision held up the whole 2026 DRG catalogue [B] ([Ärzteblatt](https://www.aerzteblatt.de/themen/drg/einigung-zu-fallpauschalenkatalog-fur-2026-erzielt-9f22115a-fc3d-4f21-b187-17a7ce99a35a)).
- Spending: WIdO estimates +17 % cases and about €360m extra GKV spending in 2025. Practice cases rose 65 % (219,000 → 363,000) and hospital cases 6 % (932,000 → 986,000). WIdO expects about €640m extra in 2026 [B] ([WIdO, 10 Sep 2026](https://www.aok.de/pp/bv/wido-pm/ausgaben-hybrid-drgs/)).
- Rule change: the emergency-care reform passed by the Bundestag deletes § 115f ("§ 115f wird gestrichen"). Hybrid DRGs are replaced by short-stay flat rates (Kurzzeitfallpauschalen) in 2028. 2027 has a transition rule: cases without an overnight stay are paid fully under the EBM [A] ([BT-Drs. 21/8629](https://dserver.bundestag.de/btd/21/086/2108629.pdf)) [B] ([Ärzteblatt, 5 Oct 2026](https://www.aerzteblatt.de/news/hybrid-drg-sollen-ab-2028-abgeschafft-werden-576552aa-a75b-4b53-ad56-e51829c020d9)).
- Status: the Bundesrat sits on 20 Nov 2026; the law needs no consent (A17).
- Trend context: outpatient surgery spending +15.7 % in 2025 [A] (BMG, via `trends.md`).
- *Inference:* every year brings a new catalogue and new billing logic, which creates admin work and revenue risk. The pain is not yet shown by [C] or by purchases: no buyer or vendor was checked in A7. It overlaps with L07 (coding/billing tools) and its incumbents.

**L11 Foreign-trained staff**
- 32,000 nursing-qualification recognitions in 2025 [A] (Destatis).
- Nursing employment: +46,000 foreign nationals vs −5,000 German nationals [B] (BA).
- Process times not found.
- → `pain-professionals.md` S10.

**L12 Practice paperwork**
- Free-form requests take "mehr als zwei Millionen Arbeitsstunden" a year [B] (KBV 2025).
- The BMG adopted 3 of 23 KBV proposals [B].
- Policy may shrink the problem.
- → `pain-professionals.md` S4.

**L13 Phone and reception**
- 10 AI phone vendors at €9–229/month, including Doctolib [B].
- Crowded and low-price.
- → `pain-professionals.md` S5.

**L14 Specialist access**
- 25 % of patients wait >30 days; 30 % find getting an appointment difficult [B] (GKV-SV survey 2025).
- Average wait was 42 days in 2024 [B].
- 116117 acute-care centres (passed 15 Oct 2026) [A]; GeDIG triage + booking (draft) [B].
- → `pain-patients.md` P4, `trends.md`.

**L15 Psychotherapy waits**
- vdek: 61 % of adults wait >2 weeks after the first consultation [B].
- BPtK: 3–9 months [B, **>3 years old**].
- The two sources measure different intervals.
- → `pain-patients.md` P5.

**L16 Cancer orientation and coordination**
- 566,587 new cancer cases in Germany (2024 estimate) [A] (GLOBOCAN, `archive/cancer-problem-statement.md`).
- Navigator review: mostly no effect [A] (PMID 41419645).
- **A7:** BARMER has run a "Versorgungslotse" for breast cancer since 2021 as "reguläres Angebot". It extended it to all childhood cancers and plans prostate cancer and a "digitaler Behandlungsbegleiter" for breast cancer in its eCare app in 2026 [B] ([BARMER, Jun 2026](https://www.barmer.de/verantwortung/transparenz/transparenzbericht6/diagnose-krebs-1506416)). *Inference:* an insurer pays for navigation, but builds it in-house.
- [C]: 5 opened krebs-kompass threads.

**L17 Cancer screening uptake and follow-up (A7, DE data)**
- Colorectal (organised programme since 2019) [A] ([G-BA evaluation report 2025, 16 Mar 2026](https://www.g-ba.de/downloads/17-98-6102/2026-03-16_oKFE-Evaluationsbericht-Darmkrebs_GFL_2021-2024.pdf)):
  - Participation 7.75 % ("gemittelt über iFOBT und FEK"), against an EU minimum of 45 %. Invitations reached 89.5 % of eligible people (target 95 %).
  - Documented follow-up colonoscopy after a positive stool test: 12.9 % (target 85 %). The report calls this a minimum value because of documentation gaps.
- Ärzteblatt summary (1 Jun 2026): "Mehr als die Hälfte der Erstteilnehmenden nahm ohne zuvor dokumentierte Einladung" teil; median 336 days from invitation to test; "Weniger als 7 %" tested within 3 months [B] ([Ärzteblatt](https://www.aerzteblatt.de/news/darmkrebsfruherkennung-wirkt-nur-wenige-nehmen-teil-d8b4414f-5874-4c48-8024-eb921f42fb11)).
- Lung: low-dose CT screening has been a GKV benefit since April 2026 for people aged 50–75 with ≥25 years of heavy smoking and ≥15 pack-years. A GP checks eligibility after special training, and radiologists need KV approval [A] ([G-BA PM, 13 Mar 2026](https://www.g-ba.de/presse/pressemitteilungen-meldungen/1316/)). About 5.5m people could benefit (DGP estimate). The rollout is not yet nationwide: radiation-protection approvals were still pending at the start [B] ([AOK G+G, 31 Mar 2026](https://www.aok.de/pp/gg/update/lungenkrebsscreening-startet/)). No uptake data yet.
- *Inference:* the buyer would be the Kassen (invitation and outreach) or screening networks. Who pays for a third-party tool is `[UNVERIFIED]`.

**L18 Rare diseases**
- Average time to diagnosis is 4.7 years [A] (Rare Barometer, EJHG 2024).
- **A7:** "Rund vier Millionen Menschen in Deutschland" are affected; there are "mehr als 30 Zentren für Seltene Erkrankungen"; ~5,000 patients were in the genome-sequencing pilot by end-2025 [A] ([BMG, Feb 2026](https://www.bundesgesundheitsministerium.de/ministerium/meldungen/tag-der-seltenen-erkrankungen-2026)).

**L19 ePA onboarding**
- About 8 % of insured people actively use the ePA [B].
- Standalone ePA apps rate 1.3–2.5 stars vs 4.5–4.8 for the same insurers' main apps [C].
- → `pain-patients.md` P10.

**L20 Drug shortages (A7 update)**
- 1,514 shortage notifications in 2025 [B] (Zi).
- **A7:** pharmacies spend on average "20,1 Stunden" per week managing shortages; 66.0 % of owners rank shortages among their biggest annoyances (82.8 % in 2024). The top hurdles are consulting physicians (72.4 %), availability queries to wholesalers (68.8 %) and checking insurer rules (53.2 %) [B] ([ABDA ZDF 2026, pp. 55–56](https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_55_56_57_Management_von_Lieferengpaessen.pdf); IQVIA survey Jul/Aug 2025).
- Pharmacy count: 16,601 at end-2025 [B] ([ABDA](https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_8_Entwicklung_der_Apothekenzahl.pdf)).
- *Inference:* the pharmacy becomes the B2B buyer. No purchase was observed.

**L21 § 302 invoice processing**
- 13 awards to incumbents with 1–3 bids each; IQVIA HSS won 5 [A].
- DAK explores in-sourcing with AI software [A] (TED 427316-2025, pin-only).
- From 2027, admin spending may only grow with the per-insured income rate [A].
- → `payer-processing.md` §1–2.

**L22 Payer/MD hospital-audit work**
- MD-IT framework, Lot 1 up to €88m; the stated driver is "die gesetzlich vorgesehenen Prüfquoten". A bidder needs €5m turnover and 25 staff, but consortia and subcontracting are allowed [A].
- TK bought DRG scoring software from QuantCo [A].
- → `payer-processing.md` §3–4.

**L23 MD care-need assessments**
- More than 3m assessments in 2025 vs 1,431,000 in 2013 [A].
- MD RLP AI PoC: only 1 reference needed, no turnover minimum; 40 requests to participate [A].
- → `pain-industry.md` I6, `payer-processing.md` §3.

**L24 PKV and GOÄ**
- More than 70m invoices a year [B].
- New GOÄ "zum 1. Januar 2028 erreichbar" [B].
- → `pain-industry.md` I7.

**L25 Public health (ÖGD)**
- The €4bn pact (2021–26) ends without follow-up money [B].
- The count of ~375 health offices is `[UNVERIFIED]` (not opened).
- → `pain-industry.md` I9.

**L26 Trial recruitment**
- Germany takes part in 668 of 1,356 (49.3 %) new commercial EU trials (2025) [A, own CTIS count], but has a ~2.9 % share of trial participants [B].
- Sites rate patient identification as a big hurdle in 4–9 % of cases, and staffing/funding in 50–74 % [B].
- An EHR patient-finder showed no enrolment effect [A] (npj Digit Med 2026).
- 5 % rule → exemption from the 8.5 % discount from 2027 [A].
- → `trial-recruitment-de.md`.

**L27 Site start-up**
- Standard contract clauses apply from Dec 2025 but are not yet fully effective [B].
- CTIS document burden [A] (Trials 2024; TIRS 2026).
- → `pain-industry.md` I2.

**L28 JCA/AMNOG**
- About 58 JCAs planned in 2026; "57% of 2025 LOIs were submitted late" [B].
- Needs deep HTA expertise (founder gap).
- → `pain-industry.md` I3.

**L29 MDR/IVDR**
- Certification takes 19.5 months (QMS) and 21.8 months (technical documentation) [B].
- 53 % of DACH makers cut R&D projects [B].
- Revision proposed Dec 2025, so the pain may shrink.
- → `pain-industry.md` I4.

**L30 FDZ data access**
- Companies may apply [A] (§ 303e SGB V).
- 53 applications by Feb 2026; claims data only so far [B].
- *Inference:* an enabler for L26 rather than a pain.
- → `pain-industry.md` I8.

## Gaps / [UNVERIFIED]
- **[C] layer thin:** Reddit is blocked (CEO API key open) and caregiver forums are unreachable. L02, L03, L10, L15, L17 and L22–L30 have no opened online voices. A Reddit key or a retry of alzheimer-forum.de / pflege-forum.org would strengthen L02, L03 and L15.
- **L10:** no buyer purchase, vendor or practice/hospital complaint was opened in A7. The DKG "Das Krankenhaus 4/2026" criticism and the KV Baden-Württemberg note on parallel EBM/hybrid billing were seen in **search snippets only**.
- **L17:** no lung-screening uptake figures exist yet. Whether Kassen buy outreach tools from third parties is not shown.
- **L20:** no pharmacy purchase of shortage-management software was found (not searched in A7).
- **L25:** number of health offices not sourced.
- **Stale (>3 years):** DEVAP 2023 (L02), RWI data 2011–19 (L08), BPtK 2018–21 (L15), bpb 2015 (L04), ACT/SCRS 2023 (L27), MDS 2013 (L23).
- **Buyer counts, signer, budget line, wedge, first-sale route:** not in this file; task A18.
- **Not listed, snippets only:** ME/CFS and Long COVID care gap; rural GP intake stops.

## Sources
Carried-over sources are listed in the linked files (accessed 2026-11-06/07 by A1–A19). Opened in A7, accessed 2026-11-07:
- https://www.g-ba.de/downloads/17-98-6102/2026-03-16_oKFE-Evaluationsbericht-Darmkrebs_GFL_2021-2024.pdf — colorectal participation 7.75 %, invitation 89.5 %, follow-up 12.9 % (minimum), EU reference values [A]
- https://www.aerzteblatt.de/news/darmkrebsfruherkennung-wirkt-nur-wenige-nehmen-teil-d8b4414f-5874-4c48-8024-eb921f42fb11 — summary of the report, 336 days, <7 % within 3 months, 1 Jun 2026 [B]
- https://www.g-ba.de/presse/pressemitteilungen-meldungen/1316/ — lung LDCT screening from April 2026, eligibility, training and KV approval [A]
- https://www.aok.de/pp/gg/update/lungenkrebsscreening-startet/ — ~5.5m potential beneficiaries (DGP), approvals pending, 31 Mar 2026 [B]
- https://www.aok.de/pp/bv/wido-pm/ausgaben-hybrid-drgs/ — hybrid-DRG cases +17 %, €360m (2025), €640m expected (2026), 10 Sep 2026 [B]
- https://www.aerzteblatt.de/themen/drg/einigung-zu-fallpauschalenkatalog-fur-2026-erzielt-9f22115a-fc3d-4f21-b187-17a7ce99a35a — hybrid-DRG volume ~270,000 → ~1m cases [B]
- https://www.aerzteblatt.de/news/hybrid-drg-sollen-ab-2028-abgeschafft-werden-576552aa-a75b-4b53-ad56-e51829c020d9 — amendment: § 115f abolished from 2028, 69 hybrid DRGs / 904 OPS codes, 2027 transition, 5 Oct 2026 [B]
- https://dserver.bundestag.de/btd/21/086/2108629.pdf — "§ 115f wird gestrichen", 2028 Kurzzeitfallpauschale, 2027 rules (Health Committee report on the emergency-care reform) [A]
- https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/5_Publikationen/Pflege/Berichte/241127_Abschlussbericht_Live_Ins_bf.pdf — live-in care: no reliable household count, 100,000–210,000 carers per day [A]
- https://www.verbraucherzentrale.de/wissen/gesundheit-pflege/pflege-zu-hause/auslaendische-betreuungskraefte-wie-geht-das-legal-10601 — 24-h care by one person not legal; €2,800–3,500/month [B]
- https://www.bundesgesundheitsministerium.de/ministerium/meldungen/tag-der-seltenen-erkrankungen-2026 — ~4m people with rare diseases, >30 centres, ~5,000 in the genome-sequencing pilot [A]
- https://www.barmer.de/verantwortung/transparenz/transparenzbericht6/diagnose-krebs-1506416 — BARMER cancer navigator programmes since 2021, Jun 2026 [B]
- https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_55_56_57_Management_von_Lieferengpaessen.pdf — pharmacies 20.1 h/week on shortages; hurdles [B]
- https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_8_Entwicklung_der_Apothekenzahl.pdf — 16,601 pharmacies end-2025 [B]
- WebSearch, snippet only (not used as fact): DKG "Das Krankenhaus 4/2026" hybrid-DRG criticism; KVBW hybrid-DRG billing audits; lung-screening start reports (PZ, aponet); Hans-Böckler live-in estimate (163,000 households); Ärzte Zeitung "five million" rare-disease figure.
