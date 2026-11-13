# Fact-check: ventures/eldercare-navigator/brief.md (C1)
Date: 2026-11-12 | Verdict: **needs work (minor)** | Sources checked: 37 of 37 listed URLs opened (all), plus all 16 TED notices named in the brief and 6 repo files it cites

Scope: the brief is the only file in `research/` and `ventures/` that is new since the last fact-check; `research/shortlist.md` (B4 edits) is covered in `2026-11-12-shortlist-B4.md`. Mode FACT-CHECK only. Not judged here: the business idea, the weight given to the PNOG substitute, and whether the kill criteria are testable. That is the red-team half of critic task C2 and is still open.

**Summary.** No fabrication: every quote I opened is verbatim and traceable, and there are no interviews or invented feedback. The numbers the brief rests on reproduce: TED values and lot titles, the PNOG quotes for §§ 7a, 7c, 7d, IW table A-3, the Destatis size classes, the Eldercare24 prices and all arithmetic in section 5. One rule-1 breach (an `[UNVERIFIED]` number is built on) and four statements that say more than the source does. None of them changes the brief's recommendation; all of them make the case slightly weaker, not stronger.

**Counts re-run (2026-11-12): all match.**
- TED API, 7 queries: 19 / 4 / 4 / 23 / 2 / 8 / 9 notices. Match.
- App Store API: Nui 185 ratings (avg 4.519), heycare 31, DAK Pflege-App 8, mitpflegeleben 15. Match.
- Nui review feed: 24 entries, 2019-04-01 to 2025-07-28, 14 five-star, 5 one-star (also 4 four-star, 1 two-star). Match. The four excerpts are verbatim with the stated month and rating.

## Critical issues (must fix)
1. **An `[UNVERIFIED]` number is used in arithmetic and then built on (CLAUDE.md rule 1), although the cited source contains the verified figure.**
   - Section 5: "SWR staff: 3,543–3,688 `[UNVERIFIED]` (search snippets only) → roughly €6 per employee per year."
   - Built on in three places: the TAM cross-check "25,742,193 employees × ~€6 ≈ €154m per year ... treat the lower one as the better guess for large firms"; the price hypothesis in section 7, "€6–12 per employee per year above that"; and the kill row "Price test with per-head pricing at 500+ staff".
   - The TED notice the brief already cites (535245-2024, field `description-proc`) says: "Insgesamt beschäftigt der SWR ca. 3.500 Festangestellte und ca. 1.800 arbeitnehmerähnliche freie Mitarbeiter" and "Für seine Mitarbeiter sucht der SWR ...". That is an [A] figure.
   - My arithmetic: €84,034 / 4 = €21,009 per year. Per head: €6.00 with 3,500 permanent staff; €3.96 with 5,300 if the freelancers are covered (the notice does not say). Cross-check: 25,742,193 × €4–6 = €103m–154m.
   - Also say next to the figure that it is one buyer's **estimate** (BT-27, contract notice) and that no award exists: I searched TED for an SWR award notice and found only the contract notice. The whole per-head method rests on this single data point.
   - Effect: the lower TAM bound and the per-head price move down or stay; the conclusion "low price points" holds.

