# Long-list scoring fields (signer, budget, wedge, route, buyer count)
Task: A18 | Date: 2026-11-07 | Status: draft

Linked from `research/longlist.md`. One provisional wedge per row (signer + product), as `research/scoring.md` v3 fix 3 requires. Wedges, prices and ACV figures are **my inference** unless a source is given. Facts carried over from earlier files keep their grade and file pointer and were not re-opened here. Sources opened in this session are listed at the end (accessed 2026-11-07).

## Findings
- **Seven wedges now have a young vendor with a named customer. None of these vendors is open to this founder, and in three rows the vendor leads its category (S2).**

  | Vendor | Row | Founded | Named customer (date) | Grade | What the evidence does not show | Category leader (S2)? |
  |---|---|---|---|---|---|---|
  | voize | L05 | 2020 | Caritasverband Stuttgart, "Start mit voize: Januar 2022", 5 care homes | [B] vendor case page | — | Yes |
  | heycare | L01/L03 employer wedge | 2022 (as heynanny) | Daimler Truck, Douglas, Vaillant, VW Retail ("laut Unternehmen", Mar 2026) | [B] | The date of the first sale | — |
  | Gesundheit von Morgen GmbH (PflegeBetreuer) | L03 Pflegekasse wedge | Not found | Mobil Krankenkasse (7 May 2026), ZF BKK (9 Jul 2026); both Kassen announced it | [B] | Founding year; fee | — |
  | Flinn | L29 | 2022 | Paul Hartmann, quoted by its SVP Regulatory Affairs (Feb 2026); also names Carl Zeiss and Philips | [B] | — | Yes |
  | Recare | L08 | Not verified | Uniklinik Köln (KHZG tender, 7 Nov 2023); 12 Knappschaftskliniken via Telekom (2023) | [B] | Founding year | Yes |
  | CrewLinQ | L09 | — | ">100 Pflegeeinrichtungen", none named | [B] | Any named customer | — |
  | calliora | L07 | — | Still no named hospital | — | Any named hospital | — |

- **No young vendor with a named paying customer was found for L06, L07, L12, L13, L17, L20, L21, L23, L24, L26, L27 or L28.**
  - L06: Tandem Health (founded 2023, Stockholm) says it is used in ">10,000 healthcare facilities in 14 European countries – including Germany", but names no German customer [B].
  - L26: MPIRIQ (founded spring 2024) names no paying practice or sponsor [B].
  - L16: the PKV insurer Debeka partnered with iuvando Health for trial access (22 Oct 2025) [B]. iuvando was founded in 2019, so it was about 6 years old at that deal and fails the ≤5-year test. No fee is stated.
  - Absence in 1–3 searches per row is not proof of absence.
- **Private, self-serve buyers exist in 6 rows, and procurement law does not apply to them:**
  - practices (L12, L13: ~98,000 practices + ~4,900 MVZ [B]);
  - pharmacies (L20: 16,601 [B]);
  - care operators (L05, L09: 16,505 care homes + 15,549 home-care services [A]; 42 % of care homes are private [B]);
  - large employers (L01/L03: 18,632 legal units with ≥250 employees [A]);
  - device makers (L29: 1,480 firms with >20 staff + ~12,000 micro firms [B]);
  - PKV insurers (L24: 39 full members [B]).
  - Hospitals: 729 of the 1,807 are privately owned (2025) [A]. Their purchasing rules below the EU threshold are `[UNVERIFIED]` (see `scoring.md`).
- **New [A] fact for L22: MDs buy audit capacity as a service.** MD Niedersachsen tendered "ca. 20.000 Aufträge" of complete DRG audits to external review firms over 4 months. The estimate is €2m in 4 lots of €500k each. The selection criteria are turnover "der ausgeschriebenen Leistung der letzten drei Jahre" and "Referenzprojekte" (TED 383478-2026, deadline 3 Jul 2026, closed).
  - So the 2027 quota wave is partly bought as physician review work, not as software.
  - *Inference:* a new company could enter only as a review-services firm with references.
