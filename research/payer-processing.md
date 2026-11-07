# Insurer invoice processing (§ 302 SGB V) and MD assessment automation: incumbents, contract values, buying route
Task: A12 (fact-check fixes A19) | Date: 2026-11-07 | Status: draft

Follow-up to I5/I6 in `research/pain-industry.md` and to the critic review `research/reviews/2026-11-06-pain-industry.md` (issues 1–3, "missing evidence"). Main method: TED API v3, award notices (`can-standard`, `veat`) per procedure ID, plus the public tender documents of the new MD-IT framework (DTVP, no login needed). Overlaps with A11 (`research/hospital-billing-audits.md`, the hospital side of the same audits).

## Findings
- **§ 302 outsourcing is a closed market of a few incumbents, and a startup cannot bid directly.** There are 13 award notices for insurer billing and bill-checking work (2024–2026). IQVIA Health System Services (formerly DAVASO) won 5 of them. The other winners were SPS Germany, GFS (2), mediakom, Abrechnungszentrum Emmendingen, GEOS and QuantCo; one winner is not named. Where the notice reports bids, each tender drew **1–3 bids**. One more tender (Salus BKK) drew 0 bids and was not awarded. Contract values: €5.48m (Pronova BKK), €6.48m (AOK BW), lots of €5.99m, €12.95m and €34.31m (IKK classic), and an €8.30m estimate (BAHN-BKK). Typical requirements are minimum turnover, three comparable references, and liability cover of €1–10m [A] (TED, table in §1). One more route is closed to private vendors: insurers can hand the work to a public-law body without a tender (BIG direkt gesund → Abrechnungszentrum Emmendingen under § 88 SGB X) [A] (TED 143948-2025).
- **Insurers are moving from paying a BPO (outsourced back office) to buying AI software and bringing the checking back in-house. That opens a software slot.**
  - DAK ran a market exploration (a prior-information notice, `pin-only`, not a tender) for "KI-basierte Rechnungsprüfungssoftware" for § 302, with the stated aim that the work "künftig wieder eigenständig erbracht werden" (TED 427316-2025) [A].
  - TK bought "DRG Scoring Software" for checking hospital bills from QuantCo (3 bids, 3 participation requests, Aug 2026; re-queried in A19) [A].
  - AOK Hessen kept only scanning and intake external (SPS) [A]. A search snippet says it took the checking itself back in-house from 1 Aug 2026 `[UNVERIFIED: snippet only]`.
  - BITMARCK, the IT provider of the BKK and Ersatzkassen insurers, runs a "KI-Marktplatz" with "KI-Produkte, entwickelt von Krankenkassen für Krankenkassen" [B]. *Inference:* the insurers' IT joint ventures are building rather than buying.
- **The largest new budget is on the MD side, and the law explicitly triggers it.** MD-IT GmbH, the central purchasing body of the 15 MDs plus DRV Knappschaft-Bahn-See, tendered a 48-month framework for **AI case summaries in hospital billing audits**. Lot 1 has a maximum value of **€88m**; bids are due **2 Dec 2026**. The stated reason is "die gesetzlich vorgesehenen Prüfquoten", which "mit den bisherigen Bearbeitungsverfahren nicht aufgefangen werden" can be [A] (TED 751925-2026 / 773326-2026; DTVP documents).
  - Eligibility rules out a startup bidding alone: average turnover ≥ **€5,000,000** (averaged since founding for firms <3 years old), ≥ **25 staff** on average in the business units involved, and 2 references with AI on sensitive data in multi-tenant operation [A] (DTVP form 04.1, re-read in A19).
  - Subcontracting is allowed (form 04.1), and so are bidder consortia and capacity borrowing ("Eignungsleihe", § 47 VgV) from a larger partner, who must then deliver the part for which its experience is borrowed [A] (DTVP 01 Angebotsbedingungen, § 15). *Inference:* a startup can only enter as subcontractor or consortium member next to a firm that meets the €5m / 25-staff bar.