## Other issues (minor; fold into the same fix round)
2. **Nui "already analyses" is not what the source says.** Section 4: "Nui's 'Pflege-Kompass' already analyses MD assessment reports [B] (heise, 17 Feb 2026)". heise: "The 'Pflege-Kompass' is intended to analyze care reports" and findings "are to be translated". The competitor table adds "AI analysis of MD reports" under the nui.care/partner link; that page only says "zukunftsweisende KI-Technologie". nui.care lists a news item dated 02/11/2026 on a "KI-Pflegegradassistent" (orientation on the likely care grade), which is a different feature. Write "announced (Feb 2026); live status not shown".
3. **TenneT "€1.1m" is ambiguous.** Section 6 gives "TenneT €1.1m [A]". Notice 159617-2026: `result-value-lot` 1,100,000, but `tender-value` and `result-value-notice` 880,000; estimate 2,100,000; 3 bids. State which value is meant (winning tender €880,000).
4. **Bundesagentur row: the eldercare part is emergency short-term care, not counselling.** Notice 547026-2025: "Beratungs-, Vermittlungs- und Betreuungsdienstleistung von Kindern und einer Kurzzeitpflegebetreuung für pflegebedürftige Angehörige" ("Kurzzeitpflege in Notfällen"). It still counts as "bundled", so the 4-of-7 / 3-of-7 count stands, but it is not evidence that the BA buys eldercare navigation.
5. **Charité "Elder Care", "own procedure": value verified, scope not.** 565616-2022 is an old-format notice: the API returns the buyer and `total-value` 372,000 but no title or lot text, and it matches the full-text query "Elder Care". The TED XML/PDF returned HTTP 202 (empty) for me. So "own procedure for eldercare" is supported only by the full-text match. With Charité uncertain, the firm examples of eldercare tendered as its own **lot** are two (SWR lot 3, Straßen.NRW lot 2), both inside a family-service procedure, not stand-alone procedures. "Tender it on its own" should read "as its own lot".
6. **heycare's own homepage shows named customers; the brief cites only the press article.** heycare.com (opened) carries testimonials attributed to named staff at Helvetia Deutschland, CCEP and Marsh, each tagged "Eingesetzte Lösungen: Familienservice" (some "+ EAP"); one further testimonial is placeholder text ("Lorem ipsum ... Name Surname"). This does not contradict the headline finding (heycare was founded in 2022, so it is 4 years old, and it sells a bundle), but the desk-test row "customers named 'according to the company'" understates what the vendor shows. The modules do not say whether care or childcare is used. First-sale dates: still not found.
7. **Stale data not flagged.** The brief flags Fraunhofer (2021) and Charité (2022). Not flagged: the iwd figures are SOEP **2022** (75 % employed, 35 h, 3 h per working day, and the 625,000 / 440,000); the two price complaints in the Nui excerpts date from Dec 2020 and May 2021. The inference "low self-pay tolerance (two of the excerpts complain about price)" therefore rests on two [C] reviews that are 5–6 years old; the €129 price is no longer on nui.care.
8. **Bertelsmann figures are the lower bound of a range.** The summary says "rund 184.000 Vollzeitäquivalenten ... bis 2045 auf rund 229.000"; the body gives "184.000 bzw. 264.000" for 2026 and "229.000 bzw. 327.000" for 2045 (two model variants). Add the range.
9. **Small attribution points.** (a) "the 625,000 figure via Personalwirtschaft": the iwd page itself has both 625,000 and 440,000. (b) The 5,161,367 are "ambulant gepflegte SPV-Versicherte" (statutory insurance only). (c) The F&W award (363180-2024, pme, EAP) exists in TED but is missing from the "Notices read" list. (d) The BKK PDF text does not contain the word "Miele"; only the file name does. (e) § 7a: the list in section 8 includes "counselling and training offers", which are numbers 8–9 and due by 1 Jan 2030, not 1 Jul 2028; the sentence after it is correct.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| MPG: pme, €1,200,000, component 8 "Homecare/Eldercare: Beratung und ggf. Vermittlung", 2 bids | TED 763108-2025, 329012-2025 | Supported | Verbatim "8. Betreuung und Pflege Angehöriger \"Homecare/Eldercare\": Beratung und ggf. Vermittlung"; winner size "large" |
| BMI: awo lifebalance ("small"), lot 1 max €949,639, lot 2 max €443,143, "Modul 5", 2 bids per lot | TED 397127-2025 | Supported | "Modul 5 - Allgemeine Beratung zur Betreuung von pflege- und unterstützungsbedürftigen Angehörigen" |
| UBA: Work-Life-Management GmbH ("small"), €358,841 both lots, 4 years, 2 bids | TED 156595-2025, 684261-2024 | Supported | |
| BA: awo lifebalance, value not published, 40 months, 1 bid | TED 547026-2025, 350159-2025 | Supported | Value field 0.01; eldercare part = emergency short-term care (issue 4) |
| SWR: lot 3 "Beratung und Vermittlung für die Pflege von Angehörigen" est. €84,034 / 48 months; lot 1 €235,294; lot 2 €184,873; award not found | TED 535245-2024 | Supported | Sum 504,201 = BT-27-Procedure; no award notice found on re-search |
| SWR staff 3,543–3,688 | search snippets | **[UNVERIFIED] built on** | Notice says ca. 3,500 + ca. 1,800 freelancers (issue 1) |
| Straßen.NRW: "Los 2: Pflege", lot 4 webinars, 2027–2030, closed 15 Sep 2026, "3 Pflichtreferenzen", €1.5m liability | TED 569145-2026 | Supported | 15 Sep 2026 is the deadline for requests to participate; €1.5m is for personal injury (€0.25m other damage) |
| Charité "Elder Care", €372,000, winner not shown, own procedure | TED 565616-2022 | Partially | Value and full-text match yes; title and scope not retrievable (issue 5) |
| Autobahn GmbH: consortia, capacity borrowing, 3 references each at ≥5,000 staff | TED 429378-2025, 630711-2025 | Supported | "mindestens 3 Referenzprojekte je Bereich ... Betriebsgröße mind. 5.000 Mitarbeitende" |
| pme wins: TenneT €1.1m, kbo, AOK Hessen, F&W | TED 159617-2026, 321969-2025, 105910-2024, 363180-2024 | Partially | Winners verified; TenneT value ambiguous (issue 3); F&W not in "Notices read" |
| PNOG § 7a: "einen einheitlichen digitalen Zugang"; functions 1–7 "spätestens bis zum 1. Juli 2028", rest by 1 Jan 2030 | BMG cabinet draft | Supported | Verbatim |
| PNOG § 7c: "Ab dem 1. Januar 2029"; "einen konkreten Termin"; care plan, aids applications, relief options, case management; phone/video; Pflegegeld recipients once a year | same | Supported | "unmittelbar nach erstmaligem Erhalt eines Pflegegrades"; "einmal jährlich" |
| PNOG § 7d: "146 Euro je pflegebedürftiger Person in häuslicher Pflege"; "rechnerisch rund 760 Millionen Euro"; "ganz oder teilweise auf Dritte übertragen"; GKV-SV recommendations by 30 Sep 2027; municipal takeover notice by 31 Dec 2027 | same | Supported | Reasoning: "Bereits heute haben manche Pflegekassen die bisherige Pflegeberatung (vollständig) auf Dritte übertragen" |
| 5,161,367 care recipients at home on 31 Dec 2025 | same (reasoning to § 7d) | Supported | SPV-insured only |
| Thresholds 15 / 30 / 50; relief allowance ends in grade 1; Entlastungsbudget €380 / €630; deadlines suspended 1 Jan–30 Apr 2027 | same (§ 15, § 37, § 142b, reasoning) | Supported | |
| First reading 5 Nov 2026, BT-Drs. 21/8869; minister announced changes to relief allowance and respite care | bundestag.de; AOK G+G | Supported | G+G also: vote planned 11 Dec; €7.6bn gap |
| 79.5 % (2023: 64.8 %); 15.7 % (2015: 14.0 %); 2.4 % Pflegelotsen; 1,005 companies, ≥5 staff, Feb–May 2026 | IW Unternehmensmonitor 2026, fig. 2-2 and table A-3 | Supported | Table A-3: 14.0 / 13.4 / 14.4 / 15.7; Pflegelotsen 2.0 (2023) / 2.4 (2026); survey 10 Feb–4 May 2026 |
| 4.6m working-age carers 2023, ~6.4m by 2045; ~184,000 FTE 2026, ~229,000 by 2045 | Bertelsmann Stiftung 2026 | Supported (partly) | Lower bound of a range (issue 8) |
| 4.1m employed carers 2021; "deutlich mehr als 80 Prozent" in establishments ≥20 staff | Fraunhofer FIT 2023 | Supported | Source text starts "Deutlich"; stale, flagged in the brief |
| ~75 % of carers 18–<50 employed 2022, 35 h/week, ~3 h per working day; 625,000 cut hours, 440,000 extended | iwd, 22 Jan 2026 | Supported | Data 2022, not flagged as >3 years (issue 7) |
| "acht Prozent aller Erwerbstätigen"; ~51 years, 17 years in the company; NRW programme, 690 employers | Personalwirtschaft | Supported | Relayed NRW ministry figures; [B] correct |
| 46.9 % highly burdened; 45.2 % of part-timers cut hours; "3 Prozent der Anspruchsberechtigten"; "fehlender Bedarf"; rheuma-online 8 of 21 | `research/pain-patients.md` P1, P3 | Supported | Matches the repo file (fact-checked 2026-11-07); forum count is "titles only" there |
| 84,701 units with 50–<250 staff (8,452,481 employees); 18,632 with ≥250 (17,289,712), 2024 | Destatis | Supported | Legal units, as the brief says |
| § 3 Nr. 34a lit. a EStG quote; €600 cap belongs to lit. b | gesetze-im-internet.de | Supported | Reading of the cap is marked as the researcher's own |
| § 2 RDG quote; § 3; § 5 ancillary service | gesetze-im-internet.de | Supported | |
| § 87 BetrVG quote | gesetze-im-internet.de | Supported | Abs. 1 Nr. 6 |
| GDPR Art. 9, 35(3)(b), 37(1)(c) | EUR-Lex | Supported | German § 38 BDSG (DPO whenever a DPIA is required) is not mentioned; not checked this run |
| Eldercare24: "Basis Paket – 299 € netto / Monat", "Komfort Paket – 499 € netto / Monat", "Preis pro Unternehmen", 24 months, ABE Akademie GmbH, placeholder testimonials, "Es erfolgen keine individuellen oder aggregierten Auswertungen" | eldercare24.de | Supported | Testimonials are "Lorem ipsum" under "Musterfrau" / "Mustermann" |
| pme ">1400 Unternehmen"; "Homecare-Eldercare" | familienservice.de | Supported | EAP customers; also "Über 1.400 Arbeitgeber:innen" |
| awo lifebalance: care counselling, "20 Jahre" | awo-lifebalance.de | Supported | |
| famPlus: care counselling incl. applications and care-grade classification; "Über 550.000 Mitarbeiter*innen"; DEKRA audit DIN 77009-1 | famplus.de | Supported | Founding year 2010 stays [UNVERIFIED], as flagged |
| heycare: "Über 450 Unternehmen", 35,000 carers, "Geringe Nutzung – oft unter 3%"; founded 2022, ~€4m extended seed Mar 2026, profitable, Scalehouse and Swiss Post Ventures | heycare.com; Munich Startup | Supported | Founded as Heynanny; see issue 6 |
| voiio: "1000+ Unternehmen", "Beratung bei plötzlichem Pflegefall", ">1200 weitere Angebote" | voiio.de | Supported | |
| Nui: founded 2019; ADAC invested early 2023; AOK Bayern, Allianz PKV, DAK; €9.99/month; "Pflegeanträge in nur 5 Minuten"; white label for "Versicherungen und Unternehmen"; Pflegewächter partner; IGP funding | nui.care, nui.care/partner, Munich Startup, heise | Supported | |
| Nui Pflege-Kompass "already analyses" MD reports | heise | **Partially** | "is intended to analyze" (issue 2) |
| Aon "betriebliche Pflegelösung" | aon.com | Supported | Offering only |
| Familienpakt Bayern: Pflegelotsen trainings by famPlus, pme München, Landratsamt Coburg, Stadt Bayreuth | PDF (Stand Feb 2026) | Supported | |
| Miele BKK concept for caring employees | BKK Dachverband PDF | Supported (partly) | Content matches; "Miele" only in the file name |
| Wellthy: "Starting at $450/month per employee"; employers since 2017; "$25M" May 2023 | wellthy.com; TechCrunch | Supported | TechCrunch: founded 2015, employers "by 2017", $25.5m |
| voiio/Bilendi study exists, paywalled | Personalwirtschaft ?p=209517 | Supported | Not used for figures |
| Funding table (BayStartUP 13 Jan 2027; SCE ≥10 h/week, ≥3 B2B customers; EXIST €2,500 / €30,000, to 31 Dec 2027; Start?Zuschuss! 50 %, max €36,000, round 23) | `research/munich-ecosystem.md` | Supported | Matches the repo file; the brief says it was not re-checked this run |
| 2nd/3rd reading planned 11 Dec 2026; DiPA excludes navigation-only apps; B1 €93–373m; score 66/62 and 64/60 | `research/trends.md`, `reimbursement-routes.md`, `shortlist.md`, red-team review | Supported | 18,632 × €5–20k = €93.2–372.6m |
| Section 5 arithmetic (TAM €371–619m; €154m; SAM 87,100 and €313m; SOM €108,000–359,000) | own check | Reproduces | 103,333 × 3,588 = 370.8m; × 5,988 = 618.8m; 25,742,193 × 6 = 154.5m; 103,333 × 0.843 = 87,110 |

