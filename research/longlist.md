# Long list: 27 healthcare problems (DE/DACH first)
Task: A7 (fact-check fixes: A21; red-team fixes: A23) | Date: 2026-11-07 | Status: draft

Method: merged the 36 raw problems in `research/pain-patients.md` (P1–P11), `research/pain-professionals.md` (S1–S10), `research/pain-industry.md` (I1–I10) and `archive/cancer-problem-statement.md` (A–E), using the deep dives `research/hospital-billing-audits.md` (A11), `research/payer-processing.md` (A12), `research/trial-recruitment-de.md` (A13), `research/reimbursement-routes.md` (A9/A15) and `research/trends.md` (A1). Result in A7: 30 problems (one new: L10) and 6 items excluded or merged. **A23** applied the red-team fixes F2–F3 (`research/reviews/2026-11-07-redteam-longlist.md`): it split who-pays into "spend on this job" and "adjacent spend", added signer clusters, merged L10 → L07 and L30 → L26, and excluded L19. **27 rows remain**, with IDs unchanged. Key facts from the earlier files are carried over with their sources and grades, and were not re-opened in A7. Sources marked **(A7)** were opened in this session. Scoring fields (signer, budget line, wedge, first-sale route, buyer count, young-vendor K2 example) are in `research/longlist-scoring-fields.md` (A18); scores come in B1.

## Findings
- **A23 (red-team fixes):**
  - **27 problems remain.** L10 merged into L07, L30 merged into L26, L19 excluded; reasons are in "Excluded or merged".
  - **Spend on the job:** only **8 rows show proven spend on the same job** (L01, L05, L07, L08, L09, L21, L22, L29), down from the 15 "proven" rows in A7. In 3 of them the buyer paid the category leader. The rest of the A7 "proven" money buys care, labour, physician fees or one-off KHZG projects (see the "Adjacent spend" column).
  - **Signer clusters:** the 27 rows fall into **13 signer clusters**, 6 of them single rows (C1, C4, C10–C13) (C1–C13, table under the long list).
  - **L25:** the budget is confirmed as ending. The last ÖGD-pact tranche of €750m is paid in 2026 "zur abschließenden Erfüllung der im „Pakt für den ÖGD" gemachten Zusagen" [A] ([BT-Drs. 21/8237](https://dserver.bundestag.de/btd/21/082/2108237.pdf), 28 Sep 2026). For 2027, "Für den ÖGD sind null Euro eingeplant" [B] ([zm, 18 Aug 2026](https://www.zm-online.de/news/detail/gesundheitsetat-faellt-2027-um-ein-drittel-kleiner-aus)). L25 stays on the list so the record is complete, but it should fail K1 in B1 unless a Land programme for 2027 is found.
  - **L22 vs L07:** L22 is the payer side of L07. B1 can rank one of the two, not both (credibility conflict).
- **All 30 A7 problems met the Stage A bar** (27 after A23): each has ≥2 independent evidence items and ≥1 graded [A]/[B] (L19: 1 [B] + 3 opened [C] app feeds; L18, L24, L25, L30 and L11 have exactly 2). The [C] layer (online voices) is thin for most rows, because Reddit and several caregiver forums are blocked (A2). Only L01, L05, L06, L09, L16, L19, L20 and L21 have ≥2 opened [C] signals. Pain intensity therefore rests mostly on [A]/[B] surveys and statistics.
- **A7 counted proven spend in 15 rows (A23: 8 on the same job), but direct startup access is rare.** The A14 tender tables hold 36 notice numbers from 32 buyers (A22 recount) (16 in `pain-industry.md`, 20 in `pain-professionals.md`). Only one buyer's procedure was accessible to a new company when tendered: the MD Rheinland-Pfalz AI PoC (one PoC reference, no turnover minimum). Its request deadline was 5 Sep 2025, so it is **closed**, and TED shows no award notice [A] (TED 543912-2025, A21). No checked notice is both open today and startup-accessible. Thresholds of 7 notices from 7 buyers are still unread (5 "Unknown" hospital notices; DAK 396194-2026 "Unlikely"; gkv informatik 481787-2026, rated "No" on its 3-reference requirement alone). The DAK and gkv informatik deadlines passed (14 Jul and 10 Aug 2026) [A] (TED API, A22); their DTVP document links returned HTTP 404 to a direct request on 7 Nov 2026, so the documents were not read. UK Saarland (1 Sep 2025) and MD Bayern (28 Feb 2025) are also closed [A] (TED 508395-2025, 63363-2025/126222-2025). MD Nordrhein was read in A21 and is not accessible alone. Other hospital, insurer and MD tenders ask for €250k–€10m turnover, university-hospital/GKV references or ISO/C5 certificates [A] (TED, see `pain-industry.md` and `pain-professionals.md` "Tender access check"). *Inference:* A18 must find a direct-award, private-buyer or channel route for each row, or the row fails knock-out K2.
- **The strongest rows combine a dated rule change, a budget and founder fit** (inference, for B1 to test; red team F1: founder fit is asserted here, not shown):
  - L07/L22: hospital billing audits (A23: opposite sides of one market; pick one). Stricter quotas start 1 Jan 2027 (enacted). MD-IT has an €88m AI framework (startups only as subcontractor or consortium member). Incumbents: Tiplu/LOGEX and calliora (Munich).
  - L26: trial recruitment. Sponsors pay. From 2027, ≥5 % of trial participants at German sites can earn an exemption from the 8.5 % extra discount. But sites name staff, not patient finding, as their main hurdle, and vendors have consolidated.
  - L05: long-term-care documentation. PNOG fund from H2 2027 (bill). § 113e money from 2028 (bill). voize ($50m) leads.