- **The MDs' smaller AI buys show an entry path.** MD Nordrhein co-developed AI for rehabilitation assessments with eventus GmbH, a Munich assessment firm (Jan 2025). In Nov 2026 it re-tendered for AI support in malpractice reviews (TED 762721-2026, deadline 3 Dec 2026) [A]. MD Rheinland-Pfalz's AI care-assessment PoC drew **40 requests to participate** [A]. It was cancelled for "change of need" and then re-tendered. The re-tender asked for only **one** comparable GenAI reference, and a finished PoC counts as one; no minimum turnover appears in its TED selection fields [A].
- **The demand driver is people, not paper.** The 15 MDs employ 12,677 people (11,140.6 FTE), including 2,148.3 physician FTE. Hospital work takes about 36 % of the reviewer resources they spend on statutory health-insurance cases. The MDs handled 1,232,119 hospital billing audits under § 275c in 2025, and only 3.7 % of insurance-related opinions were produced externally [A] (MD Bund report 2024–2025).
- **The admin cap works both ways.** From 2027, an insurer's admin spending may only grow with the average change per insured person (§ 4 Abs. 5 SGB V). For 2026, material admin spending may grow at most 8 % over 2024 (§ 4 Abs. 6, BStabG) [A]. *Inference:* both outsourcing fees and new software count against the cap, so only tools that replace existing BPO fees or staff costs with measurable savings fit. PNOG (still a draft) slightly *reduces* care-assessment volume (an advice step before assessment, in 3,000–60,000 cases/yr) [A]. It is not a demand driver for MD tools.
- *Inference for A7/B1:* "outsourced § 302 invoice processing" fails knock-out K2 as a direct sale. "AI for payer/MD hospital-audit work" has proven spend and a deadline. The realistic startup routes are (a) a component or subcontract to one of the three MD-IT framework partners, (b) a small PoC tender of the MD RLP type, or (c) the hospital side (A11). All three are B2G with procurement lead times of ≥6–12 months.

## Details

### 1. § 302 / § 300 / § 301 billing tenders: who won, value, bids, access
All rows are TED notices [A], read via the API on 2026-11-07. "Bids" = `received-submissions-type-code=tenders`. Values are as stated in the notice. "1" or "0.01" means withheld; I do not report those.

| Buyer | Scope (type) | Notice (award) | Winner | Value | Bids | Access barriers in the notice |
|---|---|---|---|---|---|---|
| AOK Baden-Württemberg | Scanning and assembling invoices from bundled data sets (§ 302 / § 105 SGB XI) (**scan/intake**) | 366472-2026 | IQVIA Health System Services GmbH (large) | €6,480,000 | 3 (8 participation requests) | BSI TR-03138 RESISCAN mandatory |
| AOK Hessen | External document management: intake, imaging, data capture, DTA creation (**scan/intake**); 19,257,000 invoices / 4 yrs | 213218-2026 | SPS Germany GmbH (large) | not disclosed | 3 | €6m annual turnover (critic review) |
| BAHN-BKK | "Annahme, Aufbereitung, Prüfung und Retaxierung" of § 301a/302 invoices, payment, online tool (**billing check**); spend volume "knapp 423.836.651,42 € pro Jahr" | 500755-2025 | DAVASO GmbH (large) | est. €8,295,000 / 4 yrs (cn 269243-2025) | 2 | — |
| Pronova BKK | Data intake, checking **software** + price database, payment, archive; checking itself done by insurer staff ("Splittservice") | 572311-2024 | DAVASO GmbH (medium) | €5,482,000 (est. €3.2m) | 1 | — |
| IKK classic | HKP/care: approval tool + billing software, insurer checks ("Outtasking") | 32477-2024 | DAVASO GmbH (2 lots) | €5,990,428 + €12,951,709 | 2 / 1 | software hosted at BITMARCK |
| IKK classic | Heilmittel, transport, midwives (**outsourced check**) + aids software | 5516-2024 | not named in API | €34,313,634 | 1 | — |
| AOK Niedersachsen | Intake, scan, OCR, visual check, portal, ≥250 developer days (**intake + pre-check**) | 247921-2025 | DAVASO GmbH (medium) | not disclosed | 1 | — |
| AOK PLUS | Checking of Heilmittel, transport, rehab sport, HKP, care, aids (**billing check**) on the insurer's "os-care® claims" software; repeat direct award to 31 Oct 2031 | 758402-2026 | mediakom GmbH & Co. KG (large) | not disclosed | 1 | negotiated without competition (§ 14 Abs. 4 Nr. 9 VgV) |
| hkk | Pharmacy billing § 300 (**billing check**) | 737201-2026 | GFS mbH (large) | not disclosed | 3 | — |
| SBK | Pharmacy billing § 300 | 705454-2026 | GFS GmbH | est. €2,186,760 (procedure estimate `BT-27-Procedure`; award value withheld) | n/a | — |
| BKK mkk | Pharmacy billing § 300 + § 106d | 516024-2024 | Abrechnungszentrum Emmendingen (small) | not disclosed | 2 | — |
| vdek (for TK, KKH) | Maintenance of hospital-bill checking software "MeRep" | 406678-2024 | GEOS mbH (small) | not disclosed | 1 | ≥3 references, ≥1 in GKV (exclusion criterion) |
| TK | "DRG Scoring Software" to complement the rule base in hospital-bill checking | 546608-2026 | QuantCo Deutschland GmbH (medium) | not disclosed | 3 | criteria in tender docs (not opened) |
| Salus BKK | Hospital billing and checking § 301, 12 months | 513971-2026 | **no award, 0 bids** | — | 0 | — |
| BIG direkt gesund | Full § 301/302 processing | VEAT 143948-2025 | Abrechnungszentrum Emmendingen (direct, § 88 SGB X) | — | — | public-law in-house route; BIG then also published cn 189396-2025 (€250k turnover + 3 references); no award found |

