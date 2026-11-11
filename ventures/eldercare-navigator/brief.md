# Venture brief: Eldercare navigator as an employee benefit (L01)
Task: C1 | Date: 2026-11-11 | Status: draft (not yet reviewed by the critic) | Score: 66 base / 62 R4 in B1; 64 / 60 after the B2 red team (competition 2 → 1). Not re-scored here; the new findings below (low price points, 2028–29 statutory substitute) would lower it further.

**Bottom line for the CEO (researcher's view, you decide):**
- The pain is real and growing, and employers do pay for eldercare counselling. But the question C1 had to answer first, **"who pays a NEW small company?", has no sourced yes**: I found no company ≤3 years old that sells eldercare alone and shows a named paying employer.
- Observed prices for eldercare alone are low: a list price of €299–499 per company per month, and one public lot of ~€21,000 per year for a broadcaster.
- Munich is occupied on both sides: famPlus, pme and heycare (employer side), Nui Care (insurer side).
- New this run: the care reform bill (PNOG, BT-Drs. 21/8869, not yet law) makes the Pflegekassen provide a digital "Pflege-Cockpit" by 1 Jul 2028 and proactive, free case support ("Pflegebegleitung") from 1 Jan 2029, funded with ~€760m a year. That is a free substitute for the core of this product, arriving about a year after the planned full-time start. It is also a possible new buyer (Kassen may hand the task to third parties).
- **Recommendation: do not go to Stage D on the wedge as picked. Revise (options in section 12 and in task C3).**

## 1. One-liner
Employees of mid-size German companies (50–1,000 staff) who suddenly have to organise care for a parent struggle with care-grade applications, benefits and finding services next to their job; we give them an AI-supported care navigator with a human care adviser, paid by the employer as a tax-free benefit, so that they keep working and the employer loses fewer hours.

Wedge chosen for this brief: **(ii) mid-size employers without a family-service contract**. Wedge (i), software sold to the bundlers, is not chosen: no evidence that any bundler buys third-party tooling (section 6).

## 2. Problem evidence
**Hard data**
- **How many employees:** 4.6m people of working age gave informal care in 2023; this could rise to ~6.4m by 2045. Care-related lost work is estimated at ~184,000 full-time equivalents in 2026, rising to ~229,000 by 2045 [B] ([Bertelsmann Stiftung, 2026](https://www.bertelsmann-stiftung.de/fileadmin/files/user_upload/BSt_Informelle_Pflege_und_Erwerbstaetigkeit.pdf)).
- 4.1m carers were employed in 2021; "deutlich mehr als 80 Prozent" of them worked in establishments with ≥20 staff [B] ([Fraunhofer FIT, Nov 2023](https://publica-rest.fraunhofer.de/server/api/core/bitstreams/b55b85da-c6a4-4425-be2f-f746eb91a83e/content); data 2021, >3 years old).
- Of carers aged 18 to under 50, ~75 % were employed in 2022, working 35 hours a week on average and caring ~3 hours per working day. About 625,000 cut their working hours when care began; 440,000 extended them [B] ([iwd, 22 Jan 2026](https://www.iwd.de/pdf/doppelte-herausforderung-durch-beruf-und-pflege-669794/); the 625,000 figure via [Personalwirtschaft, 13 Mar 2026](https://www.personalwirtschaft.de/?p=201653)).
- "acht Prozent aller Erwerbstätigen" care next to work, i.e. ~80 per 1,000 staff; the typical caring employee is ~51 years old with 17 years in the company [B] (NRW labour ministry figures, quoted in [Personalwirtschaft](https://www.personalwirtschaft.de/?p=201653)).
- 46.9 % of employed carers are highly burdened; 45.2 % of part-timers cut hours because of care [B] (WIdO 2026, see `research/pain-patients.md` P3).
- **The navigation gap:** only "3 Prozent der Anspruchsberechtigten" use statutory care counselling [A] (GKV-SV § 7a report, see `research/pain-patients.md` P1). Counter-evidence: WIdO finds "fehlender Bedarf" and preference are the main reasons for not using services [B] (same file).
- **The employer gap:** 79.5 % of companies say family-friendly measures matter for supporting caring employees (2023: 64.8 %). But only 15.7 % offer help finding care services or cooperate with care providers (2015: 14.0 %), and 2.4 % train in-house "Pflegelotsen" [B] ([IW Unternehmensmonitor Familienfreundlichkeit 2026, table A-3](https://www.bmbfsfj.bund.de/resource/blob/293882/3408f56948ed9e772410b65ea57f9dec/unternehmensmonitor-familienfreundlichkeit-2026-data.pdf); 1,005 companies with ≥5 staff, Feb–May 2026). *Inference:* stated importance rose 15 points in three years, the offer barely moved in eleven. That is either an open market or weak willingness to pay; the survey cannot tell which.

**Online voices [C]: thin (2 independent sources opened; Reddit search returned 0 reddit.com hits again)**
- Nui Care app, iOS Germany: 185 ratings (avg 4.52); the review feed holds 24 written reviews 2019–2025 (14 five-star, 5 one-star) ([App Store search](https://itunes.apple.com/search?term=nui+care+pflege&country=de&entity=software&limit=5), [review feed](https://itunes.apple.com/de/rss/customerreviews/page=1/id=1361119539/sortby=mostrecent/json)). Excerpts:
  - "wenn man von jetzt auf gleich auf Hilfe angewiesen ist und dann auch noch alle Anträge usw ausfüllen, den mdk kommen lassen muss , überfordert das einen schon sehr" (Nov 2024, 5★)
  - "Enttäuschend – nicht für alle nutzbar" (Jul 2025, 1★; title)
  - "Dass die App 9,99 € pro Monat kostet sollte dem Nutzer bereits vor der Installation mitgeteilt werden." (Dec 2020, 4★)
  - "Für alle Zusatzinfos soll man dann 129,-€ zahlen- völlig überteuert!" (May 2021, 2★)
- rheuma-online forum: 8 of 21 threads on page 1 of the insurance subforum concern care-grade applications, MD assessments or the relief budget (opened in A3, see `research/pain-patients.md` P1).
- *Inference (counter-signal):* low self-pay tolerance (two of the excerpts complain about price) and low rating counts for navigator apps after years on the market: Nui 185, heycare 31, DAK Pflege-App 8, mitpflegeleben 15 (same App Store API, 11 Nov 2026). Rating counts are a weak proxy for use.

**Why now**
- Demographics: care recipients at home 5,161,367 on 31 Dec 2025 [A] ([PNOG cabinet draft, reasoning to § 7d](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Gesetze_und_Verordnungen/GuV/P/Kabinett-GE_Pflegeneuordnungsgesetz_PNOG.pdf)).
- Rules change on 1 Jan 2027 if the PNOG passes: care-grade thresholds rise to 15 / 30 / 50 points for grades 1–3; the relief allowance ends for grade 1; Pflegegeld becomes an "Entlastungsbudget" (€380 in grade 2, €630 in grade 3); decision deadlines are suspended from 1 Jan to 30 Apr 2027 [A] (same draft, § 15, § 37, § 142b). **Bill, may change:** first reading 5 Nov 2026 (BT-Drs. 21/8869); the minister announced changes to the relief allowance and respite care [B] ([Bundestag](https://www.bundestag.de/dokumente/textarchiv/2026/kw45-de-pflegeneuordnungsgesetz-1225076), [AOK G+G, 5 Nov 2026](https://www.aok.de/pp/gg/update/erste-lesung-pnog/)). *Inference:* more confusion and more rejected applications in 2027 raise demand for help.
- Against "why now": the same bill builds the free substitute (section 8).

## 3. Customer
- **User:** employee with a parent or partner who needs care (often 45–60 years old).
- **Buyer / signer:** HR or benefits lead, in mid-size firms often the managing director. Works council review is likely where one exists (section 8).
- **Payer:** the employer. The payment is tax-free for the employee: § 3 Nr. 34a lit. a EStG exempts employer payments "an ein Dienstleistungsunternehmen, das den Arbeitnehmer hinsichtlich der Betreuung von Kindern oder pflegebedürftigen Angehörigen berät oder hierfür Betreuungspersonen vermittelt" [A] ([§ 3 EStG](https://www.gesetze-im-internet.de/estg/__3.html)). *My reading:* the €600 cap in the text belongs to lit. b (short-term emergency care), not to counselling; to be confirmed by a tax adviser.
- **How large employers buy today [A] (TED awards, API fields opened):** as multi-year family-service or EAP frameworks, mostly bundles, with 1–2 bidders.

| Buyer (notice) | Winner | Value | Eldercare part | Bids |
|---|---|---|---|---|
| Max-Planck-Gesellschaft, Munich (763108-2025) | pme Familienservice | €1,200,000 | Component 8 "Homecare/Eldercare: Beratung und ggf. Vermittlung", not priced separately | 2 |
| Federal agencies via BMI (397127-2025) | awo lifebalance (size "small") | Lot 1 max €949,639; lot 2 (talks, seminars) max €443,143 | "Modul 5" inside lot 1 | 2 per lot |
| Umweltbundesamt (156595-2025) | Work-Life-Management GmbH (size "small") | €358,841 for both lots, 4 years | Inside lot 1 (children, relatives in need of care, household) | 2 |
| Bundesagentur für Arbeit (547026-2025) | awo lifebalance | not published, 40 months | "RV Service Beruf und Familie" | 1 |
| **Südwestrundfunk (535245-2024, contract notice)** | award not found in TED | **Lot 3 "Beratung und Vermittlung für die Pflege von Angehörigen": estimate €84,034 for 48 months**; lot 1 EAP €235,294; lot 2 family €184,873 | **Own lot** | n/a |
| **Straßen.NRW (569145-2026, contract notice)** | not yet awarded | not published; 2027–2030 | **Own lot "Los 2: Pflege"**, plus lot 4 webinars | closed 15 Sep 2026 |
| Charité "Elder Care" (565616-2022) | not shown | €372,000 | Own procedure; >3 years old | n/a |

  - Source: [TED API](https://api.ted.europa.eu/v3/notices/search), queries listed under Sources.
  - *My math:* SWR lot 3 = €84,034 / 4 years ≈ €21,000 per year.
  - **Answer to the desk test "is eldercare only bought inside bundles?": mostly, but not always.** 3 of the 7 procedures in the table tender it on its own (SWR lot 3, Straßen.NRW lot 2, Charité 2022); 4 bundle it. The two current ones demand references: Straßen.NRW scores "3 Pflichtreferenzen" plus liability insurance of €1.5m. A new company cannot bid alone.
- **First segment for a new company (inference):** private employers with 50–1,000 staff, no family-service contract, older workforce (manufacturing, utilities, banks, logistics), in the Munich area. No procurement rules apply. No source shows how many of them have no contract.

## 4. Solution & product wedge
- **Smallest product:** a web app plus a named human adviser.
  - Intake chat that builds a personal checklist ("Pflegefall in 48 hours": care-grade application, power of attorney, relief services, short-term care).
  - Pre-filled application forms and reminders; explanation of the MD assessment report.
  - A 30-minute call with a qualified care adviser when the case is not standard.
  - For HR: a one-page guide on Pflegezeit and Familienpflegezeit, two webinars a year. No usage report by person.
- **What AI does:** answers from a curated, dated knowledge base of SGB XI rules and local services; drafts forms and letters; the adviser reviews anything sent to an insurer.
- **Non-goals:** no medical or nursing advice; no legal representation or objections (section 8); no placement of care workers; no childcare, EAP or mental health; no selling to Pflegekassen in year 1.
- **Honest limit:** every element above already exists at famPlus, pme, heycare (employer side) and Nui Care (app with AI, insurer side). Nui's "Pflege-Kompass" already analyses MD assessment reports [B] ([heise, 17 Feb 2026](https://heise.de/-11180202)). The only differences left are price, speed of set-up and focus on firms the bundlers do not court. *Inference.*

## 5. Market size (bottom-up; prices are [B] list or estimate values, so the result is an estimate, not a fact)
- **Buyers [A]:** 84,701 legal units with 50 to under 250 employees (8,452,481 employees) and 18,632 with ≥250 (17,289,712 employees), 2024 ([Destatis](https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/Unternehmensregister/Tabellen/unternehmen-beschaeftigtengroessenklassen-wz08.html)). Legal units overstate independent buyers (groups count several times).
- **Price points observed [B]:**
  - Eldercare24 (ABE Akademie GmbH) list price: "Basis Paket – 299 € netto / Monat", "Komfort Paket – 499 € netto / Monat", "Preis pro Unternehmen", 24-month term ([eldercare24.de](https://eldercare24.de/)). The customer quotes on that page are placeholder text, so no customer is shown.
  - SWR lot 3 estimate: ~€21,000 per year (above). SWR staff: 3,543–3,688 `[UNVERIFIED]` (search snippets only) → roughly €6 per employee per year.
- **TAM (upper bound, my math):** (84,701 + 18,632) = 103,333 units × €3,588–5,988 per year (12 × €299 / €499) = **€371m–619m per year**. Cross-check per head: 25,742,193 employees × ~€6 ≈ €154m per year. The two methods differ by a factor of 2–4; treat the lower one as the better guess for large firms.
- **SAM (inference):** units without any care-placement offer: 103,333 × (1 − 0.157) ≈ 87,100. The 15.7 % is for all firms with ≥5 staff, and larger firms offer more, so this is too high. At €3,588: ≈ €313m. Bavaria or Munich share: not sourced.
- **SOM (inference):** 30–60 customers within 24 months of full-time start × €3,588–5,988 = **€108,000–359,000 ARR** (30 × 3,588 = 107,640; 60 × 5,988 = 359,280). This does not carry two founders' salaries. A venture case needs either >500 customers, a per-head price at larger firms, or a second payer.
- B1 used €5–20k per employer with ≥250 staff (€93–373m). The low end of that range is confirmed by one list price; the high end only by the SWR estimate.

## 6. Competitors
| Company | URL | Offering | Pricing | Funding / size | Gap we could exploit |
|---|---|---|---|---|---|
| pme Familienservice | [familienservice.de](https://www.familienservice.de/web/assistance/homecare-eldercare) | EAP, childcare, "Homecare-Eldercare"; ">1400 Unternehmen" (vendor claim) | Not public; MPG framework €1.2m [A] | Wins TED frameworks (MPG, TenneT €1.1m, kbo, AOK Hessen, F&W) [A] | Sells bundles to large and public employers |
| awo lifebalance | [awo-lifebalance.de](https://www.awo-lifebalance.de/) | EAP: childcare, care counselling, household help; "20 Jahre" | Not public; BMI lot 1 max €949,639 [A] | "small" per TED | Same |
| famPlus (Munich) | [famplus.de](https://www.famplus.de/gast/angebot/pflegeberatung) | Care counselling incl. applications, care-grade classification, provider search; "Über 550.000 Mitarbeiter*innen" covered (vendor claim) | Not public | Founded 2010 `[UNVERIFIED]` (snippet) | Local incumbent with the same product; none found |
| heycare (Munich, 2022) | [heycare.com](https://www.heycare.com/) | EAP + family service incl. care; "Über 450 Unternehmen" (vendor claim); own network of 35,000 carers | Not public | ~€4m extended seed, Mar 2026; says it is profitable [B] ([Munich Startup](https://www.munich-startup.de/en/news/heycare-raises-4-million-euros-in-growth-capital)) | Started with childcare; moving to "operative Teams" and health |
| voiio (Berlin) | [voiio.de](https://voiio.de/) | Platform for mental health, family, work; "1000+ Unternehmen" (vendor claim); "Beratung bei plötzlichem Pflegefall" | Not public | — | Lists ">1200 weitere Angebote": possibly a channel, not verified |
| Work-Life-Management GmbH | site returned HTTP 403 | Family and health service | UBA €358,841 / 4 years [A] | "small" per TED | — |
| Eldercare24 (ABE Akademie) | [eldercare24.de](https://eldercare24.de/) | **Eldercare only**, for the Mittelstand: hotline, online courses, consultations, Pflegelotsen training | €299 / €499 per company per month | No customer shown | Same wedge, already priced low |
| Nui Care (Munich, 2019) | [nui.care](https://www.nui.care/partner) | Carer app: applications "in nur 5 Minuten", AI analysis of MD reports, experts; white label for "Versicherungen und Unternehmen" | Free via AOK Bayern, Allianz PKV, DAK; else €9.99/month | ADAC invested early 2023; federal IGP grant [B] ([Munich Startup](https://www.munich-startup.de/en/news/nui-care-and-adac-launch-digital-care-assistant), [heise](https://heise.de/-11180202)) | Insurer channel taken; employer sales not shown |
| Aon | [aon.com](https://www.aon.com/germany/gesundheit-vorsorge/betriebliche-pflegeloesung) | Employer care solution (see `research/shortlist.md` e3) | Not public | Broker | — |
| Free substitutes | — | Pflegekasse counselling (§ 7a), Pflegestützpunkte; Familienpakt Bayern lists Pflegelotsen trainings by famPlus, pme München, Landratsamt Coburg, Stadt Bayreuth [B] ([PDF](https://www.familienpakt-bayern.de/images/2026/Pflegelotsentermine%202026%20final1.pdf)); NRW state programme with 690 participating employers [B] ([Personalwirtschaft](https://www.personalwirtschaft.de/?p=201653)); from 2028–29 Pflege-Cockpit and Pflegebegleitung (bill) | €0 | Public | Slow, office hours, not tied to the job |
| Abroad (proof of category) | [wellthy.com](https://www.wellthy.com/employers/purchase-plan) | US care concierge sold to employers since 2017 | "Starting at $450/month per employee" (per enrolled employee) | "$25M" round, May 2023 [B] ([TechCrunch](https://techcrunch.com/2023/05/11/wellthy-lands-25m-to-grow-its-tech-enabled-care-concierge-business/)) | Not in Germany |

**Desk tests from the red team (R1), results:**
| Test | Result |
|---|---|
| Named employer contract with a price for eldercare | **Partly found.** SWR lot 3 estimate €84,034 / 48 months [A]; Charité "Elder Care" €372,000 (2022, winner not shown) [A]. Both are estimates or totals, not unit prices. No private-employer price found except the Eldercare24 list price |
| Is eldercare bought only inside bundles? | **Mostly, not always.** 4 of 7 procedures bundle it; SWR, Straßen.NRW and Charité (2022) tender it on its own |
| heycare / famPlus first-sale dates | **Not found.** heycare founded 2022, customers named "according to the company" in Mar 2026 |
| Do frameworks allow subcontractors, or do bundlers buy third-party tech? | **None found.** Bidding consortia and capacity borrowing appear in one EAP tender (Autobahn GmbH, 429378-2025: 3 references each at organisations with ≥5,000 staff). No bundler page shows a technology partner. Nui builds its own AI |
| A company ≤3 years old, eldercare only, with a named paying employer | **None found** (4 searches, 6 vendor sites). BayWa using "WDS.eldercare" appeared in a search snippet only `[UNVERIFIED]` |

## 7. Business model & pricing
- **Model:** annual subscription per company, tiered by headcount; human adviser time included up to a cap.
- **Price hypothesis (inference from the benchmarks in section 5):** €300–500 per month for 50–250 staff; €6–12 per employee per year above that. Test whether a per-case fee (employer pays only when an employee enrols; Wellthy's public plan works this way) sells better.
- **Unit economics, rough (inference, no source):** at 8 % carers and perhaps one in ten of them opening a case per year, a 300-person firm produces 2–3 cases a year. Revenue €3,600–6,000 then covers ample adviser time. The constraint is sales cost per small contract, not delivery cost.
- **Footnote (L03):** Pflegekassen may commission online carer courses under § 45 SGB XI (`research/scoring.md`). Not a second payer in this brief (red team R4). The PNOG folds home training under § 45 into the Pflegebegleitung budget (section 8).

## 8. Regulation & data
- **Medical device:** not intended. The product gives administrative and benefits guidance and has no medical purpose. *Inference;* the MDR text was not re-opened this run `[UNVERIFIED]`. Keep symptom, medication and care-technique advice out.
- **Legal services (RDG) [A]:** "Rechtsdienstleistung ist jede Tätigkeit in konkreten fremden Angelegenheiten, sobald sie eine rechtliche Prüfung des Einzelfalls erfordert" ([§ 2 RDG](https://www.gesetze-im-internet.de/rdg/__2.html)). Independent out-of-court legal services are not allowed unless permitted ([§ 3 RDG](https://www.gesetze-im-internet.de/rdg/__3.html)); § 5 allows them only as an ancillary service ([§ 5 RDG](https://www.gesetze-im-internet.de/rdg/__5.html)). *Inference:* explaining benefits and filling in applications is likely fine; drafting objections against care-grade decisions is the risk zone. Needs one legal opinion (est. €2,000–4,000, my estimate) before launch. Nui lists Pflegewächter as a partner for this part [B] (Munich Startup, above).
- **Data protection [A]:** health data of relatives is a special category (Art. 9 GDPR); large-scale processing triggers a data-protection impact assessment (Art. 35(3)(b)) and a data-protection officer if it is the core activity (Art. 37(1)(c)) ([GDPR](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32016R0679)). The relative is a third party who must consent or be represented. Design: no personal data to the employer; EU hosting.
- **Works council [A]:** co-determination for "technische Einrichtungen, die dazu bestimmt sind, das Verhalten oder die Leistung der Arbeitnehmer zu überwachen" ([§ 87 BetrVG](https://www.gesetze-im-internet.de/betrvg/__87.html)). Whether a benefit app without reporting falls under it is `[UNVERIFIED]`. Eldercare24 avoids the issue: "Es erfolgen keine individuellen oder aggregierten Auswertungen".
- **DiGA / DiPA:** no route. DiPA excludes navigation-only apps (`research/reimbursement-routes.md`).
- **EU AI Act:** transparency duties for chatbots likely apply; not checked `[UNVERIFIED]`.
- **PNOG (bill, BT-Drs. 21/8869; cabinet draft 30 Sep 2026; may change) [A]** ([cabinet draft](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Gesetze_und_Verordnungen/GuV/P/Kabinett-GE_Pflegeneuordnungsgesetz_PNOG.pdf)):
  - **§ 7a new, "Pflege-Cockpit":** every Pflegekasse opens "einen einheitlichen digitalen Zugang" for each insured care recipient and authorised relatives: benefits per care grade, benefits drawn, filing applications and receipts with status, provider and price search, counselling and training offers. Functions 1–7 "spätestens bis zum 1. Juli 2028", the rest by 1 Jan 2030.
  - **§ 7c new, "Pflegebegleitung":** "Ab dem 1. Januar 2029" care recipients at home and their carers are entitled to professional support. The Kasse must offer "einen konkreten Termin" at home right after the first care grade; tasks include a care plan, help with applications for aids, showing relief options, and case management across benefit systems. Phone or video on request. Pflegegeld recipients must call it up once a year.
  - **§ 7d new, money:** "146 Euro je pflegebedürftiger Person in häuslicher Pflege" per year, "rechnerisch rund 760 Millionen Euro". "Die Pflegekassen können die Pflegebegleitung auch ganz oder teilweise auf Dritte übertragen". The reasoning notes that some Kassen have already handed today's counselling to third parties. The GKV-SV recommends staff numbers and qualification by 30 Sep 2027; municipalities declare a takeover by 31 Dec 2027.
  - *Inference:* from 2028–29 the statutory system offers, free, most of what this product does once a care grade exists. What stays outside: the weeks before the first care grade, the job side (Pflegezeit, talking to the employer), and speed. The same bill creates a €760m-a-year task that Kassen and municipalities may outsource. That is a different customer (signer cluster C5, Pflegekasse) and a different company.
- **Certifications:** none mandatory found. famPlus advertises a DEKRA audit against DIN 77009-1; buyers may ask for it. Not checked.
- **Time and cost to launch (inference):** 3–4 months; legal and privacy set-up €4,000–8,000.

## 9. Go-to-market
- **First 10 customers (inference):** owner-led or mid-size firms with 150–1,000 staff in the Munich area with no family-service contract. Reach them through:
  - the Familienpakt Bayern network (it already promotes Pflegelotsen trainings, so its members have shown interest);
  - company health insurers (BKKs): Miele BKK presented a concept for supporting caring employees at BKK Innovativ [B] ([PDF](https://www.bkk-dachverband.de/fileadmin/Artikelsystem/BKK_INNOVATIV/Vorstellung_Konzept_pflegende_Mitarbeitende_BKK_Innovativ_Miele_BKK.pdf));
  - benefit brokers and platforms as resellers (voiio marketplace, Aon): not verified as open to new providers.
- **Pilot design:** 3 firms, 6 months, €0–1,500 each, with a signed intent to convert at list price if ≥3 % of staff open a case and HR rates it ≥8/10. Measure cases opened, time to care-grade application, hours saved (self-report).
- **Constraints:** the founder is in Lisbon until Sep 2027; mid-size HR sales are relationship sales (red team R2). 24-month contracts at €299 a month do not pay for field sales, so the channel must be inbound, partners or webinars.
- Public tenders are closed to a new company (references). They become possible only as a subcontractor or consortium member of a bundler.

## 10. Funding path
From `research/munich-ecosystem.md` (sources and dates there; all re-checked on 7 Nov 2026, not this run):
| Step | Programme | Fit | Date |
|---|---|---|---|
| Now, part-time | BayStartUP business plan competition, phase 1 | Open to part-time founders; coaching, angel network | 13 Jan 2027 |
| Now, part-time | SCE Incubation (Hochschule München), ≥10 h/week; prepares for EXIST | Needs ≥3 potential B2B customers validated | Summer batch from Mar 2027; deadline not published |
| Before founding | EXIST Gründungsstipendium (€2,500/month, 12 months, €30,000 material costs for a team) | Needs a German Hochschule host, no active job, "innovative" project. A counselling service with standard LLM tooling may not pass the innovation test (*inference*) | Guideline open to 31 Dec 2027 |
| After founding | Start?Zuschuss! (50 % of costs, max €36,000) | Digital startup ≤2 years old | Round 23: 25 Nov 2026–10 Jan 2027; two rounds a year |
| Later | Federal IGP programme | Nui's two features are IGP-funded [B] (heise) | Not checked |
- **Investors seen in this category [B]:** Scalehouse Capital, Swiss Post Ventures (heycare); ADAC (Nui). Bayern Kapital and the BayStartUP angel network as in the ecosystem file. A ≥10-name list belongs to Stage D.
- **Capital to first revenue (inference):** €8,000–15,000 (company set-up, legal and privacy opinions, insurance, tools), i.e. at or above the €10,000 own budget. A pilot before incorporation is cheaper.
- **Investor view (red team):** a services category with €3,600–6,000 contracts and funded incumbents. Venture funding is unlikely before proof of a scalable channel.

## 11. Team
- **Co-founder 1 (must-have): care counselling lead.** Qualified Pflegeberater:in or social worker with case-management practice (Pflegestützpunkt, Kasse, compass, famPlus, pme). Brings credibility with HR, content quality and the future "Pflegebegleitperson" qualification (GKV-SV recommendations due 30 Sep 2027, bill).
- **Co-founder 2 (should-have): product engineer** (web app, retrieval over legal texts, privacy by design). The CEO covers AI workflow design, sales and operations.
- **Where to look (Munich):** Hochschule München and Katholische Stiftungshochschule (nursing and social-work programmes; not checked this run `[UNVERIFIED]`), SCE and TUM Venture Lab Healthcare networks, the Munich Startup co-founder board (`research/munich-ecosystem.md`), Pflegestützpunkte staff, alumni of the incumbents.

## 12. Risks & kill criteria (draft for the critic pre-mortem)
| Riskiest assumption | Evidence so far | How to test | Kill if |
|---|---|---|---|
| A mid-size employer pays a new, unknown company for eldercare alone | None. No young eldercare-only vendor with a named employer found. List price €299–499 without shown customers | 5–8 HR conversations (needs CEO approval), then 3 paid pilots | 0 of 8 HR leads would pay ≥€250 a month, or <2 pilots convert |
| Enough firms have no family-service contract | Only 15.7 % of firms offer care-placement help [B]; share among firms of 50–1,000 staff unknown | Ask in the same conversations; count named customers on bundler sites | ≥6 of 8 already covered by pme, famPlus, awo, heycare or voiio |
| The statutory substitute does not remove the need | PNOG: Cockpit by 1 Jul 2028, Pflegebegleitung from 1 Jan 2029, free (bill) | Read the law as passed (2nd/3rd reading planned 11 Dec 2026, date from `research/trends.md`) | §§ 7a, 7c, 7d pass unchanged and the pilot value lies mostly after the first care grade |
| Employees use it | Competitor claim: classic EAP and family services have "Geringe Nutzung – oft unter 3%" (heycare marketing) | Pilot: cases per 100 staff per year | <1 case per 100 staff in 6 months |
| Unit economics carry a company | SOM €108,000–359,000 ARR at 30–60 customers (inference) | Price test with per-head pricing at 500+ staff | No route to >€1m ARR within 3 years of full-time start |
| Incumbents do not copy or undercut | famPlus and pme run Pflegelotsen trainings in Bavaria; heycare has €4m | Watch bundler pricing for small firms | A bundler offers a care-only tier at ≤€300 a month |
| Legal: help with applications is not a legal service | § 2, § 5 RDG text; no opinion yet | One legal opinion | Opinion says core features need a lawyer |
| Founder can sell from Lisbon, part-time, until Sep 2027 | Red team R2 | 10-minute founder-access check; first 5 conversations by video | No HR conversation booked within 6 weeks of approval |

**Options for the CEO (decision task C3):**
- **(a) Go to Stage D as written.** Not recommended: no paying-customer proof, low price points, substitute in 2028–29.
- **(b) Revise, cheap test first (recommended).** Approve 5–8 HR conversations and re-read the PNOG after the Bundestag vote. Then decide between the employer wedge and a re-wedge towards the new Pflegebegleitung task (tools or delivery for Kassen, Pflegestützpunkte, municipalities; €760m a year from 2029 if the bill passes). The re-wedge is a different buyer and needs its own desk run.
- **(c) Drop L01** and reopen a parked idea (L07 with a named medical-controlling co-founder, or the L11 test).

## 13. Validation plan (no outreach done; every item needs CEO approval)
- **Who (8 interviews):** 5 HR or benefits leads at Munich-area firms with 150–1,000 staff (3 without a family-service contract, 2 with pme, famPlus or heycare); 1 works-council member; 1 Pflegestützpunkt adviser or Kasse care counsellor; 1 employee who organised care for a parent in the last 12 months.
- **Questions (past behaviour, not opinions):**
  - HR: When did an employee last tell you about a care case? What happened, what did it cost you (hours, absence, resignation)? What do you offer today, since when, what do you pay, how many used it last year? Who signed? What did you look at and not buy, and why?
  - Works council: which benefit tools went through co-determination, and how long did it take?
  - Adviser: where do working relatives get stuck before and after the first care grade? What will change with Pflegebegleitung?
  - Employee: what did you do in the first two weeks, who helped, what did you pay for?
- **Confirms:** ≥3 of 5 HR leads name a recent case with cost, have no contract, and name a budget or a price ≥€250 a month; ≥1 agrees to a paid pilot.
- **Kills:** see section 12.

## Gaps / [UNVERIFIED]
- No interviews, no price quotes, no customer data (by design until Stage D).
- No first-sale dates for heycare or famPlus; famPlus founding year from a snippet only.
- SWR award and SWR headcount (snippets: 3,543 or 3,688) not verified; the per-employee price is therefore rough.
- Wellthy "$3–6 per employee per month" and the UK example KareHero/TSB: search snippets only, not used.
- BayWa using "WDS.eldercare": search snippet only; wds.care unreachable (proxy 502); amiravita.de and work-life-management.de returned HTTP 403.
- Whether voiio or Aon take on new third-party providers: not verified.
- MDR and EU AI Act texts not re-opened this run; § 87 BetrVG applicability; reading of the €600 cap in § 3 Nr. 34a EStG.
- PNOG is a bill; amendments were announced on 5 Nov 2026. All PNOG figures are from the cabinet draft.
- Share of firms with 50–1,000 staff that already hold a family-service contract: no source.
- Fraunhofer data are from 2021 (>3 years old). Stale but used only for context.

## Sources (all accessed 2026-11-11 unless noted)
- https://api.ted.europa.eu/v3/notices/search — TED API [A]. Queries: `FT~"Familienservice" AND buyer-country=DEU AND publication-date>=20220101` (19 notices); same with `"Eldercare"` (4), `"Elder Care"` (4), `"Employee Assistance"` (23), `"Pflegelotsen"` (2), `"Pflege von Angehörigen"` (8), `"pflegebedürftigen Angehörigen" AND FT~"Beschäftigte"` (9). Notices read: 763108-2025, 329012-2025, 397127-2025, 156595-2025, 684261-2024, 547026-2025, 350159-2025, 535245-2024, 569145-2026, 565616-2022, 105910-2024, 159617-2026, 321969-2025, 429378-2025, 630711-2025, 286946-2025. Fields: winner-name, result-value-lot, BT-27-Lot, title-lot, description-lot, received-submissions-type-val, winner-size, selection-criterion-description-lot, deadline dates
- https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Gesetze_und_Verordnungen/GuV/P/Kabinett-GE_Pflegeneuordnungsgesetz_PNOG.pdf — PNOG cabinet draft: §§ 7a, 7c, 7d, 15, 37, 142b, reasoning, entry into force [A]
- https://www.bundestag.de/dokumente/textarchiv/2026/kw45-de-pflegeneuordnungsgesetz-1225076 — first reading 5 Nov 2026, BT-Drs. 21/8869 [A]
- https://www.aok.de/pp/gg/update/erste-lesung-pnog/ — announced amendments, €7.6bn gap [B]
- https://www.bmbfsfj.bund.de/resource/blob/293882/3408f56948ed9e772410b65ea57f9dec/unternehmensmonitor-familienfreundlichkeit-2026-data.pdf — IW monitor 2026, table A-3, sample [B]
- https://www.bertelsmann-stiftung.de/fileadmin/files/user_upload/BSt_Informelle_Pflege_und_Erwerbstaetigkeit.pdf — carers of working age, lost FTE [B]
- https://publica-rest.fraunhofer.de/server/api/core/bitstreams/b55b85da-c6a4-4425-be2f-f746eb91a83e/content — Fraunhofer FIT, employed carers 2021 [B]
- https://www.iwd.de/pdf/doppelte-herausforderung-durch-beruf-und-pflege-669794/ — IW, carers and employment 2022 [B]
- https://www.personalwirtschaft.de/?p=201653 — 8 % of employees, 625,000 reduced hours, heycare, NRW programme [B]
- https://www.personalwirtschaft.de/?p=209517 — voiio/Bilendi study exists (paywalled; not used for figures) [B]
- https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/Unternehmensregister/Tabellen/unternehmen-beschaeftigtengroessenklassen-wz08.html — legal units by size class 2024 [A]
- https://www.gesetze-im-internet.de/estg/__3.html — § 3 Nr. 34a EStG [A]
- https://www.gesetze-im-internet.de/rdg/__2.html, /__3.html, /__5.html — RDG [A]
- https://www.gesetze-im-internet.de/betrvg/__87.html — § 87 BetrVG [A]
- https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32016R0679 — GDPR Art. 9, 35, 37 [A]
- https://eldercare24.de/ — package prices, ABE Akademie GmbH [B]
- https://www.heycare.com/ — 450 companies, modules, "oft unter 3%" [B]
- https://www.munich-startup.de/en/news/heycare-raises-4-million-euros-in-growth-capital — heycare round, founding year [B]
- https://www.famplus.de/ and https://www.famplus.de/gast/angebot/pflegeberatung — famPlus offering [B]
- https://www.familienservice.de/ and https://www.familienservice.de/web/assistance/homecare-eldercare — pme [B]
- https://www.awo-lifebalance.de/ — awo lifebalance [B]
- https://voiio.de/ — voiio [B]
- https://www.nui.care/ and https://www.nui.care/partner — Nui Care partners, pricing [B]
- https://www.munich-startup.de/en/news/nui-care-and-adac-launch-digital-care-assistant — Nui founded 2019, ADAC, insurers [B]
- https://heise.de/-11180202 — Nui contracts, AI features, IGP funding [B]
- https://www.aon.com/germany/gesundheit-vorsorge/betriebliche-pflegeloesung — Aon [B]
- https://www.familienpakt-bayern.de/images/2026/Pflegelotsentermine%202026%20final1.pdf — Pflegelotsen trainings in Bavaria [B]
- https://www.bkk-dachverband.de/fileadmin/Artikelsystem/BKK_INNOVATIV/Vorstellung_Konzept_pflegende_Mitarbeitende_BKK_Innovativ_Miele_BKK.pdf — Miele BKK concept [B]
- https://www.wellthy.com/employers/purchase-plan and https://techcrunch.com/2023/05/11/wellthy-lands-25m-to-grow-its-tech-enabled-care-concierge-business/ — Wellthy [B]
- https://itunes.apple.com/search?term=nui+care+pflege&country=de&entity=software&limit=5 (also terms heycare, mitpflegeleben) and https://itunes.apple.com/de/rss/customerreviews/page=1/id=1361119539/sortby=mostrecent/json — app ratings and reviews [C]
- Repo files: `research/pain-patients.md`, `research/shortlist.md`, `research/reimbursement-routes.md`, `research/munich-ecosystem.md`, `research/scoring.md`, `research/trends.md`, `research/reviews/2026-11-08-redteam-shortlist.md`