- **Patient- and family-side problems are the largest by headcount, but the payer is weakest.** This covers L01–L04 and L14–L19. Statutory budgets exist (relief budget, screening benefits), but payers face a ~€15bn gap in 2027 [A] (FinanzKommission, via `trends.md`), and DiPA cannot pay for navigation-only apps [A] (`reimbursement-routes.md`). Of 31 Innovation Fund navigator projects, "In most cases, no effect was observed" [A] ([PMID 41419645](https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:41419645%20AND%20SRC:MED&format=json&resultType=core)).
- **New German data added in A7:**
  - Colorectal screening: participation was 7.75 % (averaged over stool test and colonoscopy), against an EU minimum of 45 %. Documented follow-up after a positive stool test was only 12.9 % (target 85 %; a lower bound because of documentation gaps) [A] ([G-BA evaluation report, 16 Mar 2026](https://www.g-ba.de/downloads/17-98-6102/2026-03-16_oKFE-Evaluationsbericht-Darmkrebs_GFL_2021-2024.pdf)).
  - Pharmacies spend on average 20.1 h/week managing drug shortages [B] ([ABDA ZDF 2026](https://www.abda.de/fileadmin/user_upload/assets/ZDF/ZDF-2026/ZDF_2026_55_56_57_Management_von_Lieferengpaessen.pdf)).
  - Hybrid DRGs (§ 115f SGB V) are to be deleted and replaced by short-stay flat rates in 2028. The Bundestag passed this on 15 Oct 2026 [A] ([BR-Drs. 620/26](https://dserver.bundestag.de/brd/2026/0620-26.pdf); text in [BT-Drs. 21/8629](https://dserver.bundestag.de/btd/21/086/2108629.pdf)). **Not yet law:** the Bundesrat handles it on 20 Nov 2026.
  - Live-in care: 100,000–210,000 carers on any given day [A] ([BMG report, Nov 2024](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/5_Publikationen/Pflege/Berichte/241127_Abschlussbericht_Live_Ins_bf.pdf)).

## Long list
Legend (revised in A23 per red team F2):
- **Cluster:** signer cluster, see the cluster table below. Rows in one cluster share a signer type and buying route.
- **Spend on this job:** money the signer type pays today for the *same job* the row describes.
  - *proven*: a named buyer paid (award notice, named contract or named customer);
  - *commissioned/tendered*: a named buyer commissioned or tendered the job, but the award or fee was not seen;
  - *vendor market*: vendors sell the job (price lists, scale claims), but no named buyer is in the repo;
  - *budget*: a statutory or budget line for this job is in force, but no product purchase was observed;
  - *budget ended*: the money stops before 2027;
  - *none observed*.
- **Adjacent spend:** money near the problem that buys something else (care, labour, physician fees, one-off grants). It does not pass K1.
- **Evidence:** number of independent [A]/[B] items (of which [A]) / opened [C] signals.
- **Source rows:** IDs in the A3–A5 files and the cancer file.
- L10, L19 and L30 left the list in A23 (see "Excluded or merged"); their evidence stays under Details. IDs are not renumbered.

| # | Cluster | Problem (one line) | Who has it | Spend on this job (status) | Adjacent spend (not this job) | Evidence [A/B] ([A]) / [C] | Source rows → files |
|---|---|---|---|---|---|---|---|
| **Long-term care and families** ||||||||
| L01 | C5 | Families cannot navigate home-care benefits (care grade, relief budget, respite care), so entitlements go unused | ~4.9m people cared for at home + family carers | Employers: *proven* (heycare names Daimler Truck, Douglas, Vaillant, VW Retail, Mar 2026 [B], A18). Pflegekassen: *none observed* (§ 7a counselling runs in-house; 3 % use it) | €131/month relief budget (pays relief services, not navigation); DiPA excludes navigation-only apps [A] | 8 (4) / 4 | P1 → `pain-patients.md`, `reimbursement-routes.md` |
| L02 | C5 | Families cannot find care capacity (home-care service, short-term/day care, care-home place) | Same + hospital discharge cases | *None observed* for search/matching paid by families or providers. Hospital-side matching = L08. A free counselling portal exists (Verbund Pflegehilfe: "berät seit 2008 kostenlos", 1.5m consultations/yr [B], A23); its revenue model is not stated | Self-pay €3,364/month in care homes (buys care); 91 % of services turn clients away (supply is the constraint) | 6 (1) / 0 | P2 → `pain-patients.md`, `trends.md` |
| L03 | C5 | Family carers are overloaded and cut working hours | Families of 3.1m care recipients cared for mainly by relatives | Pflegekassen: *commissioned* (Mobil Krankenkasse, ZF BKK × PflegeBetreuer, 2026 [B], A18; fee not stated) on a *budget* line (§ 45 SGB XI courses, in force [A]). Employers: = L01 | Hours lost by carers (no buyer) | 4 (1) / 0 (18 titles) | P3 → `pain-patients.md` |
| L04 | C5 | 24-h live-in care runs in a legal grey zone with no reliable data | Households of high-need elderly; 100k–210k live-in carers | *None observed* for software or compliance tools | Self-pay €2,800–3,500/month + agency fees (buys labour) | 3 (1) / 0 | P11 → this file (A7) |
| L05 | C10 | Documentation and admin load in long-term and home care; care homes lag on digital tools and the TI | 446,425 home-care + 817,711 care-home staff; ~32,000 facilities | Operators: *proven* for voice documentation (voize: Caritas Stuttgart Jan 2022 [B], 1,100 facilities), i.e. the leader's product. TI/KIM onboarding sub-wedge (A18): *none observed* | § 8 Abs. 8 grant (40 % of spend, max €12k/facility; €143.3m paid 2019–24 ≈ 37 % of pool [A]; workflow purposes drop out from 2027 under PNOG); PNOG fund 2027+ and § 113e 2028+ (*bills*) | 7 (5) / 2 | S2 → `pain-professionals.md`, `reimbursement-routes.md`, `trends.md` |
| **Hospitals** ||||||||
| L06 | C2 | Physicians and nurses spend hours a day on clinical documentation (letters, ward notes) | ~176,800 physician FTE, ~391,000 nursing FTE | *Tendered* once: Harzklinikum CDSS incl. "LLM-basierte Arztbriefschreibung" (TED 492877-2025 [A]; KHZG one-off money; needs a full German-clinic reference). No award to a young vendor seen | 8 speech-recognition buyers (dictation, a different product; tenders mostly closed to startups); UKE and Leipzig build in-house [B] | 6 (3) / 2 | S1 → `pain-professionals.md` |
| L07 | C1 | Hospitals lose revenue in MD billing audits; quotas rise to up to 40 % from 2027 (incl. outpatient-rule churn from merged L10) | 1,603 hospital IKs; medical controlling, coders | *Proven*: UK Frankfurt coding-revision award (€181,800 / 3 yrs), Charité coding framework (award Jun 2025) [A]; Tiplu named users (UK Leipzig, UK Würzburg …) [B]. DKI median €40k planned non-staff spend [B] | Audit staff (DKI mean €236k/yr, labour) | ≥8 (≥5) / 1 | S3 → `hospital-billing-audits.md`, `pain-professionals.md` |
| L08 | C2 | Discharge and transitions fail: follow-up care not found, medication lists missing, bed blocking | 17.7m inpatients (2025), older polypharmacy patients; social services | *Proven*: Helios framework (TED 24618-2025) + 4 other buyers; Uniklinik Köln → Recare (2023) [B]. **But** paid from KHZG one-off money (Land applications closed 31 Dec 2021, § 14a KHG [A]); no recurring budget seen. Kassen: pilots only | KHZG penalty weights actual *use* from 2027 (20 %) [A]: pressure to use tools already bought, not new money | 7 (4) / 1 | P7 + S8 → `pain-patients.md`, `pain-professionals.md` |
| L09 | C2 | Staff shortage forces short-notice cover; agency premiums no longer refinanced | Ward managers, nurses, physicians | *Proven* for rostering software (≥10 buyers, TED [A]). Shift-pool wedge: *vendor market* (CrewLinQ ">100 Pflegeeinrichtungen", none named [B]) | Agency premiums (labour; not refinanced from 2027 [A]) | 6 (3) / 9 kununu | S7 → `pain-professionals.md` |
| L11 | C11 | Onboarding foreign-trained nurses and physicians is slow (recognition, language) | Hospitals, care operators | *None observed* | Recruiting budgets and recruiter fees `[UNVERIFIED]` | 2 (1) / 0 | S10 → `pain-professionals.md` |
| **Practices and access** ||||||||
| L12 | C6 | Practices drown in free-form payer and agency requests and forms | 191,875 contract physicians/psychotherapists | *None observed* (practice opex; insurers/MD co-own the problem) | — | 3 (0) / 1 | S4 → `pain-professionals.md` |
| L13 | C6 | Phones and reception are overloaded; medical assistants (MFA) are scarce | Practices, MFAs | *Vendor market*: 10 AI phone vendors at €9–229/month [B]; no named paying practice found (A18) | — | 4 (0) / 0 | S5 → `pain-professionals.md` |
| L14 | C6 | Patients wait weeks for specialist appointments; booking and steering are fragmented | GKV insured; worst for those in poor health | *None observed* for a booking/steering product; patients use free apps (Doctolib, 116117) | €2.9bn extra TSVG fees [B]: these are physician fees for referred cases, paid outside the budget (§ 87a Abs. 3 SGB V [A], A23) | 5 (1) / 1 app feed | P4 → `pain-patients.md`, `trends.md` |
| L15 | C7 | Psychotherapy waiting times are long (contested size) | People with mental illness, children | *None observed* | Therapy capacity (GKV, self-pay) | 3 (0) / 0 | P5 → `pain-patients.md` |
| **Patients: specific conditions and services** ||||||||
| L16 | C7 | Cancer patients lack orientation and coordination between diagnostic and treatment steps | 566,587 new cancer cases/yr in DE (GLOBOCAN 2024) + relatives | Kassen: in-house only (BARMER navigators [B]). PKV: *commissioned* (Debeka × iuvando Health, Oct 2025 [B]; fee not stated; vendor >5 years old) | — | 3 (2) / 5 | P8 + cancer E → `pain-patients.md`, `archive/cancer-problem-statement.md`, this file |
| L17 | C7 | Few eligible people take up cancer screening, and follow-up of positive results is poorly documented | Insured ≥50 (colorectal); ~5.5m current/ex-smokers (lung, since Apr 2026) | *None observed* for outreach or eligibility tools | Statutory screening benefits pay for the exam and the invitation letters, not for a third-party tool | 4 (2) / 0 | cancer A + B (US data) → replaced with DE data in this file (A7) |
| L18 | C7 | Rare-disease patients wait years for a diagnosis | ~4m people in DE | Pharma patient finding: *plausible*, `[UNVERIFIED]` | GKV rare-disease centres, genome-sequencing pilot | 2 (2) / 0 (2 titles) | P9 → `pain-patients.md`, this file |
| L20 | C12 | Drug shortages harm chronic patients and cost pharmacies ~20 h/week | Chronic patients; 16,601 pharmacies | *None observed* (3 searches, A18). Apo-Mall "Bestell-Engel" (~1,100 users) was built by pharmacist-wholesalers; price not seen | Pharmacy staff time (20.1 h/week [B]) | 5 (0) / 2 | P6 → `pain-patients.md`, this file |
| **Payers and the MD** ||||||||
| L21 | C3 | Insurers process §302 invoices from other providers largely on paper and outsource them | 92 statutory insurers' claims departments | Kassen → BPO service: *proven* (9 buyers, 13 awards to incumbents [A]). A tool sold *to a BPO* (A18 wedge): *none observed* | Admin-cost cap from 2027 [A] limits growth | 8 (6) / 3 kununu | I5 → `payer-processing.md`, `pain-industry.md` |
| L22 | C3 | MDs and insurers cannot handle the 2027 hospital-audit volume with current processes. **Opposite side of L07:** selling audit AI to both hospitals and MDs is a credibility conflict; B1 can rank one of the two, not both | 15 MDs (2,148 physician FTE), insurer hospital-bill teams | *Proven*: TK → QuantCo DRG scoring (2026) [A]. *Tendered*: MD-IT €88m AI framework (consortia only, bids 2 Dec 2026) [A]; MD Niedersachsen €2m external review services (TED 383478-2026) [A] | — | 6 (5) / 0 | I6 (part) → `payer-processing.md`, `hospital-billing-audits.md` |
| L23 | C3 | MD care-need assessments have doubled in volume (>3m in 2025) | 15 MDs; applicants waiting | *Tendered*: MD RLP AI PoC (startup-accessible, closed 5 Sep 2025, no award); MD Nordrhein AI tender (open to 3 Dec 2026; needs €600k turnover and a ≥€500k own-development reference) [A] | — | 6 (5) / 1 kununu | I6 (part) → `pain-industry.md`, `payer-processing.md` |
| L24 | C4 | Private insurers check >70m invoices a year, and a new fee schedule (GOÄ) is planned for 2028 | PKV claims teams | *Plausible*: in-house claims + IT vendors (search snippets only); no named purchase | — | 2 (0) / 0 | I7 → `pain-industry.md` |
| L25 | C13 | Public-health offices must keep digital projects running after federal pact money ends in 2026 | ~375 local health offices (2020) [B, stale] | *Budget ended*: the last pact tranche (€750m via VAT shares) is paid in 2026 "zur abschließenden Erfüllung" [A]; the 2027 federal draft budget has "null Euro" for the ÖGD [B] (A23). Some Länder may continue (snippets only) | — | 4 (1) / 0 (A23 added BT-Drs. 21/8237 [A] and zm [B]) | I9 → `pain-industry.md` |
| **Pharma, clinical research, medtech** ||||||||
| L26 | C8 | German trial sites miss recruitment targets; Germany's share of trial participants is ~2.9 % | Sponsors, CROs, site staff; patients without trial access | Sponsors/CROs → recruitment services: *vendor market* at scale (Clariness ">42,000 randomizations" [B]); no named DE sponsor buyer in the repo. Site-paid patient-finder tool: *none observed* (MPIRIQ price list €99–329/month, no named customer [B]) | Sponsor fees *to sites* for identification work (billable activity in the joint costing recommendations [B]): pays site staff, not a tool | ≥12 (≥6) / weak | I1 + cancer C → `trial-recruitment-de.md`, `pain-industry.md` |
| L27 | C8 | Trial-site start-up is slow: contracts, budgets, CTIS documents, system training | Study nurses, investigators, CRO start-up teams | *Plausible* (sponsors/CROs); no purchase observed | Site overhead | 5 (2) / 1 | I2 → `pain-industry.md` |
| L28 | C9 | EU joint clinical assessments (JCA) and AMNOG dossiers need many PICOs under tight deadlines | Pharma market-access teams, small biotechs | *Vendor market*: consultancies and CROs sell JCA services (EVERSANA, Parexel, IQVIA) [B]; no named buyer | — | 4 (1) / 0 | I3 → `pain-industry.md` |
| L29 | C9 | MDR/IVDR certification takes ~20 months and costs SMEs R&D projects | Device and IVD makers (mostly SMEs) | *Proven*: Flinn × Paul Hartmann (Feb 2026) [B], A18; RA consultants | Staff time; notified-body fees | 5 (1) / 0 | I4 → `pain-industry.md` |

### Signer clusters (A23, from red team F3)
One wedge per cluster in the top 5 is the S4 proposal (CEO decision open). Where the A18 wedge has a different signer than the row's cluster, B1 should use the wedge signer: L16 wedge → PKV (C4), L17 wedge → GP/radiology practices (C6).

| Cluster | Signer type | Rows |
|---|---|---|
| C1 | Hospital commercial director / medical controlling (revenue, coding) | L07 (+ merged L10) |
| C2 | Hospital medical/nursing director, CIO, social services (clinical workflow) | L06, L08, L09 |
| C3 | Statutory payers and MDs (claims, audits, assessments) | L21, L22, L23 |
| C4 | Private health insurers (PKV) | L24 |
| C5 | Family carer support: employer HR, Pflegekasse, families | L01, L02, L03, L04 |
| C6 | Practice owner | L12, L13, L14 |
| C7 | Patient navigation in a disease (Kasse) | L15, L16, L17, L18 |
| C8 | Sponsors/CROs (clinical research) | L26, L27 (+ merged L30) |
| C9 | Manufacturers: regulatory/market access | L28, L29 |
| C10 | Care-operator management | L05 |
| C11 | Employer HR (hospital, care operator) | L11 |
| C12 | Pharmacy owner | L20 |
| C13 | Local health office (municipal) | L25 |

Count from the table above:
- *Proven* spend on the job: **8 of 27 rows** (L01, L05, L07, L08, L09, L21, L22, L29). In L05, L08 and L29 the named buyer paid the category leader (voize, Recare, Flinn). In L08 the money was the KHZG one-off fund. In L21 the buyers paid incumbent BPOs, not a tool.
- *Commissioned/tendered* only: L03, L06, L16, L23. *Vendor market* without a named buyer: L13, L26, L28.
- *None observed*, *plausible* or *budget ended*: the other 12 (L02, L04, L11, L12, L14, L15, L17, L18, L20, L24, L25, L27).
- The A7 Findings said "proven spend exists in 15 rows". Under the stricter F2 reading it is 8.

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
| **L10** outpatient-rule churn (A23) | **Merged into L07** | Same signer (medical controlling), same vendors, same software category (red team F3). On the practice side the basic tool is free: KVSH offers "einen DRG-Grouper zur kostenfreien Nutzung über das Mitgliederportal" [B] ([KVSH, 25 Mar 2024](https://kvsh.de/fileadmin/user_upload/dokumente/Praxis/Vertraege/Hybrid-DRG/2024_03_25_Hybrid-DRG_Informationsschreiben.pdf)), and KVBW has offered a certified grouper in its member portal since 13 Feb 2025 [B] ([KVBW](https://www.kvbawue.de/praxis/aktuelles/nachrichten-zum-praxisalltag/news-artikel/hybrid-drg-grouper-ab-sofort-im-portal-verfuegbar)). The 2028 short-stay flat rates stay as a possible L07 wedge |
| **L30** FDZ data access (A23) | **Merged into L26** | The A7 file already called it "an enabler for L26 rather than a pain". Same buyer (pharma RWE/clinical ops), and only 53 FDZ applications so far |
| **L19** ePA/ident apps (A23) | **Excluded** (S6 stays excluded) | Same reason as S6. The insurers must provide an ePA "zugelassene" by gematik (§ 342 Abs. 1 SGB V) [A]. TI components and services need gematik approval (§ 325 Abs. 1) [A]. gematik sets the security requirements for the digital identity "im Benehmen mit dem Bundesamt für Sicherheit in der Informationstechnik" (§ 291 Abs. 8 SGB V) [A]. A startup cannot fix login or ident UX from outside this approval chain (inference). Un-excluding S6 instead would add a second row that no product can solve |
| L25 public health (A23) | **Kept, flagged "budget ended"** | The budget line ends in 2026 (BT-Drs. 21/8237 [A]; 2027 federal draft budget: zero for the ÖGD [B]). Excluding it is a K1 judgement for B1, not a scan decision |

## Details: evidence per problem
Grades as in the source files. "→" = file with full sources.

**L01 Home-care benefit navigation**
- Only "3 Prozent der Anspruchsberechtigten" use statutory care counselling [A] ([GKV-SV § 7a report, Jun 2026](https://www.gkv-spitzenverband.de/media/dokumente/pflegeversicherung/beratung_und_betreuung/pflegeberatung/2026-06_Bericht_des_GKV-Spitzenverbandes_7a_Absatz_9_SGB_XI.pdf)).
- 38.4 % of Pflegegeld recipients used the relief budget (2022) [B] ([AOK G+G](https://www.aok.de/pp/gg/magazine/gesundheit-gesellschaft-07-2024/pflegebetrag/)).
- Counter-evidence: the main reasons for non-use are "fehlender Bedarf" and preference [B] ([WIdO 2026](https://www.wido.de/fileadmin/user_upload/20260511_WIdO-PM_WIdOmonitor_Pflegende_Angehoerige.pdf)).
- DiPA excludes navigation-only apps [A] ([§ 40a SGB XI](https://www.gesetze-im-internet.de/sgb_11/__40a.html)).
- → `pain-patients.md` P1.

**L02 Care capacity**
- **A23:** Verbund Pflegehilfe "berät seit 2008 kostenlos" families, runs "1,5 Millionen Beratungsgesprächen pro Jahr" with >240 staff, and sells an "Entlass-Manager" to hospitals (users include Ortenau Klinikum and Klinikum Altenburger Land) with a network of ">41.000 Anbietern" [B] ([press release, Jan 2025](https://static.pflegehilfe.org/press/pressemitteilung-01.2025-entlass-manager-als-unverzichtbares-kliniktool.pdf)). *Inference:* family-side matching is already given away free, and someone (providers or hospitals) funds it. The revenue model is not stated `[UNVERIFIED]`. This adds an L08 incumbent.
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

**L10 Rules for outpatient-capable procedures keep changing (new, A7; merged into L07 in A23)**
- Volume: the 2026 catalogue *scope* grew from about 270,000 to about one million cases ("von rund 270.000 auf etwa eine Million Fälle ausgeweitet"); these are cases in scope, not billed hybrid-DRG cases. The late hybrid decision held up the whole 2026 DRG catalogue [B] ([Ärzteblatt](https://www.aerzteblatt.de/themen/drg/einigung-zu-fallpauschalenkatalog-fur-2026-erzielt-9f22115a-fc3d-4f21-b187-17a7ce99a35a)).
- Spending: WIdO estimates +17 % cases and about €360m extra GKV spending in 2025. Practice cases rose 65 % (219,000 → 363,000) and hospital cases 6 % (932,000 → 986,000). WIdO expects about €640m extra in 2026 [B] ([WIdO, 10 Sep 2026](https://www.aok.de/pp/bv/wido-pm/ausgaben-hybrid-drgs/)).
- Rule change: the emergency-care reform deletes § 115f ("§ 115f wird gestrichen"). Hybrid DRGs are replaced by short-stay flat rates (Kurzzeitfallpauschalen) in 2028. 2027 has a transition rule: cases without an overnight stay are paid fully under the EBM [A] (committee text: [BT-Drs. 21/8629](https://dserver.bundestag.de/btd/21/086/2108629.pdf)) [B] ([Ärzteblatt, 5 Oct 2026](https://www.aerzteblatt.de/news/hybrid-drg-sollen-ab-2028-abgeschafft-werden-576552aa-a75b-4b53-ad56-e51829c020d9)).
- Status: **passed by the Bundestag, not yet law.** The Bundestag adopted the committee version in its 102nd session on 15 Oct 2026 ("mit beigefügten Maßgaben, im Übrigen unverändert angenommen"; Fristablauf 20 Nov 2026); the Bundesrat print contains "§ 115f wird gestrichen" and the 2028 Kurzzeitfallpauschale [A] ([BR-Drs. 620/26](https://dserver.bundestag.de/brd/2026/0620-26.pdf), A21). The Bundesrat sits on 20 Nov 2026; the law needs no consent (A17).
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
- **A23:** the TSVG extra fees are physician fees. Services "aufgrund der Vermittlung durch die Terminservicestelle" are paid outside the capped budget [A] ([§ 87a Abs. 3 SGB V](https://www.gesetze-im-internet.de/sgb_5/__87a.html)). So they are adjacent spend, not a software budget.
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

**L19 ePA onboarding** (excluded in A23, see "Excluded or merged")
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
- MD RLP AI PoC: only 1 reference needed, no turnover minimum; 40 requests to participate [A]. **Closed:** the first procedure ended without award ("change of need", TED 483916-2025); the re-tender's request deadline was 5 Sep 2025, and TED shows no award notice as of 7 Nov 2026 [A] (TED 543912-2025, A21). It shows that an entry route existed, not a live opportunity.
- **A21:** MD Nordrhein's AI tender for malpractice reviews (open procedure, deadline 3 Dec 2026) requires an average in-field turnover of "mindestens 600.000 EUR netto" a year (available years if younger), ≥4.0 FTE besides project lead and deputy, two references for AI software in productive use (≥12 months of operation for one area), and at least one reference with own development work of "mindestens 500.000 EUR" net order value ("reine Lizenz-, Hosting- und Supportentgelte zählen nicht"; item 6.2 R6). Consortia are allowed and prove eligibility jointly; subcontracting is allowed, but project lead, architecture and information security must stay with the bidder or a consortium member, and a subcontractor counts towards eligibility only via capacity borrowing ("Eignungsleihe", § 47 VgV) [A] ([aumass tender documents AV28F1E8-EU](https://plattform.aumass.de/Veroeffentlichung/av28f1e8-eu), `Fragebogen_Eignung_MD_Nordrhein.xlsx` items 4.3, 5.3–5.5, 6.1–6.3; `Angebotsbedingungen.pdf` §§ 4–5; R6 re-read in A22). *Inference:* not accessible to a new company alone; possible only inside a consortium whose other members bring the turnover and the €500k reference. A subcontract for non-critical parts under a qualified bidder is also possible on paper (inference; no example found).
- → `pain-industry.md` I6, `payer-processing.md` §3.

**L24 PKV and GOÄ**
- More than 70m invoices a year [B].
- New GOÄ "zum 1. Januar 2028 erreichbar" [B].
- → `pain-industry.md` I7.

**L25 Public health (ÖGD)**
- The €4bn pact (2021–26) ends without follow-up money [B].
- **A23:** the federal cabinet's FAG amendment raises the Länder's VAT share by €750m in 2026 "zur abschließenden Erfüllung der im „Pakt für den ÖGD" gemachten Zusagen" [A] ([BT-Drs. 21/8237, 28 Sep 2026](https://dserver.bundestag.de/btd/21/082/2108237.pdf)). An aggregator headline dates this money to "2027" (mydrg, 21 Aug 2026, citing Ärzte Zeitung; the article itself was not opened). The bill text says 2026 and "abschließend".
- The 2027 federal draft budget: "Für den ÖGD sind null Euro eingeplant" (2026: €52m) [B] ([zm, 18 Aug 2026](https://www.zm-online.de/news/detail/gesundheitsetat-faellt-2027-um-ein-drittel-kleiner-aus)). BVÖGD criticises the federal plan to provide "ab Ende 2026 keine weiteren Finanzmittel" [B] ([BVÖGD statement, Jun 2026](https://www.bvoegd.de/wp-content/uploads/2026/06/2606-Stellungnahme-BeitragssatzstabG.pdf)).
- Some Länder may fund on their own: Niedersachsen and Baden-Württemberg appeared in search snippets only (not opened).
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

**L30 FDZ data access** (merged into L26 in A23)
- Companies may apply [A] (§ 303e SGB V).
- 53 applications by Feb 2026; claims data only so far [B].
- *Inference:* an enabler for L26 rather than a pain.
- → `pain-industry.md` I8.

## Gaps / [UNVERIFIED]
- **A23:** the "spend on this job" labels rest on facts already in the repo plus 12 sources opened in A23. No new purchase search was run per row, so *none observed* means "not found in the A3–A18 searches". The revenue model of Verbund Pflegehilfe (L02) and Land-level ÖGD money for 2027 (L25) are `[UNVERIFIED]`.
- **[C] layer thin:** Reddit is blocked (CEO API key open) and caregiver forums are unreachable. 15 rows have no opened online voices: L02, L03, L04, L10, L11, L13, L15, L17, L18, L22, L24, L25, L28, L29, L30 (L03 and L18 have titles only). L23 and L27 have 1 opened signal each; L26 is weak (CRO kununu pages in `pain-industry.md` I1). A Reddit key or a retry of alzheimer-forum.de / pflege-forum.org would strengthen L02, L03 and L15.
- **L10:** no buyer purchase, vendor or practice/hospital complaint was opened in A7. The DKG "Das Krankenhaus 4/2026" criticism and the KV Baden-Württemberg note on parallel EBM/hybrid billing were seen in **search snippets only**.
- **L17:** no lung-screening uptake figures exist yet. Whether Kassen buy outreach tools from third parties is not shown.
- **L20:** no pharmacy purchase of shortage-management software was found (not searched in A7).
- **L25:** number of health offices not sourced.
- **Stale (>3 years):** DEVAP 2023 (L02), RWI data 2011–19 (L08), BPtK 2018–21 (L15), bpb 2015 (L04), ACT/SCRS 2023 (L27), MDS 2013 (L23).
- **Buyer counts, signer, budget line, wedge, first-sale route:** see `research/longlist-scoring-fields.md` (A18).
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

Opened in A21 (fact-check fixes), accessed 2026-11-07:
- https://api.ted.europa.eu/v3/notices/search — TED 343840-2025 / 483916-2025 (MD RLP PoC, award notice: no award, "chan-need", 40 requests) and 500590-2025 / 543912-2025 (re-tender, request deadline 5 Sep 2025; no award notice under procedure 7f90bc94-…); TED 762721-2026 (MD Nordrhein, open procedure, deadline 3 Dec 2026) [A]
- https://plattform.aumass.de/Veroeffentlichung/av28f1e8-eu — MD Nordrhein tender documents (public download without registration): eligibility form (€600k average in-field turnover, ≥4.0 FTE, 2 productive AI references, R6 ≥€500k own-development reference), consortia and subcontracting rules (re-downloaded 2026-11-07, A22) [A]
- https://api.ted.europa.eu/v3/notices/search — A22 deadline checks: 396194-2026 (DAK, 14 Jul 2026), 481787-2026 (gkv informatik, 10 Aug 2026; ≥3 references), 508395-2025 (UK Saarland, 1 Sep 2025), 63363-2025 / 126222-2025 (MD Bayern, 28 Feb 2025), accessed 2026-11-07 [A]
- https://www.dtvp.de/Satellite/notice/CXS0YRXYT2XCRM06/documents and https://www.dtvp.de/Satellite/notice/CXP4YMPM3VS/documents — DAK and gkv informatik document links from TED; HTTP 404 on 2026-11-07 (A22)
- https://dserver.bundestag.de/brd/2026/0620-26.pdf — Bundesrat print 620/26: Bundestag decision of 15 Oct 2026 (102nd session), "§ 115f wird gestrichen", Kurzzeitfallpauschale 2028, Fristablauf 20 Nov 2026 [A]

Opened in A23 (red-team fixes), accessed 2026-11-07:
- https://dserver.bundestag.de/btd/21/082/2108237.pdf — FAG-Änderungsgesetz 2026 (BT-Drs. 21/8237, 28 Sep 2026): last ÖGD-pact tranche €750m via the Länder VAT share in 2026, "abschließend" [A]
- https://www.zm-online.de/news/detail/gesundheitsetat-faellt-2027-um-ein-drittel-kleiner-aus — 2027 federal draft budget: "null Euro" for the ÖGD (2026: €52m), 18 Aug 2026 [B]
- https://www.bvoegd.de/wp-content/uploads/2026/06/2606-Stellungnahme-BeitragssatzstabG.pdf — BVÖGD: no federal money after the pact ends in 2026 [B]
- https://www.mydrg.de/myDRG_archives/gesundheitspolitik/der-pakt-fuer-den-oeffentlichen-gesundheitsdienst-laeuft-aus.html — headline "Länder erhalten 2027 vom Bund 750 Millionen Euro" (aggregator; conflicts with the bill text on the year) [B]
- https://kvsh.de/fileadmin/user_upload/dokumente/Praxis/Vertraege/Hybrid-DRG/2024_03_25_Hybrid-DRG_Informationsschreiben.pdf — KVSH free DRG grouper for practices via the member portal [B]
- https://www.kvbawue.de/praxis/aktuelles/nachrichten-zum-praxisalltag/news-artikel/hybrid-drg-grouper-ab-sofort-im-portal-verfuegbar — KVBW certified hybrid-DRG grouper in the member portal, 13 Feb 2025 [B]
- https://www.gesetze-im-internet.de/sgb_5/__342.html — ePA must be gematik-approved [A]
- https://www.gesetze-im-internet.de/sgb_5/__325.html — gematik approval of TI components and services [A]
- https://www.gesetze-im-internet.de/sgb_5/__291.html — digital identity: gematik requirements set with BSI (Abs. 8) [A]
- https://www.gesetze-im-internet.de/sgb_5/__87a.html — TSS-referred services paid outside the budget (Abs. 3) [A]
- https://www.gesetze-im-internet.de/khg/__14a.html — KHZG Land applications due by 31 Dec 2021 [A]
- https://static.pflegehilfe.org/press/pressemitteilung-01.2025-entlass-manager-als-unverzichtbares-kliniktool.pdf — Verbund Pflegehilfe: free family counselling, 1.5m consultations/yr, hospital Entlass-Manager, >41,000 providers [B]
- WebSearch, snippet only (not used as fact): Pflegeplatzmanager pricing (none published); Niedersachsen/BW ÖGD money from 2027.