Still open (no award notice yet): DAK "Abrechnungsprüfung HKPF, AKI und HHhi", processing "ca. 890 Mio. Euro" **net spend volume** a year (the volume checked, *not* the contract value) and 2.0m receipts. It is outsourced "weiterhin" (an incumbent exists), with a 48-month term (cn 396194-2026). Also open: AOK NordWest via gkv informatik, intake only, 24 months, "mindestens drei vergleichbaren Referenzprojekten" (cn 481787-2026). And AOK Rheinland/Hamburg, scan only, est. €10,000,000 / 24 months, ISO 9001 or 27001 and €10m liability cover (cn 518174-2026).

**Split asked for by the critic:** scan/intake BPO = AOK BW, AOK Hessen, AOK NordWest, AOK Rheinland/Hamburg, Pronova (scan software, cancelled for "ins-fund", TED 287998-2026). Billing check = BAHN-BKK, IKK classic, AOK PLUS, DAK, BIG, hkk/SBK/BKK mkk (§ 300). Hospital-bill check (§ 301) = TK, vdek MeRep, Salus.

*My math:* BAHN-BKK pays an estimated €8.295m over 4 years = €2.07m/yr to check €423.8m/yr of claims, i.e. ≈ 0.49 % of the volume checked. This is one data point, not a market rate.