- **The Telekom TechBoost intake is published, but it is not a first-sale route for a new company (S3).**
  - The programme asks: "Do you have a marketable product and have successfully completed initial B2B customer projects?" [B].
  - The entry tier, TechBoost Connect, needs "an MVP and a commercial register entry".
  - So the channel opens only after the first customers. L21 stays "K2 unproven". No partnership between a § 302 BPO and a startup was found.
- **New trigger for L05: Rhineland-Palatinate credits speech documentation as staff time.**
  - Since 1 Oct 2026, care homes in Rhineland-Palatinate that use speech documentation can count 0.5 FTE toward their agreed staffing (§ 19a of the framework contract, signed 22 Sep 2026). Source: voize's own blog [B]; the contract text itself was not opened.
  - *Inference:* this subsidises the leader's product. It makes a new voice-documentation wedge harder, not easier.
- **The trigger dates favour late entrants in only a few rows.** Measured against the founder's full-time start in Sep 2027 (inference), the triggers that start after that date are:
  - L10/L07: short-stay flat rates, 2028 (bill passed by the Bundestag; Bundesrat on 20 Nov 2026);
  - L24: GOÄ, planned for 2028;
  - L05: § 113e money, 2028 (bill);
  - L26: 5 % rule, launches from 2027.

  Most other triggers fall in 2026 or 1 Jan 2027: audit quotas, lung screening, the TI obligation.

## Table 1: who, signer, budget, wedge
Clusters follow red-team F3 (`research/reviews/2026-11-07-redteam-longlist.md`). They are provisional. A23 set the final clusters (C1–C13) and merges in `research/longlist.md`: L10 → L07, L30 → L26, L19 excluded. **Budget line:** *job* = the signer pays today for the same job; *adjacent* = money exists nearby but buys something else (F2).

