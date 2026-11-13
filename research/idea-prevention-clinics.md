# Idea check: prevention clinics ("Medicine 3.0") in Munich
Task: C2 (researcher) | Date: 2026-11-13 | Status: draft

**Verdict: drop the clinic. No deep dive. Keep one asset-light variant alive only as a cheap test: an employer prevention programme, asked about in the same HR conversations as L01.**
Scores (method: `research/scoring.md` v3): own clinic 50/90, consumer platform via partner practices 52/90, employer programme 54/90 (49 in the sensitivity run, "unproven"). L01 has 66/62. Sources were opened on 2026-11-12 unless marked "snippet only".

## Findings
- **People pay, so demand is real. Benefit for healthy adults is not shown.** YEARS (Berlin) charges €1,990 / €7,600 / €16,900 per check-up day [B] ([YEARS](https://www.years.co/en/blog/longevity-clinics-programs-costs)). Neko had revenue of SEK 157m in 2025 [B] ([Finwire/Placera](https://www.placera.se/telegram/daniel-eks-neko-health-sakrar-miljardlan-fran-agare-breakit-20260710)). Against that: general health checks "have little or no effect on the risk of death from any cause (high-certainty evidence)" (Cochrane, 15 trials, 251,891 participants) [A] ([Cochrane](https://www.cochrane.org/evidence/CD009009_general-health-checks-reducing-illness-and-mortality)). Whole-body MRI in symptom-free people finds cancer in 1.57 % and "may lead to unnecessary investigations" (10 studies, 9,024 people) [A] ([Eur Radiol 2026](https://pubmed.ncbi.nlm.nih.gov/40884613/)).
- **The clinic model burns capital, and the German example failed.** Neko's net loss tripled to SEK 677m in 2025 on SEK 157m revenue, with 433 staff [B] (Finwire/Placera, above). Aware Health (Berlin; blood tests, €450 a year, 25–45 own sites, about $15m raised in 2022) filed for insolvency in May 2026; Aeon took over the business "für gerade einmal 100.000 Euro" [B] ([Apotheke Adhoc, 1 Jun 2026](https://www.apotheke-adhoc.de/nachrichten/detail/markt/blutanalysen-dm-partner-ist-pleite/), [follow-up](https://www.apotheke-adhoc.de/nachrichten/detail/markt/keine-blutanalyse-mehr-bei-dm/)). Forward (US) shut down in Nov 2024 after raising $400m [B] ([Maginative](https://www.maginative.com/article/ai-healthcare-startup-forward-shuts-down/)).
- **A company may not run a medical practice in Bavaria.** "Die Führung einer ärztlichen Praxis in der Rechtsform einer juristischen Person des privaten Rechts oder einer Personenhandelsgesellschaft ist nicht statthaft" (Art. 18 Abs. 1 Satz 2 HKaG, text valid from 1 Jan 2025) [A] ([gesetze-bayern.de](https://www.gesetze-bayern.de/Content/Document/BayHKaG-18)). A non-physician founder with €10k cannot own the clinic. A physician must own and run the practice, or the company only brokers.
- **Munich is already served, and the best-funded player arrives in 2027.** Aeon (Zurich, seed funding above $14m) sells whole-body MRI check-ups in Munich through the partner practice Beyond Imaging [B] ([Aeon Munich](https://aeon.life/de-de/mri-munchen/), [TFN](https://techfundingnews.com/swiss-healthtech-aeon-acquires-germanys-aware-health-as-seed-funding-tops-14m/)). Neko: "Germany represents Neko's next international market, with launch planned for 2027" (job ad, Berlin, posted 28 May 2026) [B] ([Atomico careers](https://careers.atomico.com/companies/neko-health/jobs/80662143-medical-director)). Local incumbents: Diagnostik München, TUM "Manager-Check", wellabe (now Mavie).
- **Insurers and tax law do not carry the price.** GKV pays only the statutory check-up (§ 25 SGB V) [A]. PKV model terms cover early detection "nach gesetzlich eingeführten Programmen" [B] ([MB/KK](https://www.pkv.de/fileadmin/user_upload/PKV/3_PDFs/ABV_und_MB/MB-KK.pdf)). Employer-paid check-ups are tax-free only "höchstens bis zu dem Betrag, den die gesetzlichen Krankenkassen für diese Leistungen erstatten würden" (BMF 2021, Rz. 37); the 1982 ruling that exempted executive check-ups was removed from the 2026 wage-tax notes [B] ([IWW, 28 Jul 2026](https://www.iww.de/lgp/lohnsteuer/arbeitgeberleistungen-vorsorgeuntersuchungen-und-check-ups-verschaerfung-der-lohnsteuerpflicht-f175376)).
- **Employers do buy prevention, in small tickets, from vendors with references.** WBM (Berlin housing company) tendered a framework for executive check-ups in Aug 2026 [A] (TED 594202-2026). IKK classic awarded health days for its own staff to insa Gesundheitsmanagement for €604,750 (4 bids) [A] (TED 664823-2026). Both require references. Kassen spent €281,956,037 on workplace health promotion in 2024 [A] ([Präventionsbericht 2025](https://www.vdek.com/content/dam/vdeksite/LVen/HES/Presse/2025_GKV_MD_Praventionsbericht_barrierefrei.pdf)).
- **Founder fit is weak for the clinic.** The core is physicians, devices and premises, not AI or automation. The CEO works in Lisbon until Sep 2027 (`founder-brief.md`).

## Details

### 1. What such clinics offer and charge
| Operator | Where | Offer | Price | Funding / scale | Grade |
|---|---|---|---|---|---|
| YEARS | Berlin (clinic open 2 years; capacity +50 % in 2026) | One-day check-up: 87–230+ biomarkers, whole-body MRI, liquid biopsy, genome | Core €1,990; Evolve €7,600; Ultimate €16,900 | Funding not found | [B] [prices](https://www.years.co/en/blog/longevity-clinics-programs-costs), [press release](https://www.webdisclosure.com/press-release/years-marks-two-years-since-clinic-opening-and-expands-capacity-by-50-KCrtvhgTr5H) |
| Aeon (MRI Health Holding AG) | Zurich; DE sites Berlin, Hamburg, Düsseldorf, Köln, Frankfurt, Stuttgart, München | Whole-body MRI + blood panel + app, done at partner practices | Not readable (JS page) | €8.2m seed (Jun 2025), total above $14m (Sep 2026); "live in Germany since early 2026"; own data cover 2,731 people 2022–2026 | [B] [sites](https://www.aeon.life/de-de/standorte/), [tech.eu](https://tech.eu/2025/06/04/aeon-raises-eur82m-to-bring-full-body-preventive-check-ups-to-the-masses/), [TFN](https://techfundingnews.com/swiss-healthtech-aeon-acquires-germanys-aware-health-as-seed-funding-tops-14m/), [home](https://www.aeon.life/de) |
| Aware Health | Berlin, 25–45 sites, dm pilot | Blood tests, 99 biomarkers | €450 a year; single tests €9.95–69.95 | About $15m in 2022; insolvent May 2026; sold for €100,000 | [B] Apotheke Adhoc (above) |
| Neko Health | Stockholm, London, New York; Germany planned 2027 | Body scan with own hardware, no MRI | £300 (UK); about €240 (Sweden) | $260m Series B at $1.8bn (Jan 2025); waitlist above 100,000; 2025: revenue SEK 157m, net loss SEK 677m | [B] [TechCrunch](https://techcrunch.com/2025/01/22/neko-the-body-scanning-startup-co-founded-by-spotifys-daniel-ek-snaps-up-260m-at-a-1-8b-valuation), [heise](https://heise.de/-10254073), Finwire/Placera |
| AYUN | Zurich | Walk-in longevity clinic | CHF 3,134 starter (snippet only) | "More than 1,500 clients, CHF 2.7 million in revenue"; now raising by crowdfunding (Oct 2026) | [B] [AYUN](https://www.ayun.ch/) |
| Function Health | US | Lab-test membership, MRI add-on at 130 sites | $365 a year (snippet only) | $298m Series B at $2.5bn (Nov 2025) | [B] [TechCrunch](https://techcrunch.com/2025/11/19/function-health-closes-298m-series-b-at-a-2-5b-valuation-launches-medical-intelligence) |
| Forward | US, 19 clinics | Subscription primary care, "CarePods" | — | Raised $400m; under $100m revenue since founding; closed Nov 2024 | [B] Maginative (above) |
| Lanserhof, Metamedicum (ex Preventicum) | Tegernsee, Sylt; Essen, Düsseldorf | Medical spa; executive check-ups | €7,000–50,000+; €2,000–7,000 (competitor's estimates) | Established | [B] YEARS overview (a competitor's page) |

My math: AYUN CHF 2.7m ÷ 1,500 clients = CHF 1,800 per client (period not stated). Neko 2025 loss ÷ revenue = 677 ÷ 157 = 4.3.

Inference: two models exist. Own clinics with own devices (Neko, YEARS) need tens of millions. The broker model (Aeon) needs far less, but Aeon holds it in Munich, and the one German company that tried recurring tests (Aware) ended in an asset sale.

### 2. Who pays in Germany
| Payer | What is paid today | Evidence | Reading for a startup |
|---|---|---|---|
| Self-pay | IGeL turnover "mindestens 2,4 Milliarden Euro" a year (forsa survey of 2,013 insured; all specialties, not check-ups alone) | [B] [Ärzteblatt, 3 Dec 2024](https://www.aerzteblatt.de/nachrichten/156146/IGeL-Umsatz-uebersteigt-laut-Erhebung-Zwei-Milliarden-Schwelle) | Real money, but the check-up share is not sized |
| GKV | Check-up under § 25 SGB V. Use is low: 19.2 % of AOK NordWest insured in Schleswig-Holstein in 2024 | [A] [§ 25](https://www.gesetze-im-internet.de/sgb_5/__25.html); [B] [AOK NordWest](https://www.aok.de/pp/fileadmin/bereiche/nordwest/Presse/Dokumente/2025/2025-08-13_checkup35_sh_pm.pdf) | No route for extended diagnostics |
| GKV prevention budget | €686,182,779 in 2024: workplace €281,956,037, courses €218,409,854, settings €185,816,888 | [A] Präventionsbericht 2025 | Pays courses and workplace programmes, not clinics |
| PKV (8.74m fully insured) | Early detection under statutory programmes; more only by tariff | [B] [MB/KK § 1](https://www.pkv.de/fileadmin/user_upload/PKV/3_PDFs/ABV_und_MB/MB-KK.pdf), [PKV](https://www.pkv.de/verband/presse/pressemitteilungen/private-krankenversicherung-auf-wachstumskurs-fast-jeder-zweite-deutsche-privatversichert/) | Partial, per tariff; services "auf Verlangen" must be marked on the bill (GOÄ) [B] ([BÄK](https://www.bundesaerztekammer.de/themen/aerzte/honorar/goae-ratgeber/1-anwendungsbereich/leistungen-auf-verlangen)) |
| Employers, direct | Executive check-ups under framework contracts (TUM: billed by GOÄ, "Die Kosten trägt das jeweilige Unternehmen"); WBM tender; IKK classic health days €604,750 | [B] [TUM](https://www.sport.mri.tum.de/images/files/downloads/tum-sportmedizin-betriebliche-gesundheitsfoerderung.pdf); [A] TED 594202-2026, 664823-2026 | Proven spend; references required in both tenders |
| Employers, via company health insurance (bKV) | 60,600 firms and over 2.8m people at end 2025, +16 % firms in a year; Allianz new business +58 % | [B] [PKV-Verband](https://www.pkv.de/themen/krankenversicherung/betriebliche-krankenversicherung/), [Allianz](https://www.allianz.de/presse/mitteilungen/starkes-bkv-wachstum-jeder-dritte-neukunde-waehlt-die-allianz/) | Growing channel, held by insurers. YEARS already points employers to "Allianz company health insurance" |
| Tax | €600 a year tax-free only for measures meeting §§ 20, 20b SGB V | [A] [§ 3 Nr. 34 EStG](https://www.gesetze-im-internet.de/estg/__3.html) | Extended check-ups count as taxable wage above the GKV amount (IWW, above) |

### 3. Regulation
| Topic | Rule | Source | Effect |
|---|---|---|---|
| Who may run a practice (Bavaria) | No private-law company or commercial partnership. The Bavarian Constitutional Court upheld the ban in 1999 | [A] Art. 18 HKaG; [B] [Bayerisches Ärzteblatt 10/2015](https://www.bayerisches-aerzteblatt.de/fileadmin/aerzteblatt/ausgaben/2015/10/einzelpdf/BAB_10_2015_506_508.pdf) | Physician-owned practice needed |
| MVZ | Only physicians, hospitals, dialysis providers, practice networks, non-profits or municipalities may found one. Investors therefore buy a hospital first | [A] [§ 95 Abs. 1a SGB V](https://www.gesetze-im-internet.de/sgb_5/__95.html); [B] [Capital 3/2024](https://lillian-care.de/wp-content/uploads/2024/02/Capital_3-2024_Seite_76_77_78_79_80_81.pdf) | Closed to this founder |
| Private clinic | Needs a concession | [A] [§ 30 GewO](https://www.gesetze-im-internet.de/gewo/__30.html) | Whether it fits an outpatient check-up centre: `[UNVERIFIED]` |
| Broker model | Aeon: "Wir vermitteln dir medizinische Behandlungen"; treatment happens "zwischen dir und der Gesundheitsfachperson direkt" | [B] [Aeon terms](https://aeon.life/de-de/nutzungsbedingungen/) | Legal template for an asset-light variant (inference; no legal opinion) |
| CT and X-ray screening | "Früherkennung … ist nur zulässig, wenn die Rechtsverordnung … dies vorsieht"; covers people without symptoms | [A] [§ 84](https://www.gesetze-im-internet.de/strlschg/__84.html), [§ 5 Abs. 16 StrlSchG](https://www.gesetze-im-internet.de/strlschg/__5.html) | Check-up imaging must be MRI or ultrasound |
| Evidence | Cochrane and Eur Radiol (Findings) | [A] | Benefit claims are hard to defend |
| Advertising (HWG, UWG) | No ruling on longevity or MRI check-up adverts found (1 search) | — | `[UNVERIFIED]` |

### 4. Capital need vs founder constraints
- MRI: about €750,000 to over €3,500,000 new, from about €160,000 used; installation about €350,000; running about €180,000 a year plus about €85,000 maintenance [B] ([medizinio](https://medizinio.de/medizintechnik/mrt/mrt-geraet)).
- Inference: an own clinic with imaging needs a seven-figure sum before the first customer, plus employed physicians. €10k, no clinical background and part-time work from Lisbon do not fit.

Asset-light variants:
| Variant | Buyer | Status |
|---|---|---|
| B. Consumer platform that brokers check-ups at partner practices | Self-payers | Taken by Aeon in Munich; Neko follows; Aware failed |
| C. Employer prevention programme (organised check-ups or health days, digital follow-up) | HR / benefits | Proven spend, but incumbents and reference rules |
| D. Software for private preventive practices | Practice owner | Only a foreign vendor page found (Pabau; snippet only). No purchase by a German practice found, so K1 is not shown |

### 5. Munich market and competitors
| Player | What | Source |
|---|---|---|
| Aeon × Beyond Imaging (Rosenheimer Str. 30) | Whole-body MRI check-up | [B] Aeon Munich |
| Diagnostik München | "Pionier der modernen Vorsorgemedizin"; check-ups with radiology, cardiology | [B] [kliniken.de](https://www.kliniken.de/krankenhaus/diagnostik-muenchen-4771K.html) |
| TUM Zentrum für Prävention und Sportmedizin | "Manager-Check" for companies | [B] TUM brochure |
| wellabe (Munich, 2018; Mavie Work Deutschland) | Mobile workplace check-ups, 60 values in 20 minutes; "around 100 B2B customers" in 2024; sold through AXA's bKV | [B] [Munich Startup](https://www.munich-startup.de/en/news/wellabe-acquired-by-mavie-from-austria), [AXA flyer](https://www.axa-betreuer.de/site/ao-rel2020-AXA/get/documents_E578891519/axade/medien/geschaeftskunden/betriebliche-krankenversicherung/produktflyer-wellabe.pdf) |
| Lanserhof Tegernsee, Deutsche Klinik für Prävention (Oberaudorf) | Stays and check-ups in the region | [B] YEARS overview |
| Biogena Plaza München | Opened 17 Sep 2026 (snippet only) | `[UNVERIFIED]` |

Inference: wellabe took six years to reach about 100 employer customers and then sold a majority. That is the realistic scale of variant C.

### 6. Online voices [C]
- Aware app (App Store DE): 60 ratings, average 4.3. Of the 21 latest reviews, 11 give 5 stars and 7 give 1 star ([feed](https://itunes.apple.com/de/rss/customerreviews/page=1/id=1609437818/sortby=mostrecent/json)). Themes in the 9 reviews with 1–2 stars (my count, overlapping): price (6), no appointments or too few sites (4).
  - "Endlich die Möglichkeit relevante Blutwerte regelmäßig zu checken ohne monatelang auf Termine zu warten oder sich beim Arzt rechtfertigen zu müssen." (Feb 2024)
  - "180€ im Jahr für 2 mal Blut abnehmen? … Einfach zum Arzt gehen, Termin machen, weniger zahlen" (Jun 2024)
  - "Nach dem Preisupdate Anfang 2026 ist der Service leider nicht mehr zu gebrauchen." (Apr 2026)
- Hacker News, one thread on Neko, 53 comments ([thread](https://news.ycombinator.com/item?id=40235129)); of the 10 top-level comments read, most are sceptical or questioning: "unnecessary scans can reveal what is otherwise benign findings … it can cause massive anxiety."
- wellabe app: 41 ratings, average 4.7. Reddit: 0 reddit.com hits in 1 search.
- Reading: convenience and control are valued, but price tolerance is low once the family doctor does it for free. Signal only, not sizing.

### 7. Score (`research/scoring.md` v3)
| Wedge | K1 / K2 | Pain ×3 | Market ×2 | WTP ×3 | Fit ×2 | Achiev. ×2 | Reg ×1 | Fund ×2 | Comp ×2 | Future ×1 | Base | R4 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| A. Own clinic, Munich, self-pay | Pass / pass (YEARS, Aeon) | 3 M | 3 M | 4 M | 2 M | 2 H | 3 M | 3 M | 1 H | 4 M | **50** | 50 |
| B. Consumer platform via partner practices | Pass / pass (Aeon, founded 2023) | 3 M | 3 M | 4 M | 3 M | 2 M | 3 M | 3 M | 1 H | 4 M | **52** | 52 |
| C. Employer prevention programme | Pass (WBM, IKK classic, TUM) / unproven (wellabe is from 2018; tenders need references) | 3 M | 3 M | 4 L → 3 | 3 M | 3 L | 4 M | 3 M | 2 H | 4 M | **54** | 49 |
| D. Software for preventive practices | K1 not shown | — | — | — | — | — | — | — | — | — | out | — |

Math: A = 9+6+12+4+4+3+6+2+4 = 50. B = 9+6+12+6+4+3+6+2+4 = 52. C = 9+6+9+6+6+4+6+4+4 = 54; R4 = 54 − 3 − 2 = 49.

Placement: L01 66/62, L07 63/58, L06 62/55, L03 59/52, L13 59/54, L29 57/53, L23 55/51, L26 52/45 (`research/shortlist.md`). All three wedges rank below the top 6. A and B are not "unproven": the evidence is good, and it says the field is expensive and taken. Scores are my judgement.

### 8. Cheapest tests
1. **Free, 10 minutes:** does the CEO know a physician in Munich (internal medicine, GP or radiology) who would own the practice? If not, A and B stop here.
2. **Inside the L01 HR conversations (needs C3 approval):** add two questions. "Do you pay for check-ups or prevention for staff, through whom, and at what budget per head?" "Is it bought through a bKV?"
3. **Desk, 1 session:** annual accounts of YEARS and wellabe/Mavie Work Deutschland in the Unternehmensregister; Aeon's German prices; any Neko Germany opening notice.
4. **Outward action, only if the idea stays alive:** one paid hour with a medical-law attorney on the broker model in Bavaria.

## Gaps / [UNVERIFIED]
- Neko's $700m round and New York price ($499): snippet only (nekohealth.com HTTP 429, radiologybusiness.com 403).
- Zoī (Paris, about €3,600 a year, about 1,000 members): snippet only.
- YEARS funding, customer numbers and accounts: not found. Aeon's German prices: not readable.
- FG Nürnberg ruling on check-ups (revision VI R 9/25 pending): snippet only.
- Whether § 30 GewO or a management-company structure lets a company run a check-up centre in Bavaria: not researched; legal opinion needed.
- No German figure for self-pay check-up spend. The €2.4bn is all IGeL and dates from 2024.
- Fraunhofer (TED 394188-2023) and BARMER (371071-2023) notices matched "Vorsorgeuntersuchungen"/"Check-up", but the API returned no description; not used.
- The Bavarian Präventionsfonds call (up to €500,000 per project, 90 % rate, sketches due 16 Oct 2026) is for exercise promotion and has closed [B] ([call](https://www.landkreis-pfaffenhofen.de/media/19808/stmgp_praeventionsfonds-foerdercall.pdf)). No grant route for a clinic was found.
- The Cochrane review's search ended in Jan 2018 (older than 3 years; still the current version found).

## Sources
All accessed 2026-11-12.
- https://www.years.co/en/blog/longevity-clinics-programs-costs — YEARS prices; estimates for Lanserhof, Preventicum [B]
- https://www.years.co/en/longevity-kliniken-deutschland — German provider overview; Aeon via partner clinics; Metamedicum [B]
- https://www.webdisclosure.com/press-release/years-marks-two-years-since-clinic-opening-and-expands-capacity-by-50-KCrtvhgTr5H — YEARS two years, +50 % capacity, Allianz bKV [B]
- https://www.aeon.life/de , https://www.aeon.life/de-de/standorte/ , https://aeon.life/de-de/mri-munchen/ , https://aeon.life/de-de/nutzungsbedingungen/ , https://aeon.life/de-de/impressum/ — Aeon offer, sites, Munich partner, broker terms, legal entity [B]
- https://tech.eu/2025/06/04/aeon-raises-eur82m-to-bring-full-body-preventive-check-ups-to-the-masses/ — Aeon €8.2m seed, insurer deals [B]
- https://techfundingnews.com/swiss-healthtech-aeon-acquires-germanys-aware-health-as-seed-funding-tops-14m/ — Aeon seed above $14m, Aware assets, founded 2023 [B]
- https://www.apotheke-adhoc.de/nachrichten/detail/markt/blutanalysen-dm-partner-ist-pleite/ — Aware insolvency, funding, prices [B]
- https://www.apotheke-adhoc.de/nachrichten/detail/markt/keine-blutanalyse-mehr-bei-dm/ — sale to Aeon for €100,000 [B]
- https://techcrunch.com/2025/01/22/neko-the-body-scanning-startup-co-founded-by-spotifys-daniel-ek-snaps-up-260m-at-a-1-8b-valuation — Neko Series B, waitlist, £300 [B]
- https://heise.de/-10254073 — Neko price in Sweden [B]
- https://www.placera.se/telegram/daniel-eks-neko-health-sakrar-miljardlan-fran-agare-breakit-20260710 — Neko 2025 revenue, loss, staff, €150m loan [B]
- https://careers.atomico.com/companies/neko-health/jobs/80662143-medical-director — Neko Germany launch planned for 2027 (via WebFetch) [B]
- https://www.ayun.ch/ — AYUN clients and revenue [B]
- https://techcrunch.com/2025/11/19/function-health-closes-298m-series-b-at-a-2-5b-valuation-launches-medical-intelligence — Function Health round [B]
- https://www.maginative.com/article/ai-healthcare-startup-forward-shuts-down/ — Forward shutdown [B]
- https://www.cochrane.org/evidence/CD009009_general-health-checks-reducing-illness-and-mortality — general health checks [A]
- https://pubmed.ncbi.nlm.nih.gov/40884613/ — whole-body MRI meta-analysis (abstract via NCBI E-utilities) [A]
- https://www.gesetze-bayern.de/Content/Document/BayHKaG-18 — Art. 18 HKaG [A]
- https://www.bayerisches-aerzteblatt.de/fileadmin/aerzteblatt/ausgaben/2015/10/einzelpdf/BAB_10_2015_506_508.pdf — GmbH ban, court ruling 1999 [B]
- https://www.gesetze-im-internet.de/sgb_5/__95.html , https://www.gesetze-im-internet.de/sgb_5/__25.html , https://www.gesetze-im-internet.de/gewo/__30.html , https://www.gesetze-im-internet.de/strlschg/__84.html , https://www.gesetze-im-internet.de/strlschg/__5.html , https://www.gesetze-im-internet.de/estg/__3.html — statutes [A]
- https://lillian-care.de/wp-content/uploads/2024/02/Capital_3-2024_Seite_76_77_78_79_80_81.pdf — investors need a hospital to own practices [B]
- https://www.pkv.de/fileadmin/user_upload/PKV/3_PDFs/ABV_und_MB/MB-KK.pdf — PKV model terms § 1 [B]
- https://www.bundesaerztekammer.de/themen/aerzte/honorar/goae-ratgeber/1-anwendungsbereich/leistungen-auf-verlangen — services on request under GOÄ [B]
- https://www.iww.de/lgp/lohnsteuer/arbeitgeberleistungen-vorsorgeuntersuchungen-und-check-ups-verschaerfung-der-lohnsteuerpflicht-f175376 — wage tax on check-ups [B]
- https://www.vdek.com/content/dam/vdeksite/LVen/HES/Presse/2025_GKV_MD_Praventionsbericht_barrierefrei.pdf — GKV prevention spending 2024 [A]
- https://www.aerzteblatt.de/nachrichten/156146/IGeL-Umsatz-uebersteigt-laut-Erhebung-Zwei-Milliarden-Schwelle — IGeL €2.4bn [B]
- https://www.aok.de/pp/fileadmin/bereiche/nordwest/Presse/Dokumente/2025/2025-08-13_checkup35_sh_pm.pdf — check-up use 19.2 % [B]
- https://www.pkv.de/themen/krankenversicherung/betriebliche-krankenversicherung/ , https://www.allianz.de/presse/mitteilungen/starkes-bkv-wachstum-jeder-dritte-neukunde-waehlt-die-allianz/ , https://www.pkv.de/verband/presse/pressemitteilungen/private-krankenversicherung-auf-wachstumskurs-fast-jeder-zweite-deutsche-privatversichert/ — bKV and PKV figures [B]
- TED API (https://api.ted.europa.eu/v3/notices/search), notices 594202-2026 (WBM), 370897-2026 and 664823-2026 (IKK classic) [A]
- https://www.sport.mri.tum.de/images/files/downloads/tum-sportmedizin-betriebliche-gesundheitsfoerderung.pdf — TUM Manager-Check [B]
- https://www.munich-startup.de/en/news/wellabe-acquired-by-mavie-from-austria , https://www.axa-betreuer.de/site/ao-rel2020-AXA/get/documents_E578891519/axade/medien/geschaeftskunden/betriebliche-krankenversicherung/produktflyer-wellabe.pdf — wellabe [B]
- https://www.kliniken.de/krankenhaus/diagnostik-muenchen-4771K.html — Diagnostik München [B]
- https://medizinio.de/medizintechnik/mrt/mrt-geraet — MRI costs [B]
- https://itunes.apple.com/de/rss/customerreviews/page=1/id=1609437818/sortby=mostrecent/json , https://itunes.apple.com/search?term=wellabe&country=de&entity=software — app reviews and rating counts [C]
- https://hn.algolia.com/api/v1/items/40235129 — Hacker News thread on Neko [C]
- https://www.landkreis-pfaffenhofen.de/media/19808/stmgp_praeventionsfonds-foerdercall.pdf — Bavarian Präventionsfonds call [B]
