# Parked-ideas screen: L07, L06, L03, L13, L29 on payer, price, customers and cash
Task: C6 | Date: 2026-11-14 | Status: draft

Method: the test that stopped L01 (`research/reviews/2026-11-13-redteam-eldercare-navigator-brief.md`, `-C4.md`): strict K1 (the wedge's signer pays for this job), strict K2 (a named young vendor was paid, or an open route), customers × **sourced** price for three salaries and for €1m ARR, cash to month 24, incumbents and free substitutes, founder access, cheapest test. Facts carried over from earlier files are marked "(repo)" with the file; everything else was opened in this run. All arithmetic is my own (*my math*). **Salary assumption (not sourced, same as the L01 brief):** €60,000 employer cost per person; three people = €180,000 a year.

## Findings
- **No parked idea passes as a venture case for this founder today. One passes the arithmetic: L07 (hospital MD-audit defence).** At the two sourced price points (€40,000 DKI median of planned spend [B]; €60,600 a year, UK Frankfurt coding-revision award [A]), three salaries need **3–5 hospitals** and €1m ARR needs **17–25** (*my math*). The L01 equivalents were 31–51 and 167–279. L07 fails on access, not on size: every public award for AI coding software in 2025–26 went to the incumbent Tiplu (LMU Klinikum, UK Würzburg €545,250, MU Lausitz) [A]. Lausitz required **≥€1m a year turnover in the field**, and Klinikum Stuttgart's market sounding asks for a cross-hospital ML network and "hohe Marktdurchdringung" in university hospitals [A] ([TED API](https://api.ted.europa.eu/v3/notices/search): 57060-2025, 278914-2025, 552501-2026, 214386-2026, 515360-2026). Tiplu now belongs to LOGEX (press release on Thoma Bravo's site, 8 Jul 2026) [B]. The Munich rival calliora ($6m pre-seed, Max Planck AI PhDs) still names no hospital [B].
- **L13 (AI phone assistant for practices) passes K1 and the count test, but the price is collapsing.** October 2026 price lists: €69–229 a month (10 vendors) [B] ([medizinio](https://medizinio.de/digitalisierung/telefonassistent-arztpraxis)). The web host IONOS sells a flat rate for **€99 a month, all calls** (blog price table, 13 Nov 2026) [B]. fonio (founded autumn 2024) reached **>7,000 customers** and "knapp unter 7 Millionen Dollar" ARR, and raised €14.6m (Jun 2026) [B] ([Trending Topics](https://www.trendingtopics.eu/fonio-ai-bewertung-steigt-auf-120-millionen-euro-146-mio-euro-in-der-seed-runde/)). *My math:* ≈$1,000 a year per customer. €1m ARR would take **419–842 practices**. It is a good founder-skill test, not a venture for a new entrant.
- **L03 (§ 45 online carer course for Pflegekassen) is too small to stand alone.** Care courses have their own account line. One statutory Pflegekasse (SVLFG) spent **€52,792.33** on "Pflegekurse" in Q1 2026, against €254.9m in benefits [A] ([PV45](https://cdn.svlfg.de/fiona8-blobs/public/svlfgonpremiseproduction/73990c18040c7332/4cfb9404ff71/pv45-2026-01.pdf)). Scaled to the 2025 national benefit spend of €70.42bn [A] ([BMG](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Statistiken/Pflegeversicherung/Finanzentwicklung/03-Finanzentwicklung-der-sozialen-Pflegeversicherung__2025.pdf)), that is **≈€14.6m a year for all carer courses**, in person and online (*my math, one Kasse, rough*). Online courses are already free to carers through curendo and PflegeBetreuer [B].
- **L06 (LLM discharge letters) has no shown purchase and a giant in the job.** The one tender (Harzklinikum, KHZG) still has **no award notice 15 months later** [A]. Microsoft's Dragon Copilot has been "allgemein verfügbar" for German clinics since 7 Oct 2025 and drafts "Epikrisen oder Arztbriefe"; five German hospitals piloted it [B] ([Microsoft](https://news.microsoft.com/de-de/nach-erfolgreicher-pilotphase-microsoft-dragon-copilot-fuer-deutschlands-kliniken-und-praxen-ab-sofort-allgemein-verfuegbar/)).
- **L29 (AI post-market surveillance for device SMEs) passes K1/K2, but the leader holds the wedge and the law may shrink the pain.** Flinn (2022): "Trusted by 200+ global MedTech & IVD Leaders" [B] ([flinn.ai](https://www.flinn.ai)). No price was found. The Commission's Dec 2025 proposal would cut PSUR updates for class IIb/III devices from yearly to every two years after year 1. It is not adopted [B] ([Arthur Cox](https://www.arthurcox.com/knowledge/mdr-ivdr-overview-of-the-commissions-december-2025-proposed-amendments/)). The core skill is regulatory affairs, so founder fit is 2.
- **A cross-cutting cost:** providers, Kassen and their processors may process health data in the cloud only with a **C5 attestation** (Type 1 for the first 18 months after launch, then Type 2) [A] ([§ 393 SGB V](https://www.gesetze-im-internet.de/sgb_5/__393.html)). This applies to L06, L07 and L13 (and L03 if hosted). The audit cost was not found `[UNVERIFIED]`.

## Ranked table (inference on sourced inputs)
| Rank | Idea → first buyer | K1 strict | K2 strict | Sourced price | Customers for 3 salaries / €1m ARR (*my math*) | Reachable? | Verdict |
|---|---|---|---|---|---|---|---|
| 1 | **L07** MD-audit defence → independent private hospital | **Pass** (4 public awards for the job 2024–26 [A]; DKI spend [B]) | **Unproven** (calliora unnamed; Tiplu >5 years old; public route needs ≥€1m turnover) | €40,000 (DKI median, acquisition + running) [B]; €60,600/yr (UK Frankfurt) [A] | **3–5 / 17–25** | Count yes (729 private hospitals [A], repo). Access: only with a medical-controlling co-founder and a niche Tiplu/calliora do not cover | **Cheap test first** (co-founder access + wedge check), then brief |
| 2 | **L13** AI phone → practice | Pass (2 paying practices, 2024 [B], repo; 10 public price lists [B]) | Unproven (fonio 2024 paid but no named practice; One100 "zehn Einrichtungen", unnamed) | €69–229/month [B]; IONOS €99 flat [B] | **75–152 / 419–842** | Count plausible (~103k practices [B], repo); price and channel held by CGM, Doctolib, fonio, IONOS | **Cheap test** (founder-skill project), **no venture brief** |
| 3 | **L03** § 45 course → Pflegekasse | Budget line passes [A]; **price not shown** | Unproven (Gesundheit von Morgen: age and fee unknown) | None; only the €50,000 direct-award cap [A] | 4 / 20 at the cap | Pool ≈€14.6m/yr for all courses; free substitutes | **Drop** as a company; at most an add-on |
| 4 | **L29** AI PMS → device SME | Pass (Flinn × Hartmann [B], repo) | Pass (Flinn 2022) = also the leader | **None found** | 6–18 / 34–100 at an unsourced €10–30k | Flinn claims 200+ customers; PSUR cycle may halve | **Drop** unless an RA co-founder appears |
| 5 | **L06** LLM letters → hospital | **Weak** (1 tender, no award) | Unproven | **None found** | 2–6 / 10–34 at an unsourced €30–100k | Microsoft, KIS vendors, Tandem/Telekom, in-house builds | **Drop** |

## Details

### Cash to month 24 (same frame for all; *my math*, my assumptions)
- **Cost:** three people for 24 months = €360,000, before tools, insurance, legal and C5 costs.
- **Money in sight** (repo, `research/munich-ecosystem.md` [A]):
  - €10,000 own funds.
  - EXIST, best case: 3 × €2,500 × 12 = €90,000 in stipends + €30,000 material costs. It needs no active job (sabbatical allowed), a German Hochschule host and an "innovative" project.
  - Start?Zuschuss!: 50 % of costs, max €36,000, after incorporation.
  - Total ≤ €166,000.
- **Reading:** if EXIST pays year 1, year 2 needs about **€150,000 in collected revenue** (€180,000 − €36,000 + other costs) or a pre-seed round.
  - L07: 3 hospitals at ~€50,000 that pay from month 12.
  - L13: ~63–125 practice-years in year 2. On a linear ramp, that means ending month 24 with ~125–250 paying practices.
  - L03: 3 Kassen at the €50,000 cap.
  - L06 and L29: no sourced price, so no reading.
- Without EXIST (the CEO stays employed until Sep 2027) nobody is paid until revenue or a round arrives.
- Hospital sales-cycle length was not found `[UNVERIFIED]`. *Inference:* L07 is the only idea where a handful of contracts closes the gap. It is also the idea with the longest buyer cycle.

### L07: MD-audit case defence → private hospital <300 beds
1. **Signer and price.** Head of medical controlling or commercial director; hospital opex, no procurement for private hospitals (repo, `hospital-billing-audits.md`).
   - Public awards for the job [A] (TED API, `winner-name`, `tender-value`, `duration-period-*`):

   | Notice | Buyer | Winner | Value / term |
   |---|---|---|---|
   | 57060-2025 (Jan 2025) | LMU Klinikum: "MD-sicheres Kodieren" with AI, "zur Sicherheit eines möglichen Prüfverfahrens nach § 275 SGB V" | Tiplu GmbH | not published |
   | 278914-2025 (Apr 2025) | UK Würzburg, automated coding | Tiplu GmbH | €545,250 (`tender-value`); term not in the API |
   | 552501-2026 (Aug 2026) | MU Lausitz, same scope | Tiplu GmbH | 60 months; value withheld (−1) |
   | 515360-2026 (Jul 2026, prior information) | Klinikum Stuttgart, AI coding | (market sounding) | — |

   - Klinikum Stuttgart's sounding looks for a broad "klinikübergreifenden Machine-Learning-Netzwerk" and requires "eine hohe Marktdurchdringung, insbesondere in Krankenhäusern der Maximalversorgung und Universitätskliniken".
   - Lausitz eligibility (214386-2026): annual turnover in the field "mind. 1.000.000 EUR"; liability cover €5m / €1m.
   - Older anchors (repo): UK Frankfurt €181,800 / 3 years (*my math:* €60,600 a year); DKI median €40,000 of "Sachkosten für Anschaffung und laufende Kosten" [B]; Dr. Baller (service firm) won UK Frankfurt's €360,000 coding-support framework [A].
   - **K1: pass. K2: unproven.** No ≤5-year-old vendor with a named hospital. calliora (2023) says "Private, kirchliche und öffentliche Häuser in fünf Bundesländern arbeiten im Alltag mit calliora" (interview, 6 Oct 2026), but names none [B] ([startupvalley](https://startupvalley.news/de/calliora-krankenhaeuser-ki-plattform/), [calliora.com](https://www.calliora.com), 2 searches).
2. **Customers × price.** 3 salaries: €180,000 / €60,600 = 3; / €40,000 = 4.5 → **3–5 hospitals**. €1m ARR: 17–25 hospitals. Buyer pool: 729 private hospitals [A] (repo). How many are independent of the chains (Helios, Asklepios, Sana …), which buy centrally, was **not counted** `[UNVERIFIED]`.
3. **Cash.** Best fit to the frame above: three contracts close year 2. Pilots in a hospital need the C5 attestation if the tool is cloud-hosted (§ 393 SGB V) [A], or an on-premise install.
4. **Incumbents and law.**
   - Tiplu: wins the public tenders; "MBEG-Assistent" in about 30 hospitals (repo) [B]; acquired by LOGEX (signed 8 Jul 2026) [B] ([Thoma Bravo](https://www.thomabravo.com/press-releases/logex-healthcare-analytics-ag-acquires-tiplu-gmbh)).
   - calliora (Munich, $6m) [B]; ID Berlin, Dedalus, Solventum (repo).
   - Law: the 2027 quotas are enacted. The 1 % tier awaits the Bundesrat on 20 Nov 2026; the BMG report on quotas is due 31 Dec 2026 (repo, A17). A rule change in either direction moves demand.
5. **Founder access.** Buyer: head of medical controlling. Required co-founder: a medical controller or coding specialist (DKI: ~4,000 FTE nationally, repo). Not answered by the CEO yet.
6. **Cheapest test.**
   - (a) CEO, 10 minutes: name one medical controller or coder who might co-found.
   - (b) Desk, one run: count independent private hospitals with ≥1 completed MD audit per quarter (GKV-SV XLSX × Destatis ownership). Also find what small houses pay external MD-defence services, e.g. per-case or success fees. None found in one search, which is the price a service-first wedge would need.

### L13: AI phone assistant → practice
1. **Signer and price.** Practice owner; self-serve, no procurement. Price lists, "Datenstand: Herstellerangaben, Oktober 2026" [B] ([medizinio](https://medizinio.de/digitalisierung/telefonassistent-arztpraxis)):
   - Doctolib (aaron.ai): €192.44 net per physician, only inside a bundle;
   - CGM ONE: €199 per site, 12 months;
   - Mediform Medivoice: €75 + €0.15/min;
   - 321 MED: €69;
   - PraxisConcierge: €149 + modules;
   - docmedico: €79.95;
   - fonio: €99;
   - VITAS: €49 + €0.28 per conversation;
   - Eterno Connect: €9 standalone.

   IONOS All-Flat €99 a month for all calls [B, blog price table dated 13 Nov 2026] ([kopfundstift](https://kopfundstift.de/ki-telefonassistent-kosten/)). **K1: pass** (repo: two paying practices, Ärzteblatt 7/2024).
   **K2: unproven on a named practice:**
   - fonio: founded autumn 2024, ">7.000 Kund:innen", mostly firms "mit 10 bis 100 Mitarbeitern", no practice named [B];
   - One100 (Vienna, 2026): "bereits bei zehn Einrichtungen im Einsatz"; target ">300 Praxen" by end of 2026 [B] ([Trending Topics, 11 Feb 2026](https://www.trendingtopics.eu/one100/));
   - Sinalis (Munich, TUM.ai hackathon): funded by a €10,000 prize, applying for grants [B] ([Munich Startup, 14 Jan 2026](https://www.munich-startup.de/news/pitch-and-people-sinalis)).
2. **Customers × price.** At €99–199 a month (€1,188–2,388 a year): 3 salaries = **75–152 practices**; €1m ARR = **419–842**. Pool ~98,000 practices + ~4,900 MVZ [B] (repo).
3. **Cash.** Cheap to build; the risk is churn and price. Repo: one practice cancelled after 2 of 10 calls were handled.
4. **Incumbents.** The PVS owners bundle it (CGM; Doctolib since buying aaron.ai). A horizontal leader is funded (fonio: €14.6m seed at a €120m valuation, >€20m in total) [B]. IONOS sells it to every small business. From 2 Aug 2026 the AI Act's Art. 50 transparency duty applies (secondary source only, `[UNVERIFIED]`).
5. **Founder access.** Practice owners are reachable without procurement. This is the CEO's own skill (AI agents).
6. **Cheapest test.** Build one specialty voice agent with one PVS integration as a side project; count paying practices after 3 months. It tests the founder, not a venture.

### L03: § 45 SGB XI online carer course → Pflegekasse
1. **Signer and price.** Head of care services at a Pflegekasse. § 45 lets the Kasse run courses itself or commission "geeignete andere Einrichtungen" [A] (repo, `§ 45`). Courses are free to carers.
   - No fee is published for PflegeBetreuer (Mobil Krankenkasse, 7 May 2026; ZF BKK) [B] ([Mobil Krankenkasse](https://mobil-krankenkasse.de/unternehmen/presse/pressemeldungen/Pflegebetreuer.html)).
   - **K1: budget line passes, price not shown.**
2. **Customers × price.** Only the direct-award cap of €50,000 is sourced (§ 22 SVHV [A], repo): 4 Kassen for salaries, 20 for €1m ARR. The whole national pool for all carer courses is ≈€14.6m a year (*my math:* SVLFG Q1 2026 Pflegekurse €52,792.33 / benefits €254,940,956.39 = 0.0207 %; × €70.42bn = €14.6m). One rural Kasse is a weak base, so read this as an order of magnitude. €1m ARR would be ~7 % of all course spending for one online vendor.
3. **Cash.** 3 Kassen at the cap would close year 2, but no Kasse is shown paying near €50,000.
4. **Incumbents and substitutes.**
   - curendo: "Kostenfrei dank Übernahme durch Ihre Pflegekasse", advertised on pflege.de [B] ([pflege.de](https://www.pflege.de/pflegende-angehoerige/pflegewissen/pflegeberatung/pflegekurse/)).
   - PflegeBetreuer [B]; Kassen's own courses.
   - The PNOG bill would add statutory counselling duties (repo, L01 brief).
5. **Founder access.** Kasse department heads. Not answered.
6. **Cheapest test.** One desk run: ask Kassen tender portals and the GKV-SV for § 45 online-course awards with values. If none above €20,000 a year, close the row.

### L29: AI post-market surveillance / literature → device SME
1. **Signer and price.** Head of RA/QA. Flinn × Paul Hartmann (repo [B]); Flinn's site: "Trusted by 200+ global MedTech & IVD Leaders" and a Dentsply Sirona customer story listed in its sitemap [B] ([flinn.ai](https://www.flinn.ai)). **No price found** (2 searches; consultancies such as NAMSA quote on request; Freyr sells templates only).
   - **K1 and K2: pass.** But the K2 vendor is the category leader.
2. **Customers × price.** Only the A18 guess of €10–30k (unsourced): 6–18 SMEs for salaries, 34–100 for €1m ARR. Pool: 1,480 firms >20 staff [B] (repo).
3. **Cash.** Not computable without a price.
4. **Incumbents and law.**
   - Flinn ($20m), Greenlight Guru, Ketryx, Enzyme (snippet only); RA consultancies.
   - The Commission proposal of 16 Dec 2025 would end automatic 5-year certificate expiry and move PSUR updates for IIb/III to every two years after year 1. It is before Parliament and Council, not adopted [B] (Arthur Cox, 19 Mar 2026).
5. **Founder access.** Needs an RA co-founder; the core is regulatory expertise (fit 2).
6. **Cheapest test.** None worth running unless an RA co-founder candidate exists.

### L06: LLM discharge-letter drafting → hospital
1. **Signer and price.** Medical director or CIO. One tender: Harzklinikum "LLM-basierte Arztbriefschreibung", KHZG project 4.01, framed as a decision-support system (TED 492877-2025). A re-query on 14 Nov 2026 shows no award under the buyer [A].
   - Adjacent purchases are speech recognition, not LLM letters, all won by incumbents [A]: Saarland €587,575 to Solventum; Mittweida €424,701 to Grundig (Dragon Medical One); BG Klinikum Hamburg €480,884 to 4voice.
   - Caritas Gesundheit Berlin direct-awarded "KI-basierte Sprachdokumentation" for nursing (VEAT 366802-2026; winner not in the API) [A].
   - **K1: weak. K2: unproven.** No price.
2. **Customers × price.** Only the A18 guess of €30–100k (unsourced).
3. **Cash.** Not computable. Extra costs:
   - MDR: software that acts on data beyond storage, communication or simple search "may be" medical device software (MDCG 2019-11 rev. 1, Jun 2025) [A] ([MDCG](https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=mdcg_2019_11_en.pdf)). Harzklinikum itself calls its purchase decision support.
   - C5 attestation for cloud hosting (§ 393 SGB V) [A].
4. **Incumbents.** Microsoft Dragon Copilot (available in Germany since 7 Oct 2025; piloted at Charité and hospitals in Mannheim, Stuttgart, Halle and Hannover) [B]; KIS vendors (Dedalus, CGM, Telekom); Tandem Health (Telekom-backed, repo); in-house at UKE and Leipzig (repo).
5. **Founder access.** Needs clinical and KIS-integration co-founders (fit 3).
6. **Cheapest test.** None recommended.

### Desk tests from A24/A26 that bear on these rows
| Test | Result (14 Nov 2026) | Grade |
|---|---|---|
| calliora named hospital (A24) | None found (3 searches + site + Oct 2026 interview) | — |
| L07 independent private hospitals with ≥1 MD audit/quarter (A26) | **Not run**: GKV-SV XLSX has no ownership field; needs a Destatis match | — |
| L03 price of a Kassen-funded online course (A26) | None found; national course pool ≈€14.6m/yr (inference) | [A] data |
| L13 young vendor with a named practice (B1 open check) | None named (fonio, One100, Sinalis, Mediform checked) | [B] |
| L13 funding of top vendors (B1 open check) | fonio €14.6m seed (Jun 2026); Doctolib owns aaron.ai (repo); Mediform €1.5m (May 2025, snippet only, page 403) | [B] / snippet |
| L06 private-chain LLM-letter purchase (B1 open check) | None found; Microsoft GA; Harzklinikum unawarded | [A]/[B] |

## Recommendation (inference)
- **Do not write a second full brief yet.** Run two cheap steps first, both under one hour of CEO time:
  - (1) The CEO names whether he can reach a medical controller or coder as a co-founder candidate (10 minutes).
  - (2) One desk run on an L07 wedge Tiplu and calliora do not serve: independent small private hospitals, service-first (AI-assisted MD-objection drafting sold per case or as a retainer). Count the buyers, find a sourced service price, check the 20 Nov Bundesrat result and the Q3 data (A17).
- If (1) is "no one": L07 is not achievable for this founder. **Return to the long list** and run this same customers × price screen on the other 22 rows before picking again.
- L13 is worth doing only as a hands-on skill test (cheap, the CEO's own craft), not as the venture.
- Drop L03, L06 and L29 as standalone ideas.

## Gaps / [UNVERIFIED]
- Hospital IT sales-cycle length; cost of a C5 attestation; number of independent (non-chain) private hospitals.
- No sourced price for L06, L29 or L03. L07's €40,000 is acquisition + running cost (not annual); €60,600 is a university hospital.
- UK Würzburg's €545,250: contract term not in the API, so no annual figure.
- Mediform €1.5m (May 2025): search snippet only (startbase 403).
- AI Act Art. 50 transparency from 2 Aug 2026 and the Greenlight Guru, Ketryx and Enzyme competitor list: search snippets only.
- The SVLFG ratio is one rural Kasse; the €14.6m national figure is an order-of-magnitude inference.
- The MDR revision text was read through a law-firm summary (Arthur Cox), not EUR-Lex.
- Tandem's German customer story (Rheumazentrum Mittelhessen): page returned 404 in WebFetch, not used.
- Not checked: Austrian/Swiss markets; the founder's own access (CEO question).

## Sources
- https://api.ted.europa.eu/v3/notices/search — 57060-2025 (LMU, Tiplu), 278914-2025 (Würzburg, Tiplu, €545,250), 214386-2026 / 552501-2026 (Lausitz: ≥€1m turnover, 60 months, Tiplu), 515360-2026 (Stuttgart PIN: market penetration requirement), 492877-2025 (Harzklinikum, no award), 366802-2026 (Caritas VEAT), 822217-2025, 349501-2025, 162629-2025 (speech recognition awards) [A], accessed 2026-11-14
- https://www.thomabravo.com/press-releases/logex-healthcare-analytics-ag-acquires-tiplu-gmbh — LOGEX to become sole shareholder of Tiplu, 8 Jul 2026 [B], accessed 2026-11-14
- https://startupvalley.news/de/calliora-krankenhaeuser-ki-plattform/ — calliora interview, 6 Oct 2026: hospitals in five states, unnamed; Max Planck founders [B], accessed 2026-11-14
- https://www.calliora.com — no customer named, demo form only [B], accessed 2026-11-14
- https://medizinio.de/digitalisierung/telefonassistent-arztpraxis — 10 AI phone vendors, prices, data as of Oct 2026 [B], accessed 2026-11-14
- https://kopfundstift.de/ki-telefonassistent-kosten/ — IONOS, VITAS, fonio price table, 13 Nov 2026 [B, blog], accessed 2026-11-14
- https://www.trendingtopics.eu/fonio-ai-bewertung-steigt-auf-120-millionen-euro-146-mio-euro-in-der-seed-runde/ — fonio founded autumn 2024, >7,000 customers, ARR just under $7m, €14.6m seed, 9 Jun 2026 [B], accessed 2026-11-14
- https://www.trendingtopics.eu/one100/ — One100: ten facilities, target >300 practices by end of 2026, 11 Feb 2026 [B], accessed 2026-11-14
- https://www.munich-startup.de/news/pitch-and-people-sinalis — Sinalis, Munich, €10,000 prize money, 14 Jan 2026 [B], accessed 2026-11-14
- https://cdn.svlfg.de/fiona8-blobs/public/svlfgonpremiseproduction/73990c18040c7332/4cfb9404ff71/pv45-2026-01.pdf — SVLFG PV45 Q1 2026: account 04510 Pflegekurse €52,792.33; benefits €254,940,956.39 [A], accessed 2026-11-14
- https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Statistiken/Pflegeversicherung/Finanzentwicklung/03-Finanzentwicklung-der-sozialen-Pflegeversicherung__2025.pdf — SPV benefits 2025 €70.42bn; no national course line [A], accessed 2026-11-14
- https://mobil-krankenkasse.de/unternehmen/presse/pressemeldungen/Pflegebetreuer.html — PflegeBetreuer online courses free to insured, no fee stated (via search result text; page carried over from repo) [B], accessed 2026-11-14
- https://www.pflege.de/pflegende-angehoerige/pflegewissen/pflegeberatung/pflegekurse/ — curendo online course "Kostenfrei dank Übernahme durch Ihre Pflegekasse" [B], accessed 2026-11-14
- https://news.microsoft.com/de-de/nach-erfolgreicher-pilotphase-microsoft-dragon-copilot-fuer-deutschlands-kliniken-und-praxen-ab-sofort-allgemein-verfuegbar/ — Dragon Copilot GA in Germany, 7 Oct 2025; Arztbriefe; pilot hospitals [B], accessed 2026-11-14
- https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=mdcg_2019_11_en.pdf — MDCG 2019-11 rev. 1 (Jun 2025), software qualification steps [A], accessed 2026-11-14
- https://www.gesetze-im-internet.de/sgb_5/__393.html — § 393 SGB V: C5 attestation for cloud processing of health data (Type 1 for 18 months, then Type 2) [A], accessed 2026-11-14
- https://www.flinn.ai — "Trusted by 200+ global MedTech & IVD Leaders"; Dentsply Sirona story in sitemap [B], accessed 2026-11-14
- https://www.arthurcox.com/knowledge/mdr-ivdr-overview-of-the-commissions-december-2025-proposed-amendments/ — MDR proposal 16 Dec 2025: PSUR every two years for IIb/III, no automatic certificate expiry; not adopted [B], accessed 2026-11-14
- WebSearch, snippets only (not used as fact): Mediform €1.5m (startbase, 403); Flinn competitors (ai.engineer); AI Act Art. 50 date (medizinio vendor page); Freyr/NAMSA PSUR pricing; Tandem × Eterno and Rheumazentrum Mittelhessen.
- Carried over (see linked repo files): `research/hospital-billing-audits.md` (UK Frankfurt €181,800, DKI €40,000, Dr. Baller €360,000, 729 private hospitals, A17 status), `research/shortlist.md` (Ärzteblatt 7/2024 practices, ~98,000 practices, 1,480 device firms, § 22 SVHV, 92 Kassen), `research/munich-ecosystem.md` (EXIST, Start?Zuschuss!), `ventures/eldercare-navigator/brief.md` (salary assumption, PNOG).