| # | Cluster | User | Signer (role + org type) | Budget line | Wedge: product → first customer type; price/ACV guess (inference) |
|---|---|---|---|---|---|
| L01 | Carer support | Family carer who is also an employee | Employer HR / benefits lead (large firm) | *Job (employer):* EAP/benefit budgets. heycare sells exactly this. *Adjacent:* § 7a counselling (Pflegekassen run it in-house) | Care-benefit navigator as an employee benefit (merge with L03) → employer with ≥250 staff; ~€5–20k/yr |
| L02 | Carer support | Family looking for a care place | None for search. Hospital side = L08 | *Adjacent:* families pay for care, not for search (F2) | No viable wedge: supply is the constraint (red team: out) |
| L03 | Carer support | Family carer | (a) Pflegekasse head of care services; (b) employer (= L01) | *Job (a):* § 45 SGB XI carer courses, in force [A] (`scoring.md`) | Personalised online carer course → BKK-size Pflegekasse; fee unknown. Pilot ≤€50k direct award |
| L04 | Carer support | Household using live-in care | Agency owner | *Adjacent:* labour fees €2,800–3,500/month [B] (`longlist.md`) | Compliance/contract software for agencies. Not a fit for a software founder (red team: out) |
| L05 | Single | Care staff | Managing director / care manager (Pflegedienstleitung) of a care operator (42 % of homes private) | *Job:* operator software budget; § 8 Abs. 8 grant up to €12k/facility at 40 % co-funding (`reimbursement-routes.md`); RLP § 19a 0.5-FTE credit since 1 Oct 2026 [B]. PNOG fund and § 113e are bills | Voice documentation is taken (voize). Sub-wedge: TI/KIM/ePA onboarding as a service for care homes (50 % with an activated TI card, Apr 2026 [A], `longlist.md`) → small private operators; ~€1–3k/facility one-off + €50–150/month |
| L06 | Hospital clinical workflow | Physicians | Medical director / CIO, private hospital | *Adjacent:* dictation tenders (`pain-professionals.md`). KHZG money has ended | LLM discharge-letter drafting → small private hospital; ~€30–100k/yr |
| L07 | Hospital revenue | Medical controlling, coders | Commercial director / head of medical controlling | *Job:* DKI median €40k planned non-staff spend for MD audits [B] (`hospital-billing-audits.md`) | MD-audit case defence (document check, objection drafting) → private hospital <300 beds; ~€20–40k/yr |
| L08 | Hospital clinical workflow | Social services / discharge team | Head of discharge management / social services | *Job:* discharge platforms (Helios framework, Uniklinik Köln KHZG award [B]). KHZG money has ended | Crowded network product (Recare). A niche (e.g. transition medication list) is untested → hospital; ~€10–30k/yr |
| L09 | Hospital clinical workflow / care operators | Ward and shift managers | Nursing director / HR, care operator or hospital | *Job:* rostering software (≥10 buyers, `pain-professionals.md`). *Adjacent:* agency premiums not refinanced from 2027 [A] | Internal shift-cover pool app → care operator with 3–10 homes; ~€3–10k/yr |
| L10 | Hospital revenue | Medical controlling; surgical practices | = L07 | *Adjacent:* groupers are mandatory, but KVs hand them out free (A18 notes, not re-opened) | Merge into L07 (F3). Possible 2028 wedge: short-stay flat-rate billing checks |
| L11 | Single (employers) | HR, foreign-trained staff | HR director, hospital or care operator | *Adjacent:* recruiting budgets; fees `[UNVERIFIED]` | Recognition case management as a service → care operator; per-hire fee `[UNVERIFIED]` |
| L12 | Practice admin | Physicians, MFAs | Practice owner | *Job:* practice opex. No observed purchase for form automation | AI pre-fill of insurer/agency requests → practices; ~€30–80/month. Blocked by PVS integration |
| L13 | Practice admin | MFAs, reception | Practice owner | *Job:* AI phone tools at €9–229/month [B] (`pain-professionals.md`) | AI phone assistant → practices; €100–200/month. Commodity |
| L14 | Practice admin / navigation | Patients | KV (116117) / Kassen | *Adjacent:* the €2.9bn TSVG money is paid as physician fees (F2) | None (red team: out) |
| L15 | Patient navigation | Patients | GKV | *Adjacent:* treatment capacity | None. Not product-solvable |
| L16 | Patient navigation | Cancer patients | Kasse care management / PKV benefits | *Adjacent:* BARMER builds in-house [B]; Debeka–iuvando partnership (fee unknown) [B] | Trial-access/orientation service paid by PKV → PKV insurer; fee unknown |
| L17 | Patient navigation | Insured people eligible for screening | (a) Kasse care management; (b) GP / radiology network | *Adjacent:* the statutory benefit pays for the exam, not for outreach | Lung-LDCT eligibility check + referral tool → GP practices or radiology network; ~€50/month or per-referral fee. Unexamined (red team: watch) |
| L18 | Patient navigation | Rare-disease patients | Pharma (orphan patient finding) | *Job:* pharma patient-finding spend `[UNVERIFIED]` | Out for this founder (needs a clinical co-founder) |
| L19 | Single | Insured ePA users | Kassen IT providers | *Adjacent:* ident vendors (Nect for BARMER, A18 notes, not re-opened) | Exclude (same rule as S6) |
| L20 | Single | Pharmacy staff | Pharmacy owner | *Job:* pharmacy opex. No purchase of a shortage tool observed. A 50-cent fee per shortage exchange is mentioned `[UNVERIFIED]` (search snippet only) | Shortage assistant (alternatives, prescriber query, insurer-rule check) → independent pharmacies; ~€50–150/month |
| L21 | Payer/MD | Kassen claims staff | (a) Kasse head of claims; (b) BPO (IQVIA HSS, SPS) | *Job:* § 302 processing awards (13 awards, `payer-processing.md`) | Document-classification module sold to a BPO, not to a Kasse (red team) → BPO; ~€50–150k/yr |
| L22 | Payer/MD | MD physicians | MD-IT / MD head of hospital audits | *Job:* €88m MD-IT AI framework [A]; external DRG review firms (MD Niedersachsen €2m [A], this file) | Only as a review-services firm or consortium member. Conflicts with L07 |
| L23 | Payer/MD | MD care assessors | MD head of care assessment | *Job:* MD AI PoC budgets (MD RLP 2025, closed [A]) | AI drafting of care-assessment reports → one MD; pilot ≤€50k |
| L24 | Private insurers | PKV claims staff | PKV head of benefits/claims | *Job:* PKV claims processing (>70m invoices/yr [B], `pain-industry.md`). Incumbent IT vendors (adesso; search snippet only) | GOÄ-2028 invoice-check module → mid-size PKV; ~€100–300k/yr |
| L25 | Single | Health-office staff | Head of a local health office (municipal) | *Adjacent:* pact money ends in 2026 | Out (K1: budget not in force from 2027) |
| L26 | Clinical research | Sponsor clinical ops; study sites | Sponsor head of clinical operations / feasibility (DE affiliate) | *Job:* sponsor recruitment budgets. Sites are paid per patient. The 5 % rule exempts sponsors from 2027 [A] (`trial-recruitment-de.md`) | German recruitment and feasibility service + software for 2027+ launches → mid-size sponsor; ~€50–200k per trial |
| L27 | Clinical research | Study nurses, CRO start-up teams | CRO start-up lead; site manager | *Adjacent:* site overhead | Site start-up pack (documents, contract templates) → CRO; fee unknown |
| L28 | Regulatory/market access | Market-access teams | Pharma head of market access | *Job:* consultancy spend on JCA [B] (`pain-industry.md`) | AI PICO scoping → small biotech; ~€30–100k per dossier. Needs an HTA co-founder |
| L29 | Regulatory/market access | RA/QA staff | Head of RA/QA, device maker | *Job:* RA consultants and staff [B]; Flinn customers [B] | AI post-market surveillance and literature evaluation for SMEs → device SME with 20–250 staff; ~€10–30k/yr |
| L30 | Clinical research | RWE teams | = L26 | — | Merge into L26 (F3) |