## Evidence grades
- Tags are right: TED, statutes, the cabinet draft and Destatis [A]; reports, trade press and vendor sites [B]; App Store reviews and the forum [C].
- No market size rests on [C]. The TAM rests on one vendor **list** price with no customer shown and one buyer's estimate; the brief says so ("an estimate, not a fact").
- Vendor claims (pme, famPlus, heycare, voiio customer counts; heycare's "oft unter 3%") are labelled as vendor claims.

## [UNVERIFIED] items
| Item | Where | Treated as fact or built on? |
|---|---|---|
| SWR staff 3,543–3,688 (snippets) | Section 5 | **Yes** (issue 1); resolvable from the cited notice |
| famPlus founded 2010 (snippet) | Section 6 | No |
| BayWa using "WDS.eldercare" (snippet) | Section 6 desk tests | No |
| MDR: no medical purpose (text not re-opened) | Section 8 | Used as a design assumption ("not intended"); marked as inference |
| § 87 BetrVG applies to a benefit app without reporting | Section 8 | No |
| EU AI Act transparency duties | Section 8 | No |
| Hochschule München / KSH programmes as co-founder sources | Section 11 | No |
| Wellthy "$3–6 per employee per month"; KareHero/TSB | Gaps | Not used |

## Unsourced statements (not tagged)
- Section 3: user "often 45–60 years old" (the only sourced figure is "rund 51 Jahre"); "Works council review is likely".
- Section 8: "Time and cost to launch: 3–4 months; €4,000–8,000" and section 10 "€8,000–15,000" are marked as inference but have no basis shown.
- Section 9: Familienpakt members "have shown interest" (inference, not marked).

## Not verified this run
- Charité notice title and scope (TED XML/PDF returned HTTP 202).
- Whether voiio or Aon take third-party providers; wds.care; work-life-management.de (the brief lists these as gaps).