### 2. Incumbents
- **IQVIA Health System Services GmbH (formerly DAVASO, Leipzig).** "Seit 2021 ist DAVASO Teil der IQVIA Unternehmensgruppe". It has "rund 1.350 Mitarbeitenden" and handles "einen großen Teil des Abrechnungsmanagements der etwa 230.000 Leistungserbringer … Gesamtabrechnungsvolumen von ca. 25 Mrd. Euro" [B] ([DAVASO PR, Jun 2025](https://www.gesundheit-adhoc.de/wp-content/uploads/2025/06/DAVASO_Pressemitteilung_BGF_AOKPLUS_20250612f.pdf)). In 2024 it reported "rund 55.000 registrierte direktabrechnende Leistungserbringer" on its portal [B] (older figure: [IKK classic/DAVASO PR, Mar 2024](https://www.ikk-classic.de/assets/408/15408_ikkc_web_pdf.pdf)). TK names it its central data-intake point, "mit der Datenannahme, Rechnungsprüfung und -bezahlung … beauftragt" [B] ([TK](https://www.tk.de/leistungserbringer/personengruppen/abrechnungen/ext-dl-iqvia-2058196)). AOK BW's 2026 award went to "IQVIA Health System Services GmbH", the renamed entity (TED 366472-2026) [A].
- **DDG GmbH (Essen)** is BARMER's billing office for Heilmittel [B] ([BARMER](https://www.barmer.de/leistungserbringer/gesundheitsbereiche/heilmittel/abrechnungsstelle-heilmittel-1274132)).
- **GFS mbH (Radebeul)** does "Rechnungsbezahlung und Rezeptprüfung für Arzneimittelabrechnungen nach § 300 SGB V" for DAK [B] ([DAK](https://www.dak.de/leistungserbringer-portal/apotheken/rezeptpruefung-rechnungsbezahlung-gfs_64034)), and won hkk and SBK in 2026 [A]. A trade-press snippet says a Munich hedge fund took GFS over `[UNVERIFIED: snippet only]`.
- **SPS Germany (Swiss Post Solutions)**, **mediakom**, **Abrechnungszentrum Emmendingen** (an "Eigenbetrieb des BKK Landesverbandes Süd", i.e. public-law) and **GEOS** each appear once or twice [A].
- **Software layer:** the IT joint ventures. gkv informatik buys on behalf of AOK NordWest (TED 481787-2026) [A]. An older article describes it as a joint venture whose members include Barmer and HEK [B, >3 years old] ([cio.de](https://www.cio.de/article/3671890/gkv-informatik-stellt-kostenverrechnung-neu-auf.html)). BITMARCK hosts IKK classic's billing software (TED 32477-2024) [A]. BITMARCK piloted "bitDetect", ML scores for "DRG-Prüfung: Scores, die die … Rechnungsprüfung über die [MD]" in 2022 [B, >3 years old] ([BITMARCK slides 2022](https://www.bitmarck.de/fileadmin/Infothek/Veranstaltungen/Kundentag_PowerPoints/BITMARCK-Kundentag_2022_KI-gest%C3%BCtzte_Entscheidungsprozesse.pdf)). In 2025 it built "zentrale Plattformen für KI-Life-cycle-Management und Chatbots" and a "KI-Partnerschaft" with DAK [B] ([BITMARCK annual report 2025](https://www.bitmarck.de/fileadmin/Infothek/downloads/Gesch%C3%A4ftsbericht_2025_Final.pdf)).
- **New entrants:** caery automates "Leistungsprüfung, Abrechnung und Auszahlung" and sells through the Telekom channel [B] ([Telekom, Sep 2026](https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken)). I found no caery customer. QuantCo won the TK tender above [A].
- **[C] Incumbent staff:** DAVASO on kununu has a score of 3.2 from 361 reviews and 50 % recommendation. One excerpt: "Viel Leistungsdruck" ([kununu](https://www.kununu.com/de/davaso/kommentare)). This signals a labour-intensive model under pressure, not buyer pain.

### 3. MD side: workload and AI purchases
- **Capacity [A]** ([MD Bund report 2024–2025, as of 1 Jun 2026](https://md-bund.de/fileadmin/dokumente/Publikationen/Richtlinien_MDS_MD_Bund/Bericht_Taetigkeit_Personalausstattung_MD_GKV_2024_2025.pdf)):
  - "der 15 Medizinischen Dienste"; 12,677 people / 11,140.6 FTE at 31 Dec 2025: 2,148.3 physician FTE, 4,851.7 care-assessor FTE, 474.8 coding-specialist FTE.
  - 2,812,183 insurance-related opinions in 2025, of which 1,252,253 on hospital services. 1,232,119 audits of hospital treatment under § 275c.
  - Hospital services (incl. billing audits) take "rund 36 %" of reviewer resources in individual cases.
  - External share: 3.7 % overall, 3.5 % for hospital services, 60.4 % for dentistry.
  - *Inference:* the MDs do almost everything in-house, so their lever is productivity tools, not outsourcing. This updates A11's 2023 figure (2,135 physician FTE).
- **AI and assessment-related tenders, 2024–2026 [A] (TED):**

| MD / buyer | What | Notice | Result |
|---|---|---|---|
| MD Nordrhein | AI co-development for assessments, first applications for inpatient rehab (§ 40 SGB V) | 95051-2025 | eventus GmbH (small), 9 submissions (type not labelled), value withheld |
| MD Nordrhein | AI assistant for malpractice reviews (analyse records, draft opinions) | cn 762721-2026 | open, bids due 3 Dec 2026 |
| MD Rheinland-Pfalz | GenAI: transcribe interview audio → draft care-assessment opinion; PoC → 1 site → roll-out (60 months) | 483916-2025 | **no award, "chan-need"**, 40 requests to participate; re-tendered (cn 500590/543912-2025), no award notice yet |
| MD Bayern | Chatbot and AI search | cn 63363/126222-2025 | no award notice found; required ≥€100,000/yr in-field turnover, >4 staff, 3 references |
| MD-IT (all MDs) | Speech recognition (cloud) | 94411-2026 | 4voice GmbH, €2,500,000 / 48 months, 2 bids |
| MD-IT (all MDs) | Video assessment framework, max. 5,000 licences/month | 276227-2025 | arztkonsultation ak GmbH, €95,940 tender value, 3 bids |
| MD-IT (15 MDs + DRV KBS) | AI case summary for hospital billing audits (Lot 1), AI governance (Lot 2), management-system software (Lot 3) | cn 751925 / 773326-2026 | open, bids due 2 Dec 2026; max. €88m / €26m / €7m (Lot 3: the cn 751925 said €5m; change notice 773326-2026 of 6 Nov 2026 corrects it to "7.000.000 EUR netto") |
| MD Bayern | Outsourced care assessments (file-based + phone) | 180585-2024 | innovas GmbH, €4,320,000, 1 bid |
| MD Hessen | Outsourced care assessments § 18 SGB XI | 444001-2024 | eventus GmbH (large), 1 bid |
| MD Niedersachsen | ~20,000 outsourced DRG audits, 4 months | cn 383478-2026 | see A11 (€2m; turnover + references) |

- *Inference:* eventus appears on both sides, as an external assessor (MD Hessen) and as an AI co-developer (MD Nordrhein). A Munich assessment firm is thus already the incumbent partner for MD AI. Its HQ is in Munich per a job ad seen as a snippet only `[UNVERIFIED]`.

### 4. MD-IT framework "KI-RV 2026" (read from the public tender documents)
Source: DTVP project CXP4YE6M1SX, documents 03.1, 03.7, 04.1, 07.1 (downloaded 2026-11-07) [A]. The critic could not re-read DTVP; in A19 I re-downloaded 01 (Angebotsbedingungen V1.2), 04.1 and Bieterinformation Nr. 1–2 (4 and 6 Nov 2026) and re-checked the eligibility rules and the lot values (Lot 1 €88m incl. €10m for extensions; Lot 2 €26m; Lot 3 €7m; deadline "02.12.2026, 10:00 Uhr"). Version 1.1 of the documents replaced 1.0 on 4 Nov 2026; the deadline is unchanged.
- **Why:** "Der Bedarf ergibt sich aus der gestiegenen Zahl der Prüfaufträge im Bereich der stationären Begutachtung. Die gesetzlich vorgesehenen Prüfquoten … führen zu einer Belastung, die mit den bisherigen Bearbeitungsverfahren nicht aufgefangen werden kann."
- **What:** a hosted web app, opened from the existing case system. It provides document search and filtering, a case summary and a case chat. The summary "darf keine Handlungsanweisung oder verbindliche Entscheidungsempfehlung darstellen". The AI Act is named, including the high-risk scenario. MCP is allowed as an interface.
- **Award model:** a framework with the **3** best bidders. Each MD is bound to a ranking for focus A (preparing case material: 12 MDs + DRV KBS) or focus B (embedded support of assessment: MD Nordrhein and MD Sachsen-Anhalt). MD Niedersachsen chooses per call-off. No minimum purchase is guaranteed.
- **Pricing basis:** price per audit order, plus a monthly fee per MD (16 bodies × 48 months; 220 users per body assumed). Calculation basis: 500,000 user-triggered and 2,700,000 preparatory generations a year, 1.33 generations per order.
  - *My math:* (500,000 + 2,700,000) / 1.33 ≈ **2.4m orders a year**, about twice the 1,232,119 § 275c audits of 2025. This is a scoring assumption, not a forecast.
  - €88m / 4 years = **€22m/yr ceiling** for Lot 1 across all MDs (a cap, not expected spend).
- **Eligibility (Lot 1):** average turnover ≥ €5,000,000 net over the last 3 years (or since founding); ≥ 25 staff (average, business units involved); liability cover ≥ €2,000,000 per claim (a commitment to take it out on award is enough); ≥ 2 references with three features (sensitive document data, AI components, productive multi-tenant operation): one must show all three, the other at least two. A **finished pilot with sensitive data under the controller's supervision may replace one of the two references** (then only feature 1 is needed for the pilot, and the other reference must show all three). *Correction (A19):* the earlier text said a pilot replaces a "3rd" reference; the form calls the slot "Referenz Nr. 3" but it substitutes one of the two required references. Subcontractors, consortia and capacity borrowing (§ 47 VgV) are allowed.

### 5. Buying routes (summary)
| Route | Example | Startup access |
|---|---|---|
| EU open tender by the insurer/MD (≥ €216,000 net for services, 2026–27 [B] [IHK](https://www.ihk.de/hannover/hauptnavigation/unternehmensfoerderung/oeffentliches-auftragswesen/aktuell-auftragswesen/neue-schwellenwerte-fuer-eu-ausschreibungen-fuer-2026-und-2027-6927176)) | BAHN-BKK, AOK BW, TK | Low: turnover/reference thresholds; 1–3 bidders, incumbents |
| Central purchasing by the IT joint venture | MD-IT for all MDs; gkv informatik for AOK NordWest | Very low alone (MD-IT: €5m turnover, 25 staff); possible as subcontractor or consortium member / via capacity borrowing from a qualified partner |
| Public-law in-house delegation (§ 88 SGB X; § 197b SGB V allows third parties if "wirtschaftlicher" [A] [§ 197b](https://www.buzer.de/197b_SGB_V.htm)) | BIG → Abrechnungszentrum Emmendingen | None (bypasses the market) |
| Repeat/direct award to incumbent | AOK PLUS → mediakom to 2031 | None until 2031 |
| Small PoC tender with light criteria | MD RLP (1 PoC reference, no turnover minimum seen) | **Medium**: the realistic first contract |
| Subcontract/channel | caery via Telekom; subcontractor to an MD-IT framework partner | Medium; margin and IP risk |
| Below EU threshold (national procurement; Bavaria direct award ≤ €100k, see red-team review) | not observed for insurers in TED (by definition) | Possible for a PoC, `[UNVERIFIED]` for insurers |

### 6. Admin cap and PNOG
- **§ 4 Abs. 5 SGB V (from 2027):** "dürfen sich die Verwaltungsausgaben einer Krankenkasse … nur nach Maßgabe der … durchschnittlichen Veränderungsrate je Versicherten erhöhen". IT-security spending is exempt.
- **§ 4 Abs. 6 (2026):** "die sächlichen Verwaltungsausgaben … nicht um mehr als 8 Prozent gegenüber dem Jahr 2024" (version per BStabG, in force 30 Jul 2026) [A] ([§ 4 SGB V](https://www.buzer.de/4_SGB_V.htm)).
- There are now 92 statutory insurers ("92 Ergebnisse (Stand: 07.11.2026)") [A] ([GKV-SV list](https://www.gkv-spitzenverband.de/service/krankenkassenliste/krankenkassen.jsp)). This corrects "93" in `pain-industry.md`.
- *Inference:* BPO fees are material admin spending, so a tool that cuts the fee per invoice fits under the cap, while an add-on that adds cost does not. The DAK and AOK Hessen moves (§ 1) fit this reading. The MDs are funded by insurer contributions, so the same pressure applies indirectly.
- **PNOG (cabinet draft, not law):**
  - It raises care-grade thresholds. IGES estimates a recognition drop "um knapp 12 Prozent" to "etwa 22 Prozent" for first assessments.
  - It adds an advice step before assessment, with "rund 3.000 bis 60.000 jährlichen Anwendungsfällen" and €0.19–3.8m/yr relief.
  - Net admin effect: "jährliche Entlastungen in Höhe von knapp 70 Millionen Euro" for the social insurance branches.
  - [A] ([BMG cabinet draft PNOG](https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Gesetze_und_Verordnungen/GuV/P/Kabinett-GE_Pflegeneuordnungsgesetz_PNOG.pdf)).
  - *Inference:* PNOG makes care assessments more contested (thresholds), not more numerous. It is a weak driver for MD care-assessment AI, unlike the BStabG audit quotas on the hospital side.

### 7. Counter-evidence and risks
- Concentration: IQVIA HSS won 5 of the 13 awards and is the single largest outsourcer. MD AI work goes to eventus, 4voice and arztkonsultation. A startup faces incumbents with GKV references in every lane.
- Build-in-house: BITMARCK's "von Krankenkassen für Krankenkassen" marketplace and its 2022 bitDetect pilot mean the obvious ML use cases (DRG scores) may already be in-house at BKK/Ersatzkassen insurers.
- Cancellations: MD RLP (change of need), Pronova scan software (no funds), Salus (0 bids). Public buyers cancel often, so pipelines slip.
- The MD-IT framework locks in up to 3 vendors for 4 years from ~2027. If a startup is not inside a winning bid, the largest MD budget is gone until ~2031.
- Lünendonk (A5): insurers expect few short-term savings from AI [B]. This conflicts with the "cap forces automation" reading.

## Gaps / [UNVERIFIED]
- AOK Hessen taking billing checks back in-house from 1 Aug 2026: search snippet only (aok.de news is JS-rendered; WebFetch DNS fails).
- Contract values withheld ("1"/"0.01") for most awards. The national size of § 302 outsourcing is unknown. DAVASO's €25bn is billing volume, not revenue. IQVIA HSS revenue (Bundesanzeiger) not checked.
- Winner of IKK classic 5516-2024 (€34.3m) not named in the API. No award notice yet for DAK 396194-2026, BIG 189396-2025, gkv informatik 481787-2026, AOK Rheinland/Hamburg 518174-2026 or MD RLP 543912-2025.
- TED covers only tenders above the EU threshold. Below-threshold insurer buys and direct awards (except VEATs) are invisible.
- caery customers and funding, QuantCo's TK contract value, and gkv informatik's current shareholders: not found.
- AOK Systems: its role was not checked. AOK PLUS's claims software is called "os-care® claims" (TED 758402-2026); that this is AOK Systems' oscare product is `[UNVERIFIED]`.
- eventus HQ in Munich and the GFS ownership change: snippets only.
- MD-IT Lot 1 award criteria weights and the Erprobung (live test) conditions were not read in full (doc 03.5 downloaded, not analysed).
- No [C] buyer voices (B2B pain is not discussed in public forums; Reddit not used). Stage D interviews with insurer billing heads and MD heads are needed.

## Sources
- https://api.ted.europa.eu/v3/notices/search — all TED notices cited (cn/can/veat: 366472-2026, 213218-2026, 500755-2025, 269243-2025, 572311-2024, 32477-2024, 5516-2024, 247921-2025, 758402-2026, 737201-2026, 705454-2026, 516024-2024, 406678-2024, 261425-2024, 546608-2026, 746499-2025, 513971-2026, 143948-2025, 189396-2025, 396194-2026, 481787-2026, 518174-2026, 287998-2026, 427316-2025, 95051-2025, 762721-2026, 483916-2025, 543912-2025, 63363-2025, 94411-2026, 276227-2025, 751925-2026, 773326-2026, 180585-2024, 444001-2024, 383478-2026), accessed 2026-11-07
- https://www.dtvp.de/Satellite/public/company/project/CXP4YE6M1SX/de/documents — MD-IT KI-RV 2026 tender documents (03.1, 03.7, 04.1, 07.1), accessed 2026-11-07
- https://www.dtvp.de/Satellite/public/company/project/CXP4YE6M1SX/de/documents — re-read in A19: 01_Angebotsbedingungen V1.2 (lot maxima, deadline, § 15 consortia / Eignungsleihe), 04.1 eligibility form, Bieterinformation Nr. 1 (4 Nov 2026) and Nr. 2 (6 Nov 2026); accessed 2026-11-07
- https://md-bund.de/fileadmin/dokumente/Publikationen/Richtlinien_MDS_MD_Bund/Bericht_Taetigkeit_Personalausstattung_MD_GKV_2024_2025.pdf — MD staff, volumes, external share, accessed 2026-11-07
- https://www.buzer.de/4_SGB_V.htm — § 4 Abs. 5 and 6 SGB V, accessed 2026-11-07
- https://www.buzer.de/197b_SGB_V.htm — § 197b SGB V, accessed 2026-11-07
- https://www.buzer.de/302_SGB_V.htm — § 302 SGB V scope, accessed 2026-11-07
- https://www.gkv-spitzenverband.de/service/krankenkassenliste/krankenkassen.jsp — 92 insurers, accessed 2026-11-07
- https://www.bundesgesundheitsministerium.de/fileadmin/Dateien/3_Downloads/Gesetze_und_Verordnungen/GuV/P/Kabinett-GE_Pflegeneuordnungsgesetz_PNOG.pdf — PNOG admin effects and assessment changes, accessed 2026-11-07
- https://www.gesundheit-adhoc.de/wp-content/uploads/2025/06/DAVASO_Pressemitteilung_BGF_AOKPLUS_20250612f.pdf — DAVASO/IQVIA size, accessed 2026-11-07
- https://www.ikk-classic.de/assets/408/15408_ikkc_web_pdf.pdf — DAVASO portal users (Mar 2024), accessed 2026-11-07
- https://www.tk.de/leistungserbringer/personengruppen/abrechnungen/ext-dl-iqvia-2058196 — TK uses IQVIA HSS, accessed 2026-11-07
- https://www.barmer.de/leistungserbringer/gesundheitsbereiche/heilmittel/abrechnungsstelle-heilmittel-1274132 — BARMER uses DDG, accessed 2026-11-07
- https://www.dak.de/leistungserbringer-portal/apotheken/rezeptpruefung-rechnungsbezahlung-gfs_64034 — DAK uses GFS, accessed 2026-11-07
- https://www.bitmarck.de/fileadmin/Infothek/downloads/Gesch%C3%A4ftsbericht_2025_Final.pdf — BITMARCK KI-Marktplatz, DAK partnership, accessed 2026-11-07
- https://www.bitmarck.de/fileadmin/Infothek/Veranstaltungen/Kundentag_PowerPoints/BITMARCK-Kundentag_2022_KI-gest%C3%BCtzte_Entscheidungsprozesse.pdf — bitDetect pilot (2022), accessed 2026-11-07
- https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken — caery via Telekom, accessed 2026-11-07
- https://www.cio.de/article/3671890/gkv-informatik-stellt-kostenverrechnung-neu-auf.html — gkv informatik joint venture (old), accessed 2026-11-07
- https://implisense.com/en/companies/md-it-gmbh-berlin-DE0QCWR6CI57 — MD-IT purpose "IT-Dienstleistungen für die Gesellschafter" (register text via aggregator), accessed 2026-11-07
- https://www.ihk.de/hannover/hauptnavigation/unternehmensfoerderung/oeffentliches-auftragswesen/aktuell-auftragswesen/neue-schwellenwerte-fuer-eu-ausschreibungen-fuer-2026-und-2027-6927176 — EU threshold €216,000, accessed 2026-11-07
- https://www.kununu.com/de/davaso/kommentare — DAVASO staff reviews [C], accessed 2026-11-07
- Snippet only (not opened): https://www.aok.de/gp/news-pflege/newsdetail/neuer-dienstleister-fuer-die-rechnungsannahme-ab-august-2026 (AOK Hessen insourcing); apotheke-adhoc (GFS owner); mydrg.de job ad (eventus HQ)