## Table 2: status quo, trigger, first-sale route, K2 example, buyer count
**Direct-award limits** (`scoring.md`):
- statutory insurers, Pflegekassen and MDs: ≤€50k, and the buyer "soll … wechseln";
- Bavarian state/municipal buyers: ≤€100k;
- federal buyers: ≤€50k;
- university hospitals and private, church or municipal-GmbH hospitals: no limit found, `[UNVERIFIED]`.

**K2 example:** a young vendor (≤5 years old at its earliest named sale, sale dated 2021+, per the critic's proposal; not yet a CEO decision) with a named paying customer for this signer type.

| # | Status quo today | Trigger (date; vs Sep 2027) | First-sale route (threshold) | K2 example (vendor, founded, named customer, date, grade) | DE buyer count (DACH) |
|---|---|---|---|---|---|
| L01 | Pflegestützpunkte, Kassen counselling (3 % use, [A] `longlist.md`), portals, heycare | None dated; ageing | Private employer, no procurement | **heycare** (2022 as heynanny [B]): Daimler Truck, Douglas, Vaillant, VW Retail ("laut Unternehmen", Mar 2026) [B]. Passes the age test; the date of the first sale is not shown. Also the competitor | 18,632 legal units with ≥250 employees (2024) [A]. AT/CH not searched |
| L02 | Phone calls, portals, hospital social services | None | — | None searched (red team: out) | — |
| L03 | Kassen's own courses, curendo, PflegeBetreuer | § 45 in force; none dated | Kasse direct award ≤€50k [A] | **Gesundheit von Morgen GmbH (PflegeBetreuer)**: Mobil Krankenkasse (7 May 2026) [B], ZF BKK (9 Jul 2026) [B]. Founding year not found → age test open; fee not stated | 92 Kassen (each runs a Pflegekasse) [A] |
| L04 | Agencies, grey market | None | — | None searched | ~266 agencies (2017) `[UNVERIFIED]`, A18 notes, not re-opened |
| L05 | PC/paper documentation in suites (e.g. Vivendi); voize | RLP § 19a since 1 Oct 2026 [B]; PNOG fund H2 2027 (bill); § 113e 2028 (bill) | Private operators, no procurement; municipal homes ≤€100k (Bavaria) | **voize** (2020): Caritasverband Stuttgart, "Start mit voize: Januar 2022", 5 homes, 700 staff [B]; Kreszentia-Stift München, Jul 2023 [B]. Passes; voize is the leader (S2: criterion 8 ≤ 2) | 16,505 care homes + 15,549 home-care services (15 Dec 2023) [A]. AT/CH not searched |
| L06 | Dictation; in-house LLMs (UKE, Leipzig) [B]; Tandem Health | None dated (KHZG over) | Private hospitals (rules `[UNVERIFIED]`); KIS-vendor channel (T-Systems iMedOne in >250 hospitals, per Tandem [B]) | **None found.** Tandem Health (2023, Telekom investment Oct 2026) names no DE hospital [B] | 1,807 hospitals: 529 public, 549 non-profit, 729 private (2025) [A] |
| L07 | Tiplu/LOGEX, ID Berlin, Dedalus, calliora, in-house staff | Audit quotas 1 Jan 2027, **before** Sep 2027 | Private hospitals direct; public tenders need references (Charité, Lausitz) | **None found.** calliora (2023) names no hospital (2 searches) | 1,603 hospital IKs in the audit statistics [A] (`hospital-billing-audits.md`); 1,807 hospitals [A] |
| L08 | Recare, Pflegeplatzmanager, phone/fax | None dated | Hospital tenders (KHZG ended); KIS channel | **Recare**: Uniklinik Köln (tender, 7 Nov 2023) [B]; 12 Knappschaftskliniken via Telekom (Apr 2023) [B]. Founding year not verified → age test open; leader | 1,807 hospitals [A] |
| L09 | Rostering suites, WhatsApp groups, agencies | Pflegebudget overruns not refinanced from 2027 [A] | Private operators direct | **CrewLinQ**: ">100 Pflegeeinrichtungen" use its matching daily (ConSozial 2025 entry) [B]. No named customer; founding year 2021 only from an aggregator `[UNVERIFIED]` | 1,807 hospitals + 16,505 care homes [A] |
| L10 | Groupers, KV billing | Kurzzeitfallpauschalen 2028 (bill; Bundesrat 20 Nov 2026), **after** Sep 2027 | = L07 | Not searched (merge) | = L07 |
| L11 | Recruiters, Länder authorities | None dated | Private employer | Not searched (A24 test 10) | = L09 employers |
| L12 | Manual forms; PVS | KBV form reform (policy may shrink it) | Self-serve; needs a PVS interface (KV-Connect in "rund 170 PVS", search snippet only) | **None found** (1 search) | ~98,000 practices + ~4,900 MVZ [B] (Hartmannbund 2025) |
| L13 | MFAs on the phone; 10 AI vendors incl. Doctolib | None dated | Self-serve, no procurement | **None named.** Doctolib bought aaron.ai (22 May 2024) [B]; fonio testimonials are unnamed [B] | ~98,000 + ~4,900 [B] |
| L14 | 116117, Doctolib | GeDIG (draft) | — | None (out) | — |
| L15 | — | — | — | None (out) | — |
| L16 | Kassen in-house (BARMER), DiGA (Mika) | None dated | PKV is private; Kasse ≤€50k | **Fails age test:** iuvando Health (2019 [B]) × Debeka (22 Oct 2025) [B]; fee not stated | 92 Kassen [A]; 39 PKV full members [B] |
| L17 | GP counselling after training; KV-approved radiologists; no central invitation for lung (search snippet only) | Lung LDCT benefit since Apr 2026, **before** Sep 2027 | Practices self-serve; Kasse ≤€50k | **None found** (1 search) | ~98,000 practices [B]; radiology sites with approval `[UNVERIFIED]` |
| L18 | Rare-disease centres | Genome pilot | Pharma vendor qualification | Not searched (out) | >30 centres [A] (`longlist.md`) |
| L19 | Kassen apps, Nect ident | — | — | Not searched (exclude) | 92 Kassen [A] |
| L20 | Wholesaler queries, Apo-Mall "Bestell-Engel" (two pharmacists, ~1,100 users, Mar 2025) [B], ERP features | No dated rule. Exchange freedom runs to 1 Jul 2028 (search snippet only) | Self-serve, private | **None found** (3 searches). Apo-Mall was built by two pharmacist-wholesalers, not an independent startup | 16,601 pharmacies (end-2025) [B] (`longlist.md`) |
| L21 | IQVIA HSS, SPS, in-house; AOK Hessen takes content checks back in-house from 1 Aug 2026 (search snippet only) | Admin-cost cap from 2027 [A] | Kasse ≤€50k + § 80 SGB X notice; tenders need ISO 27001 + references; TechBoost needs completed B2B projects [B] | **None found.** No BPO–startup partnership found (2 searches) | 92 Kassen [A]; BPOs: a handful (`payer-processing.md`) |
| L22 | MD staff + external review firms | Audit quotas 1 Jan 2027 | MD-IT framework (bids 2 Dec 2026, consortia only); MD review-firm lots (turnover + references) [A] | None | 15 MDs [A] (`payer-processing.md`) |
| L23 | Assessors; Word templates | Volume >3m/yr [A] | MD ≤€50k direct award (inference via § 280 SGB V); TED shows no open MD AI PoC: 9 MD notices with "KI/Künstliche" in the title since 2025 cover 5 procedures (MD Bayern chatbot; MD RLP PoC and its re-tender; MD Nordrhein 2025 award and 2026 tender); MD Nordrhein needs €600k turnover | None found | 15 MDs [A] |
| L24 | In-house claims + IT vendors (adesso, Verisk; search snippets only) | GOÄ planned 1 Jan 2028, **after** Sep 2027 | Private insurer, no procurement law; outsourcing/DORA rules `[UNVERIFIED]` | **None found** (2 searches) | 39 full + 10 extraordinary PKV members [B] (lobby register) |
| L25 | ÖGDigital rollout (BW/BY) (search snippet only) | Pact money ends 2026 | Bavarian municipal ≤€100k; Kulmbach "Digitales Gesundheitsamt" tender got 0 bids (search snippet only) | Not searched (out) | ~375 health offices (2020) [B, stale] |
| L26 | CROs, site networks, TriNetX; MPIRIQ | 5 % rule from 2027 launches [A] | Sponsor vendor qualification (long); site SaaS self-serve | **None found.** MPIRIQ (2024) names no customer [B] | 668 new commercial EU trials with DE sites in 2025 [A] (`trial-recruitment-de.md`); AMNOG count = A24 |
| L27 | CTMS/eISF suites; standard contract clauses | Clauses since Dec 2025 [B] | CRO private | **None found** (1 search) | Sites `[UNVERIFIED]` |
| L28 | HTA consultancies (e.g. Decisive Consulting "PICO Predict"; search snippet only) | ~58 JCAs in 2026 [B] | Pharma vendor qualification | **None found** | ~58 JCAs/yr EU [B] |
| L29 | RA consultants, eQMS, Flinn | MDR revision proposal Dec 2025 (may shrink the pain) | Private manufacturer | **Flinn** (2022 [B]): Paul Hartmann, quoted by its SVP RA (19 Feb 2026) [B]. Passes; leader ($20m Series A, S2) | 1,480 firms >20 staff + ~12,000 micro firms [B] (BVMed Jun 2025) |
| L30 | FDZ (claims data only) | — | = L26 | Not searched (merge) | 53 FDZ applications by Feb 2026 [B] |

## Details
- **Age-test caveat.** The "≤5 years at earliest named sale" reading is the critic's proposal and still awaits a CEO decision. Under "≤5 years old today", only heycare (2022), Flinn (2022) and Tandem Health (2023) are young. voize (2020) would fail.
- **Recare's founding year** was not confirmed. The recaresolutions.com pages returned 404, and the press releases do not state it.
- **Hospital count base.** I use 1,807 hospitals (Destatis 2025) as the total. 1,603 is the number of hospital IKs in the GKV-SV audit statistics, a different unit.
- **Employer count.** 18,632 is the number of legal units with ≥250 employees in all sectors (Destatis business register, reference year 2024). It replaces the ~17,000 estimate in the A18 notes.
- **MD notices.** A TED search for buyer-name "Medizinischer Dienst" from 1 Jan 2026 returns 53 notices. Only MD Nordrhein 762721-2026 is AI software. MD Niedersachsen 383478-2026 is the external review-firm tender.
- **ACV guesses** are anchored where possible:
  - L07 on the DKI median of €40k;
  - L13 on the €9–229/month price lists;
  - L03 and L23 on the €50k direct-award cap.

  All others are inference without an anchor, so B1 should tag them L.

## Gaps / [UNVERIFIED]
- **No price found for any wedge except L13** (public price lists) and the caps above. voize prices on request ("Jetzt Preise anfragen").
- **Founding years not confirmed:** Recare, Gesundheit von Morgen GmbH, CrewLinQ.
- **Unnamed or snippet-only claims:**
  - The St. Josefs-Krankenhaus Potsdam quote in the CrewLinQ PDF appeared in a search summary only.
  - AOK Hessen insourcing: www.aok.de is not resolvable in WebFetch, and curl returns a JS shell.
- **DACH counts:** AT and CH were not verified in this session. The AT figures in the A18 notes (257 hospitals, 1,440 pharmacies) were not re-opened. A CH snippet says 274 hospitals and birth centres reported in 2023 (not opened).
- **Not searched:** L02, L04, L10, L11, L14, L15, L18, L19, L25, L30 (merge/out per red team), plus the A24 tests not covered here (AMNOG count, care-suite AI, nursing recognitions by country).
- **Purchasing rules** of private and municipal-GmbH hospitals below the EU threshold: `[UNVERIFIED]`.

## Sources
- https://www.voize.ai/de/kundengeschichten/caritas-stuttgart — Caritas Stuttgart, start Jan 2022, 5 homes, 700 staff [B], accessed 2026-11-07
- https://www.voize.ai/de/kundengeschichten/kreszentia-stift-muenchen — Kreszentia-Stift, start Jul 2023 [B], accessed 2026-11-07
- https://www.voize.ai/de/blog/rheinland-pfalz-refinanzierung — RLP § 19a: 0.5 FTE credit since 1 Oct 2026, signed 22 Sep 2026 [B], accessed 2026-11-07
- https://www.voize.ai/de/preise — licence per person cared for; price on request [B], accessed 2026-11-07
- https://www.munich-startup.de/en/news/heycare-raises-4-million-euros-in-growth-capital — heycare founded 2022 as Heynanny; customers Daimler Truck, Douglas, Vaillant, VW Retail; profitable [B], accessed 2026-11-07
- https://www.trendingtopics.eu/heycare-hr-tech-startup-sichert-sich-4-millionen-euro-fuer-rundum-care-plattform/ — heycare founders, 2022, customers, Mar 2026 [B], accessed 2026-11-07
- https://www.zfbkk.de/en/news/details/online-nursing-courses — ZF BKK × Gesundheit von Morgen GmbH, 9 Jul 2026 [B], accessed 2026-11-07
- https://mobil-krankenkasse.de/unternehmen/presse/pressemeldungen/Pflegebetreuer.html — Mobil Krankenkasse × Gesundheit von Morgen GmbH, 7 May 2026 [B] (opened in A20; re-confirmed by search result), accessed 2026-11-07
- https://www.lisavienna.at/news/detail/flinn-receives-20-million-to-automate-the-product-lifecycle-in-medtech-and-pharma-with-ai/ — Flinn customers Carl Zeiss, Philips, Paul Hartmann; Hartmann SVP quote; 19 Feb 2026 [B], accessed 2026-11-07
- https://tech.eu/2022/12/20/n26/ — Flinn "formed earlier this year" (2022), Vienna [B], accessed 2026-11-07
- https://www.medconweb.de/blog/wp-content/uploads/2023/11/PM_Uniklinik-Koeln-digitalisiert-mit-Recare.pdf — Uniklinik Köln chooses Recare in a KHZG tender, 7 Nov 2023 [B], accessed 2026-11-07
- https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2023/04/knappschaftskliniken — 12 Knappschaftskliniken use Telekom + Recare [B], accessed 2026-11-07
- https://edge.sitecorecloud.io/nurnbergmes0e18-nmmultisite6e34-prod50da-6065/media/Project/NuernbergMesse/ConSozial/PDFs/Sozialer-Innovationspreis/2025/CrewLinQ-GmbH.pdf — CrewLinQ: ">100 Pflegeeinrichtungen", no named customer [B], accessed 2026-11-07
- https://www.telekom.com/en/newsroom/latest-updates/media-information/2026/10/telekom-invests-in-tandem-health — Tandem Health: >10,000 facilities in 14 countries incl. Germany; ISO 27001, C5, MDR CE [B], accessed 2026-11-07
- https://www.trendingtopics.eu/tandem-health-telekom-lg-norrsken/ — Tandem founded 2023 in Stockholm; T-Systems KIS in >250 clinics [B], accessed 2026-11-07
- https://techboost.telekom.com/public/startups?lang=en — TechBoost intake: programme requires a marketable product and completed B2B customer projects; Connect requires an MVP + register entry [B], accessed 2026-11-07
- https://www.munich-startup.de/news/mpiriq-7-fragen — MPIRIQ interview; no named paying customer [B], accessed 2026-11-07
- https://www.cash-online.de/a/digitale-unterstuetzung-fuer-krebspatienten-kooperation-zwischen-debeka-und-iuvando-health-705194/ — Debeka × iuvando Health, 22 Oct 2025 [B], accessed 2026-11-07
- https://www.uni-heidelberg.de/en/node/48623 — iuvando Health founded 2019 [B], accessed 2026-11-07
- https://www.apotheke-adhoc.de/nachrichten/detail/apothekenpraxis/grosshandelsapotheker-entwickeln-bestellplattform/ — Apo-Mall "Bestell-Engel", ~1,100 users, 6 Mar 2025 [B], accessed 2026-11-07
- https://www.aerzteblatt.de/nachrichten/151593/Doctolib-uebernimmt-Telefonassistenten — Doctolib acquires aaron.ai, 22 May 2024 [B], accessed 2026-11-07
- https://www.fonio.ai/de/ki-telefonassistenten/ki-telefonassistent-arztpraxis — fonio practice page; unnamed testimonials [B], accessed 2026-11-07
- https://api.ted.europa.eu/v3/notices/search — TED 383478-2026 (MD Niedersachsen external DRG review firms: ~20,000 orders, €2m, 4 × €500k, turnover + references, deadline 3 Jul 2026); MD notice counts 2025–26; 762721-2026 [A], accessed 2026-11-07
- https://www.destatis.de/DE/Presse/Pressemitteilungen/2026/10/PD26_376_231.html — 1,807 hospitals (529 public, 549 non-profit, 729 private), 2025 [A], accessed 2026-11-07
- https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Gesundheit/Pflege/Tabellen/pflegeeinrichtungen-deutschland.html — 16,505 care homes, 15,549 home-care services (15 Dec 2023) [A], accessed 2026-11-07
- https://www.kbv.de/infothek/zahlen-und-fakten/gesundheitsdaten/pflegeheime-und-personal — 42 % of care homes private (2023) [B], accessed 2026-11-07
- https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/Unternehmensregister/Tabellen/unternehmen-beschaeftigtengroessenklassen-wz08.html — 18,632 legal units with ≥250 employees (2024) [A], accessed 2026-11-07
- https://www.hartmannbund.de/wp-content/uploads/2025/11/2025-HV_Praxen-bleiben-unverzichtbare-Saeule-der-Versorgung.pdf — ~98,000 practices, ~4,900 MVZ [B], accessed 2026-11-07
- https://www.gkv-spitzenverband.de/service/krankenkassenliste/krankenkassen.jsp — "92 Ergebnisse (Stand: 07.11.2026)" [A], accessed 2026-11-07
- https://www.lobbyregister.bundestag.de/media/41/99/707149/Lobbyregister-Registereintraege-Detailansicht-R000815-2026-03-17_15-55-23.pdf — PKV-Verband: 39 full + 10 extraordinary members [B], accessed 2026-11-07
- https://kommunalwiki.boell.de/index.php/Gesundheitsamt — ~375 health offices (2020) [B, stale], accessed 2026-11-07
- https://www.bvmed.de/download/positionspapier-medtech-kmu — 1,480 medtech firms >20 staff, ~12,000 micro [B], accessed 2026-11-07
- WebSearch, snippet only (not used as fact): AOK Hessen insourcing from 1 Aug 2026 (aok.de); IQVIA GKV AI PoCs (Nov 2025 article); adesso/Verisk PKV claims tools; KV-Connect in ~170 PVS; 50-cent shortage fee; Kulmbach ÖGD tender 0 bids; LÄKH "no central invitation" for lung screening; Decisive Consulting PICO Predict; CH 274 hospitals 2023.
