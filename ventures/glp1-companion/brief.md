# Venture brief: GLP-1 self-payer companion
Task: C11 | Date: 2026-11-14 | Status: draft (not yet reviewed by the critic) | Score: 37/55 base in the consumer-health scan (`research/consumer-health-scan.md`, adapted scale; not re-scored on the /90 scale)

**Bottom line for the CEO (researcher's view, you decide):**
- **The customer is real but small and leaves fast.** About **100,000** people in Germany paid for obesity drugs themselves at the end of 2024 (IQVIA [B]); no newer count was found. Drug costs are about €130 to just under €500 a month (Verbraucherzentrale, Mar 2026 [B]). Where patients pay themselves, fewer than 10 % are still on the drug after 12 months in some countries (review [A]).
- **The "companion" job is already done, often for free, by the companies that sell the drug.** GoLighter (Wellster, a Munich company) gives its drug customers free nutrition counselling and, since 1 Sep 2026, the Weight Watchers GLP-1 programme at no extra cost. It also sells side-effect "care packages" for €19.99–€32.99 [B]. Weight Watchers sells its GLP-1 programme on its own for €45 a month at list price, or €11.25 a month on a 12-month deal [B]. People with a BMI of 30–40 can get a reimbursed weight-loss app on prescription (Oviva Direkt, zanadio) [B]. The German App Store lists at least 25 GLP-1 tracker apps; most were launched in 2025–26 and have fewer than 60 ratings [C].
- **Muscle loss is a real problem but not a unique hook.** Lean mass is 25–39 % of the weight lost on these drugs. That is about the same as with diet alone (26 %), and strength training helps most (17.5 %) [A]. Protein products are a commodity: a branded 908 g whey tub costs €49.90 [B]. Supplements advertised with "GLP-1" are "in der Regel unzulässig" [B].
- **The arithmetic is hard** (section 5, my math). At €30 a month and a 6-month customer life, €1m revenue needs ~5,600 new paying customers a year. That is ~5.6 % of today's self-payers, every year. Marketing at the 39–46 % of revenue seen in filings [A] allows €70–83 to acquire each customer, and no desk source shows whether that is achievable.
- **One gap is visible.** GoLighter's free extras stop when the drug order stops ("Mit einem ärztlich verschriebenen Abnehmmedikament … kostenfrei"). People who quit, many because of cost, regain weight [A]. Nobody in DE was found serving them at scale; one small waitlist site plans a 12-week programme for under €129 [B].
- **Recommendation: do not go to Stage D.** Either run one €300, 2-week demand test on the "after the shot" (maintenance) angle, with the pass mark set in advance (section 13), or drop the consumer route. Of the two I recommend the test: acquisition cost is the one unknown that decides this, and only a test can measure it. If it fails, drop. Options are in task C12.

## 1. One-liner
People in Germany who pay €130–500 a month for a weight-loss drug, and especially those who stop because of cost or side effects, struggle to keep muscle, eat enough protein on little appetite and keep the weight off; we offer a low-cost, AI-supported nutrition and strength-training programme (optionally with a claims-compliant protein product), sold directly to them, so that they keep more muscle and regain less weight. **Unproven:** no source shows that such a programme reduces regain after stopping. Strength training and protein do preserve lean mass during weight loss (section 2).

Wedge chosen in this brief: **(b) "after the shot" maintenance** (people stopping or tapering the drug). Wedge (a), "companion during treatment", is described for comparison but not recommended: the drug platforms already bundle it free (section 6).

## 2. Problem evidence
**Hard data**
| What | Number | Source |
|---|---|---|
| Private (self-pay) users of anti-obesity drugs, DE | "almost 100,000 patients use AOMs privately" at the end of 2024 | [IQVIA blog, Dec 2024](https://www.iqvia.com/locations/emea/blogs/2024/12/doctors-and-obesity-are-healthcare-professionals-ready-for-the-new-anti-obesity-medications) [B] |
| Households using GLP-1 drugs (incl. diabetes, reimbursed) | "rund zwei Millionen deutsche Haushalte nutzen GLP-1-Medikamente aktiv", two million more interested (YouGov shopper panel 2025) | [Ernährungsindustrie (BVE), 12 Jun 2026](https://www.ernaehrungsindustrie.de/wie-die-glp-1-abnehmspritze-den-deutschen-lebensmittelmarkt-veraendert/) [B]; "über 4 Millionen Haushalte nutzen … oder ziehen ihre Nutzung in Betracht" ([YouGov, 15 Jan 2026](https://yougov.com/de-de/artikel/53896-yougov-daten-zeigen-abnehmspritze-verandert-den-deutschen-konsumalltag) [B]) |
| Statutory-insured people on GLP-1 drugs (mainly diabetes) | ~260,000 (2020) → 550,000 (2024) | [bifg/BARMER factsheet](https://www.bifg.de/media/dl/ePaper/factsheets/bifg-Factsheet-Abnehmspritzen.pdf) [B] (payer research institute) |
| Self-pay drug cost | €130 to "knapp 500 Euro" a month (Mar 2026); Mounjaro up to €490, Wegovy up to €276 (Jan 2026); Wegovy tablet ~€170 (1.5/4 mg) to ~€230 (9 mg) for 30 tablets (Sep 2026) | [Verbraucherzentrale FAQ](https://www.verbraucherzentrale.de/wissen/gesundheit-pflege/medikamente/abnehmspritzen-haeufige-fragen-und-antworten-zum-trend-118893) [B]; [ZDF, 18 Jan 2026](https://www.zdfheute.de/wirtschaft/unternehmen/abnehmspritze-preise-novo-nordisk-eli-lilly-geschaeft-ozempic-100.html) [B]; [zm-online, 1 Sep 2026](https://www.zm-online.de/news/detail/wegovy-ab-heute-auch-als-pille) [B] |
| Lean-mass loss | Lean mass = 35.2 % (semaglutide), 25.4 % (tirzepatide), 26.8 % (liraglutide) of weight lost; lifestyle alone 26.2 % (no significant difference); lifestyle + resistance training 17.5 %. 20 RCTs, n = 15,782 | [Diabetes Obes Metab 2026, PMID 41877354](https://pubmed.ncbi.nlm.nih.gov/41877354/) [A] |
| Nutrition guidance | Joint advisory of four US societies: protein 0.8 g/kg/d is the reference; "1.2–1.6 g/kg/d" proposed during weight reduction; "micronutrient or protein supplementation as needed" | [Am J Clin Nutr 2025, PMID 40450457](https://pubmed.ncbi.nlm.nih.gov/40450457/) (full text via Europe PMC PMC12612741) [A] |
| Persistence | ~75–80 % at 12 months in reimbursed diabetes cohorts (Sweden, Denmark) vs "below 10 % in obesity-focused or high out-of-pocket-cost settings (Poland, Colombia)"; drivers: GI intolerance and cost | [Nutrients 2026, PMID 42280404](https://pubmed.ncbi.nlm.nih.gov/42280404/) [A] (narrative review) |
| Why people stop | 31.7 % stopped within 180 days; of these 26.8 % adverse reaction, 14.4 % cost, 11.2 % non-adherence (US, n = 1,374) | [Diabetes Obes Metab 2026, PMID 41713959](https://pubmed.ncbi.nlm.nih.gov/41713959/) [A] |
| DE persistence (statutory, mainly diabetes) | ~16 % stop after the first use; a further 20 % / 33 % within 12 / 24 months | [bifg/BARMER factsheet](https://www.bifg.de/media/dl/ePaper/factsheets/bifg-Factsheet-Abnehmspritzen.pdf) [B] |
| What happens after stopping | "weight regain and the deterioration of multiple cardiometabolic risk factors are common" | [Nat Rev Endocrinol 2026, PMID 42168641](https://pubmed.ncbi.nlm.nih.gov/42168641/) [A] |
| Spend on adjacent products | Active GLP-1 users over-index on hair/skin/nail supplements, with higher average spend; people considering the drugs over-index on OTC digestive remedies (YouGov shopper panel 2025) | [YouGov, 12–13 Nov 2026](https://yougov.com/de-de/artikel/53834-der-hype-um-die-abnehmspritze-und-was-dahinter-steckt) [B] |

*Counter-evidence:* the "muscle loss" message is weaker than marketing suggests: lean-mass share on the drugs equals that on diet alone [A]. One German pharmacy source says neither supplements nor protein products alone prevent drug-related muscle loss; strength training does (pflueger.de, search result only, `[UNVERIFIED]`).

**Online voices [C]: 3 independent DE sources opened; Reddit not usable (search returns mirrors, not used per `lessons.md`); Mumsnet returned HTTP 403 this run**
- **Shotsy (GLP-1 tracker), German App Store review feed:** 150 reviews, Jun 2025 – Nov 2026. My keyword count: 14 say they use the free version, 3 say the subscription is not worth it, 4 say they gladly pay ([feed](https://itunes.apple.com/de/rss/customerreviews/page=1/id=6499510249/sortby=mostrecent/json)). Excerpts:
  - "Und für den Wirkstoffspiegel ist es mir nicht wert zu zahlen" (Oct 2026, 2★)
  - "viele Mounjaro-Nutzer in Deutschland „klicken“, nutzen also Teildosen eines höher dosierten Kwikpens, um Geld zu sparen" (Oct 2025, 5★). This is a cost workaround: people split higher-dose pens to save money.
  - "Dir zahlungspflichtige Version war noch besser … Leider ist mir diese etwas zu teuer." (typo "Dir" in the original) (Aug 2026, 5★)
- **Juniper app (telemedicine incumbent), German App Store:** 96 ratings, average 3.79. 25 written reviews (May–Nov 2026) are mostly about bugs ([feed](https://itunes.apple.com/de/rss/customerreviews/page=1/id=1661064221/sortby=mostrecent/json)). Excerpts:
  - "Die Behandlung selbst ist also nicht das Problem. Aber die App ist super schlecht." (Jul 2026, 2★)
  - "Der KI-Chat hat keinerlei Zugriff auf Verlaufsdaten" (Sep 2026, 1★)
- **glp-1forum.de (German self-help forum, founded by a patient):** "1.200+ Mitglieder". It offers a "Klick-Rechner" (dose in pen clicks), a side-effect barometer and an article on "Dosis splitten". The founder says he "plötzlich hatte ich hundert Fragen, aber keinen Ort, wo ich sie stellen konnte" ([home page](https://glp-1forum.de/)). Health threads are behind a login; not read.
- **Count of tracker apps:** German App Store search on 14 Nov 2026 ("GLP-1", "abnehmspritze", "mounjaro", "wegovy", "ozempic tracker") returns **≥25 GLP-1 tracker apps**. Most were released in 2025–26 and have fewer than 60 ratings. The leader, Shotsy, has 1,738 ([iTunes search API](https://itunes.apple.com/search?term=GLP-1&country=de&entity=software&limit=15)).
- *Inference:* voices show an information need and price sensitivity (free versions, pen splitting). They do not show willingness to pay for a companion beyond the drug.

**Why now**
- The **Wegovy tablet** has been on the German market since **1 Sep 2026**, at ~€170–230 a month; Germany was the first EU country to launch it ([zm-online](https://www.zm-online.de/news/detail/wegovy-ab-heute-auch-als-pille) [B]; [FoodNavigator, 6 Aug 2026](https://www.foodnavigator.com/Article/2026/08/06/germany-first-to-launch-wegovy-pill/) [B]). Early demand is "noch nicht so groß" ([dpa via leinetal24, 6 Oct 2026](https://www.leinetal24.de/wirtschaft/apotheken-bisher-wenig-nachfrage-nach-abnehmtablette-zr-94526410.html) [B]).
- **Reimbursement debate:** the new G-BA chair proposed in Aug 2026 that the legislator could ask the G-BA to define "welche Patientengruppen …, wie lange, mit welchen Begleitmaßnahmen" ([Apotheken Umschau, 3 Aug 2026](https://www.apotheken-umschau.de/news/koennte-die-abnehmspritze-auf-kassenkosten-kommen-g-ba-vorsitzende-zeigt-sich-offen-1566279.html) [B]). The AOK chief warned of ~€45bn a year if everyone with BMI ≥30 were treated ([Apotheken Umschau, 24 Aug 2026](https://www.apotheken-umschau.de/gesundheitspolitik/abnehmspritze-auf-rezept-welche-kosten-die-kassen-befuerchten-1576085.html) [B]). Today, § 34 Abs. 1 SGB V still excludes weight-regulating drugs; a court upheld this for Mounjaro ([apotheke adhoc, 7 Feb 2025](https://www.apotheke-adhoc.de/nachrichten/detail/politik/gericht-kasse-muss-mounjaro-nicht-bezahlen/) [B]).
- **Generics:** semaglutide protection in Europe runs to **19 Mar 2031**. Generics in India cost ~$15 a month ([apotheke adhoc, 26 May 2026](https://www.apotheke-adhoc.de/nachrichten/detail/internationales/semaglutid-generika-riesen-gehen-in-stellung/) [B]).
- *Inference:* more users and lower drug prices from 2027–2031 enlarge the companion market. Cheaper drugs may also mean fewer stop for cost reasons, which shrinks wedge (b).

## 3. Customer
- **User = buyer = payer:** the self-paying patient. No insurer pays for this companion. A reimbursed alternative exists only for BMI 30–40 (DiGA, section 6).
- **First segment (wedge b):** adults in Germany who stopped or are tapering a self-paid GLP-1 drug, plus those who are about to stop because of cost. Size: not counted anywhere. *Inference from the sources above:* with ~100,000 self-payers and persistence well under 50 % at 12 months, tens of thousands stop each year. This is unproven; no DE persistence data for self-payers exists.
- **Comparison segment (wedge a):** people currently on the drug. Most reach it through telemedicine platforms that bundle coaching (section 6), or through their own physician plus a pharmacy. How the self-payer pool splits between these two routes is unknown.
- **Decision process:** individual, online, impulse-to-considered; price anchor is the drug (€130–500/month) on one side and WW (€11.25–45/month) or free DiGA on the other.
- **Profile:** YouGov describes interested households as "eher jüngere Haushalte, bei denen das Thema Selbstoptimierung einen hohen Stellenwert hat" ([BVE](https://www.ernaehrungsindustrie.de/wie-die-glp-1-abnehmspritze-den-deutschen-lebensmittelmarkt-veraendert/) [B]). Juniper targets "particularly … women" ([Pulse 2.0, 6 Jun 2026](https://pulse2.com/hims-hers-completes-eucalyptus-acquisition-and-expands-weight-management-care-in-germany/) [B]).

## 4. Solution & product wedge
**Smallest product (wedge b, "Nach der Spritze"):** a 12-week digital programme for people who stop or taper:
1. A personal protein target and simple small-portion recipes.
2. Two 30-minute strength sessions a week, at home or in a gym, with progression.
3. A weekly check-in: weight, waist and strength.
4. An AI coach (chat) that answers food and training questions within set limits, with escalation to a human nutrition professional.
5. Optional, later: a private-label protein product that meets "source of protein" (≥12 % of energy from protein), so that the authorised muscle-mass claim can be used (section 8).

What AI/automation does: personalised plans and check-ins, coaching chat, automated nudges, and content generation reviewed by a nutrition professional. This is the CEO's skill set (`founder-brief.md`). *Inference.*

**What it is NOT (non-goals):**
- No dosing, dose-splitting or "click" calculators and no side-effect treatment advice. These would turn the app into medical-device software (MDCG 2019-11 rev.1, section 8).
- No drug sales, no prescriptions, no telemedicine.
- No "GLP-1" supplement and no claim to mimic the drug.
- No weight-loss promise.

**Wedge (a), during treatment, for comparison:** the same content sold to people on the drug. Not recommended: GoLighter, Juniper and Voy bundle coaching with the drug, and WW sells it for €11.25–45 (section 6).

## 5. Market size
**Price points found (sourced):**
| Offer | Price | Source |
|---|---|---|
| Weight Watchers "GLP-1 Begleitprogramm" (DE) | €45/month list; €31.50/month on 3 months; €11.25/month on a 12-month deal ("75 %" promo, "2026 Peak") | [weightwatchers.com/de/preise](https://www.weightwatchers.com/de/preise) (page data, accessed 2026-11-14) [B] |
| GoLighter care packages (side effects, OTC products) | €19.99 (2 products), €32.99 (4 products), shipping free | [golighter.de/p/care-pakete](https://www.golighter.de/p/care-pakete) [B] |
| "Nach der Spritze" 12-week programme (waitlist, not launched) | "soll unter 129 € kosten" | [nachderspritze.de](https://nachderspritze.de/wissen/muskelabbau-abnehmspritze/) [B] |
| Commodity whey protein (ESN Designer Whey) | €49.90 per 908 g | [esn.com product feed](https://www.esn.com/products.json) [B] |
| Drug + programme bundles | Voy from €173/month (up to €349; "Max" from €230); GoLighter "ab 99 Euro monatlich" (Sep 2025) | [myvoy.de](https://www.myvoy.de/) [B]; [apotheke adhoc branch news, 29 Sep 2025](https://www.apotheke-adhoc.de/branchennews/alle-branchennews/branchennews-detail/adipositas-therapie-mit-golighter/) [B] (vendor text) |

**Hypothesis for this brief:** €30 a month for the programme. That sits between WW's 3-month price (€31.50) and a whey tub, and is about €129 per 12 weeks. Average paid life **6 months** = **€180 per customer** (assumption; no persistence data for companion products).

**Bottom-up (my math; assumptions labelled):**
| | Customers | × €180 | Note |
|---|---|---|---|
| TAM today: all DE self-payers buy | 100,000 | **€18m/yr** | IQVIA end-2024 count [B]; the count is stale and growth since is not measured |
| TAM if the pool triples by 2028 | 300,000 | €54m/yr | *Assumption*, not sourced |
| Adjacent: statutory GLP-1 users (diabetes) | 550,000 (2024) | €99m/yr | [B]. They do not pay for the drug; whether they would pay for a companion is not shown |
| SAM wedge (b): people stopping each year | not counted | — | *Inference:* tens of thousands a year |
| **Three modest salaries** (€180,000 employer cost; assumption reused from the L01 brief) | 2,500 new customers/yr | €450,000 revenue | Needs 40 % of revenue left after 20 % COGS and 40 % marketing (assumptions) → 0.4 × 450,000 = 180,000 |
| **€1m revenue** | **~5,560 new customers/yr** | €1,000,000 | 1,000,000 / 180 = 5,556 |

- 5,556 is **~5.6 % of today's 100,000 self-payers, every year** (5,556 / 100,000). 2,500 is 2.5 %.
- **Allowed acquisition cost:** marketing is 39 % of revenue at Hims & Hers in 2025 ($919.3m of $2,347.6m; my math from [SEC XBRL filing data](https://data.sec.gov/api/xbrl/companyfacts/CIK0001773751.json) [A]), 46 % at Hims & Hers in 2024 and 44 % at PharmaSGP in 2019 (`research/consumer-health-scan.md`, `research/futrue-benchmark.md` [A]). At €180 revenue per customer that allows **€70–83 per paying customer** (0.39 × 180 = 70.2; 0.46 × 180 = 82.8). If customers stay 3 months instead of 6: €35–41.
- *Reading:* the TAM is small for a venture (€18m today in Germany). It becomes venture-sized only if (1) the self-pay pool grows several-fold (tablet, price cuts, generics 2031), (2) the product reaches DACH/EU, or (3) a payer route opens (section 7). None of these is in hand.

## 6. Competitors
| Company | URL | Offering | Pricing | Funding / size | Gap we exploit |
|---|---|---|---|---|---|
| GoLighter (Wellster Healthtech Group; audited 2024 accounts say "München", imprint now Monheim am Rhein) | golighter.de | Telemedicine route to the drug + free nutrition counselling (WhatsApp) + free WW GLP-1 programme since 1 Sep 2026 + paid care packages + zanadio DiGA referral | Free extras "Mit einem ärztlich verschriebenen Abnehmmedikament"; care packages €19.99–32.99 | Series B $60m (company newsroom); 2024 GmbH accounts: revenue **€9.94m, net loss €3.12m**, 51 FTE ([audited accounts via Bundestag lobby register](https://www.lobbyregister.bundestag.de/media/a1/95/704698/E_11037725_2024_18983_TA1_Testat-Wellster_dt.pdf) [A]); "EUR50 million in revenue" and "full profitability" in 2025 per press ([InforCapital, 23 Mar 2026](https://inforcapital.com/news/wellster-healthtech-expands-debt-facility-to-eur10-million-with-claret-capital-to-fund-international-expansion-1) [B]; not reconciled with the accounts, probably group vs GmbH or gross vs net) | Extras end when the drug order ends (*inference from the "mit … Abnehmmedikament" condition*) |
| Weight Watchers | weightwatchers.com/de | GLP-1 companion programme: protein targets, coaching, workshops, strength videos, dose and side-effect tracker | €11.25–45/month | Listed parent (WW International) | Strong brand; generic, not maintenance-specific (*inference*) |
| Juniper (Eucalyptus; Hims & Hers since Jun 2026) | myjuniper.com/de | Drug + coaching programme, since Mar 2023 | €172 first month, then €299 per 28 days (search snippet only, `[UNVERIFIED]`; site 403) | Acquisition up to $1.15bn ([Pulse 2.0](https://pulse2.com/hims-hers-completes-eucalyptus-acquisition-and-expands-weight-management-care-in-germany/) [B]) | App rated 3.79 with bug complaints [C] |
| Voy (Menwell Ltd) | myvoy.de | Drug + programme with nutrition and behaviour experts | From €173/month | n/a | Same as above |
| Oviva Direkt, zanadio (DiGA) | oviva.com, zanadio.de | Reimbursed digital lifestyle therapy, BMI 30–40; zanadio class IIa, prescribed "mehr als 50.000-mal" | Free for statutory patients on prescription | Oviva: ">800.000 behandelten Patienten in Europa" (2024) ([PTAheute, 4 Mar 2026](https://www.ptaheute.de/aktuelles/2026/03/04/diga-bei-adipositas-lebensstilintervention-mit-evidenz) [B]) | Not for BMI <30, i.e. many people after successful weight loss (*inference*) |
| GLP-1 tracker apps (Shotsy and ≥24 others) | App Store | Dose, weight, side-effect tracking | Freemium | Small; Shotsy 1,738 DE ratings | Crowded, low willingness to pay [C] |
| Gerresheimer | gerresheimer.com | White-label GLP-1 support app for pharma companies (in development) | B2B | Listed company | Shows the B2B route is taken by a supplier with pharma access |
| Nach der Spritze | nachderspritze.de | 12-week maintenance programme, waitlist | "unter 129 €" planned | Unknown; one-site project | Closest to wedge (b); proves the idea is visible, not that it sells |
| Nupo (Danish diet foods) | nupo.de | GLP-1 guide content; diet products | e.g. 10 bars €29.99 | n/a | Content marketing aimed at GLP-1 users, no GLP-1 product found in its feed |
| Big food (US only so far) | — | Nestlé Vital Pursuit (US, 2024), Herbalife "GLP-1 Nutrition Companion" (US/Puerto Rico, Feb 2024) | — | — | Not launched in DE as far as found ([BVE](https://www.ernaehrungsindustrie.de/wie-die-glp-1-abnehmspritze-den-deutschen-lebensmittelmarkt-veraendert/) [B]: "Gezielt auf GLP-1-Nutzer ausgerichtete Produkte sind hierzulande bislang kaum zu finden"; Herbalife US launch per [Herbalife IR](https://ir.herbalife.com/news-events/press-releases/detail/879/herbalife-launches-glp-1-nutrition-companion-product-combos), search result only) |

Also: Arla reports demand for protein dairy; Arla says users do not want to be singled out: "Nutzer möchten keine Sonderrolle einnehmen" ([t-online/dpa, 6 Oct 2026](https://www.t-online.de/finanzen/aktuelles/id_101467624/abnehmspritze-wird-in-deutschland-bald-weniger-gegessen-.html) [B]). Nestlé US found only "rund 20 Prozent der Käufer" of Vital Pursuit use the drugs ([BVE](https://www.ernaehrungsindustrie.de/wie-die-glp-1-abnehmspritze-den-deutschen-lebensmittelmarkt-veraendert/) [B], citing Handelsblatt). *Inference:* a "GLP-1 food" label may matter less than the protein benefit itself, so a protein product competes with every protein brand.

## 7. Business model & pricing
- **Model:** direct-to-consumer subscription, €30/month or ~€129 per 12 weeks (hypothesis, benchmarks in section 5). Optional later: a private-label protein product. Contract makers start from 2,000 units with 8–12 weeks lead time (`research/consumer-health-scan.md` [B]); unit price not published `[UNVERIFIED]`.
- **What drives repeat purchases:** the programme length (12 weeks), visible progress (strength, waist), and possibly a restart when a person goes back on the drug. *Inference*; no repeat-rate data for this category.
- **Alternative B2B models (not chosen, noted for the CEO):**
  - (i) White-label programme for telemedicine platforms or online pharmacies. There are few buyers, the big ones build in-house or partner with WW, and Gerresheimer offers white-label software to pharma.
  - (ii) A reimbursed programme, if the legislator changes § 34 SGB V and the G-BA requires "Begleitmaßnahmen". This is not law. The adult obesity DMP exists on paper: the G-BA commissioned an IQWiG guideline update on 8 Jul 2026, and the commission asks the IQWiG to show "Empfehlungen zu digitalen medizinischen Anwendungen" ([G-BA decision PDF](https://www.g-ba.de/downloads/39-261-7917/2026-07-08_IQWIG-Beauftragung_Leitliniensynopse-DMP-Adipositas-Erwachsene.pdf) [A]). The obesity society says DMP implementation "hapere" ([PZ, 10 Aug 2026](https://www.pharmazeutische-zeitung.de/erstattungsdebatte-geht-in-die-naechste-runde-167471/) [B]). A reimbursed route would likely mean a DiGA (medical device, years), not this product.

## 8. Regulation & data
| Area | Rule | What it means here | Source |
|---|---|---|---|
| The drug | Rx-only; § 34 Abs. 1 SGB V excludes weight-regulating drugs from statutory cover | Customers pay themselves; a reform would change the customer base (risk and opportunity) | [apotheke adhoc, LSG BW case](https://www.apotheke-adhoc.de/nachrichten/detail/politik/gericht-kasse-muss-mounjaro-nicht-bezahlen/) [B] |
| Advertising the drug | Public advertising of Rx drugs is banned (§ 10 HWG). LG München I (4 HK O 15458/24, 3 Mar 2025, interim relief): an online pharmacy may not advertise questionnaire-only obesity treatment to consumers; "vor der Verschreibung einer Abnehmspritze [ist] ein persönlicher ärztlicher Kontakt … erforderlich" | Never mention or promote the drug in ads. Whether naming the target group ("für Menschen, die die Abnehmspritze absetzen") is allowed for a food or a coaching service is **not settled** `[UNVERIFIED]`: one paid hour with a lawyer (proposed outward action) | [LG München I press release](https://www.justiz.bayern.de/gerichte-und-behoerden/landgericht/muenchen-1/presse/2025/3.php) [A]; [Verbraucherzentrale](https://www.verbraucherzentrale.de/faq/glp1werbung-fuer-nahrungsergaenzungsmittel-108473) [B]. Appeal OLG München 29 U 1035/25 (search result only, outcome unknown, `[UNVERIFIED]`) |
| "GLP-1" supplements | "gibt es keine Wirknachweise. Die Werbung ist in der Regel unzulässig, da krankheitsbezogen" | No GLP-1 wording, no "natural Ozempic" | [Verbraucherzentrale](https://www.verbraucherzentrale.de/faq/glp1werbung-fuer-nahrungsergaenzungsmittel-108473) [B] |
| Protein claims | "Source of protein": ≥12 % of energy from protein; "high protein": ≥20 %. Authorised health claims exist for "source of protein" foods, e.g. growth and maintenance of muscle mass | A protein product can carry the muscle-mass claim if it meets the threshold. Exact claim wording in Reg. (EU) 432/2012 was not re-read (EUR-Lex bot-checked this run) | [EC Knowledge4Policy, dietary protein](https://knowledge4policy.ec.europa.eu/dietary-protein_en) [A] |
| Supplements generally | BVL notification (§ 5 NemV); disease claims banned for all foods (Art. 7(3) LMIV) | Notification, not approval; claims are the constraint | `research/consumer-health-scan.md` [A]/[B] |
| App: medical device? | Software that analyses patient-specific data "to suggest dosage adjustments" is medical-device software | Leave out dose calculators, "click" converters and side-effect management. A food, exercise and habit programme without a medical purpose is *probably* not a medical device (*inference*; a claim to treat obesity or prevent regain as a disease outcome could change that) | [MDCG 2019-11 rev.1, Jun 2025](https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=mdcg_2019_11_guidance_qualification_classification_software_en.pdf) [A] |
| Health data | Weight and health data are special-category data under Art. 9 GDPR; explicit consent, DE/EU hosting | Standard for a health app; budget for a data-protection review | Not re-opened this run (`[UNVERIFIED]` for details) |
| Platform ad rules | Meta and Google restrict weight-loss and prescription-drug ads | Shapes the demand test (section 13) | Third-party summaries only, `[UNVERIFIED]` |

Time and cost to market (*inference*): a non-device digital programme can go live in 2–3 months with no approval. A protein product needs a contract maker (MOQ ~2,000 units), a label check and a BVL notification if it is a supplement. Legal review: one to a few lawyer hours. Prices not sourced.

## 9. Go-to-market
- **First 10 customers (wedge b):** people who announce they are stopping, reached via paid social and search on maintenance and "after the injection" topics. Claims-compliant wording only. Self-help forums and Facebook groups could be used only with the admins' consent, as an outward action needing CEO approval.
- **Partners (later, outward action):** platforms that lose the customer when the drug stops (GoLighter, Juniper, Voy) could refer leavers to a maintenance programme. *Inference:* they may prefer to keep the customer on the drug or build this themselves; WW already partners with GoLighter.
- **Pilot design:** 12-week paid cohort of 30–50 people. Measure completion, strength gain, weight change and willingness to continue at full price. No health claim from pilot results without proper evidence.

## 10. Funding path
- **Own money:** €10,000 (`founder-brief.md`). This covers a demand test, a landing page, a lawyer hour and a small paid pilot cohort (*inference*). It does not cover a protein product run plus marketing.
- **Grants** (details and deadlines in `research/munich-ecosystem.md`):
  - EXIST needs leaving the job or a sabbatical plus a Hochschule host; a pure consumer brand may not count as "innovativ, technologieorientiert" (*inference*). The current guideline takes applications to 31 Dec 2027.
  - Start?Zuschuss! pays 50 %, max €36,000, for digital startups up to 2 years old; round 23 is planned for 25 Nov 2026 – 10 Jan 2027 (needs a company).
  - BayDiGuP funds digital health projects through calls.
  - EIC Accelerator does not fit at this stage (TRL 6–8).
- **Investors:** Calm/Storm (Vienna; B2C and B2B healthtech pre-seed), HTGF and Bayern Kapital (`research/munich-ecosystem.md`). Wellster's backers include Mangrove Capital, with venture debt from Claret Capital ([InforCapital](https://inforcapital.com/news/wellster-healthtech-expands-debt-facility-to-eur10-million-with-claret-capital-to-fund-international-expansion-1) [B]).
- **Capital to first revenue:** small; paid cohorts can start within weeks (*inference*). **Capital to €1m revenue:** ~€400–460k of marketing a year at 39–46 % (my math: 0.39–0.46 × €1m), which must come from investors.

## 11. Team
- **CEO (you):** product, AI/automation, operations; German-speaking market. Fits the digital programme well.
- **Co-founder 1 (needed): nutrition/medical lead.** A nutrition scientist (M.Sc.) or a physician in nutritional medicine who owns the programme content, safety limits and claims. Where in Munich: the TUM nutrition-medicine environment (TUM's Prof. Hauner is quoted on GLP-1 online prescribing in [apotheke adhoc, 2 Oct 2025](https://www.apotheke-adhoc.de/nachrichten/detail/panorama/abnehmspritze-problemlos-rezepte-fuer-normalgewichtige/) [B]) and the TUM Venture Lab Healthcare networks (`research/munich-ecosystem.md`). An exercise scientist (strength training) is a second-best profile.
- **Co-founder 2 or early hire: performance marketer.** Acquisition cost decides the case (section 5). Munich has DTC health operators (Wellster itself) whose alumni have this skill (*inference*).
- 10-minute check for you: do you know a nutrition scientist, a physician in nutritional medicine, or a performance marketer you could call?

## 12. Risks & kill criteria (researcher's pre-mortem; the critic's pre-mortem is still to come)
| Riskiest assumption | Evidence so far | How to test | Kill if |
|---|---|---|---|
| R1 People who stop the drug will pay for a maintenance programme | Regain after stopping [A]; cost is a reason to stop [A]; one waitlist site [B]; no sale observed | €300 demand test (section 13); 8 interviews | Cost per sign-up with price shown **> €15 on both themes** after 2 weeks / €300 |
| R2 Acquisition cost ≤ €70–83 per paying customer | Benchmarks only (39–46 % marketing [A]); no category CAC | Demand test + 30-person paid cohort | Paid conversion from waitlist < 5 % in the first cohort |
| R3 Incumbents leave the "after the shot" gap open | GoLighter extras tied to a drug order [B]; WW open to anyone at €11.25–45 [B] | Re-check GoLighter, Juniper, Voy and WW offers on the test date | ≥2 of GoLighter / Juniper / Voy offer a free maintenance programme to leavers by the test date |
| R4 Ads can name the target group legally | LG München I ruling on drug ads [A]; no ruling on food/coaching ads found | One lawyer hour (outward action, CEO approval) | Lawyer says no compliant wording can reach the target group, and the neutral wording fails the test |
| R5 The self-pay pool keeps growing | 100k end-2024 [B]; tablet launched [B]; generics 2031 [B] | Watch IQVIA/press for a 2026 count; § 34 SGB V debate | A § 34 SGB V change passes the Bundestag before Sep 2027: re-assess (customer becomes an insurer's patient; not an automatic kill) |
| R6 Price drops make fewer people stop | Generics only in 2031 in EU [B]; no DE price cut found | Watch list prices | — (would shrink wedge b, enlarge wedge a) |
| R7 Founder can build a team | No named candidate | 10-minute check (section 11) | No nutrition/medical co-founder candidate named by **31 Mar 2027** |

## 13. Validation plan
**Demand test (for CEO approval later; nothing goes live without it):**
- **Budget and duration:** €300 ad spend, 2 weeks, one platform (Meta or Google; check its current health-ad rules first, `[UNVERIFIED]`), plus a free landing-page tool.
- **Two themes, €150 each:**
  - A, maintenance: "Gewicht halten nach dem Abnehmen: 12 Wochen Kraft und Eiweiß".
  - B, low appetite: "Genug Eiweiß, wenn der Appetit fehlt".
- **Claims rules:**
  - No drug names, no "GLP-1", no "Abnehmspritze" unless the lawyer hour clears it.
  - No weight-loss promise, no disease claim, no before/after images.
  - Show the price (€129 per 12 weeks) on the page; the sign-up is a waitlist with an e-mail address.
- **Pass mark (set in advance, my math):** the allowed CAC is €70–83 per paying customer (section 5). If 10 % of price-aware waitlist sign-ups later pay (*assumption*), the cost per sign-up must be ≤ ~€7. Rule: **pass** if a theme gets ≥40 sign-ups for €300 (≤ €7.50 each); **kill** if both themes cost > €15 per sign-up; anything between is "inconclusive", and the default is stop.
- **Data:** GDPR-compliant form; e-mails deleted after the test unless people opt in.

**5–10 interviews (Mom Test, after the test or instead of it; outward action):**
- **Who:** 4 people who stopped a self-paid GLP-1 drug in the last 12 months; 3 current self-payers; 1 pharmacist who dispenses many private prescriptions; 1 nutrition professional who coaches GLP-1 patients; 1 platform manager (GoLighter, Juniper or Voy).
- **Questions:**
  - "Why did you stop? What happened in the 3 months after?"
  - "What have you spent money on besides the drug (food, supplements, apps, coaching, gym)? How much a month?"
  - "What did you try to keep the weight off? What did it cost?"
  - Platform: "What do you offer people who stop the drug? Why?"
- **Confirms:** ≥3 of 7 patients have already paid for a companion product or service outside the drug, and ≥2 stoppers describe regain as their main worry.
- **Kills:** <3 of 7 report any companion spend, or the platform already runs a leaver programme.

## Sources
- https://www.iqvia.com/locations/emea/blogs/2024/12/doctors-and-obesity-are-healthcare-professionals-ready-for-the-new-anti-obesity-medications — ~100,000 private AOM users in DE end-2024, accessed 2026-11-14 [B]
- https://www.ernaehrungsindustrie.de/wie-die-glp-1-abnehmspritze-den-deutschen-lebensmittelmarkt-veraendert/ — YouGov ~2m active-user households, profile, no GLP-1 products in DE, Nestlé 20 %, accessed 2026-11-14 [B]
- https://yougov.com/de-de/artikel/53896-yougov-daten-zeigen-abnehmspritze-verandert-den-deutschen-konsumalltag — >4m households use or consider (15 Jan 2026), accessed 2026-11-14 [B]
- https://yougov.com/de-de/artikel/53834-der-hype-um-die-abnehmspritze-und-was-dahinter-steckt — users over-index on hair/skin/nail supplements, accessed 2026-11-14 [B]
- https://www.bifg.de/media/dl/ePaper/factsheets/bifg-Factsheet-Abnehmspritzen.pdf — GKV GLP-1 users 260k→550k, persistence, accessed 2026-11-14 [B]
- https://www.verbraucherzentrale.de/wissen/gesundheit-pflege/medikamente/abnehmspritzen-haeufige-fragen-und-antworten-zum-trend-118893 — monthly cost €130–<500 (Mar 2026), platform test purchases, accessed 2026-11-14 [B]
- https://www.zdfheute.de/wirtschaft/unternehmen/abnehmspritze-preise-novo-nordisk-eli-lilly-geschaeft-ozempic-100.html — Mounjaro up to €490, Wegovy up to €276 (18 Jan 2026), accessed 2026-11-14 [B]
- https://www.zm-online.de/news/detail/wegovy-ab-heute-auch-als-pille — Wegovy tablet launch 1 Sep 2026, prices, accessed 2026-11-14 [B]
- https://www.foodnavigator.com/Article/2026/08/06/germany-first-to-launch-wegovy-pill/ — Germany first EU launch, accessed 2026-11-14 [B]
- https://www.leinetal24.de/wirtschaft/apotheken-bisher-wenig-nachfrage-nach-abnehmtablette-zr-94526410.html — weak early tablet demand (dpa, 6 Oct 2026), accessed 2026-11-14 [B]
- https://pubmed.ncbi.nlm.nih.gov/41877354/ — lean-mass meta-analysis (abstract via NCBI E-utilities), accessed 2026-11-14 [A]
- https://pubmed.ncbi.nlm.nih.gov/40450457/ — joint nutrition advisory; full text Europe PMC PMC12612741, accessed 2026-11-14 [A]
- https://pubmed.ncbi.nlm.nih.gov/42280404/ — persistence review (abstract), accessed 2026-11-14 [A]
- https://pubmed.ncbi.nlm.nih.gov/41713959/ — discontinuation reasons (abstract), accessed 2026-11-14 [A]
- https://pubmed.ncbi.nlm.nih.gov/42168641/ — consequences of discontinuation (abstract), accessed 2026-11-14 [A]
- https://www.apotheken-umschau.de/news/koennte-die-abnehmspritze-auf-kassenkosten-kommen-g-ba-vorsitzende-zeigt-sich-offen-1566279.html — G-BA chair proposal (3 Aug 2026), accessed 2026-11-14 [B]
- https://www.apotheken-umschau.de/gesundheitspolitik/abnehmspritze-auf-rezept-welche-kosten-die-kassen-befuerchten-1576085.html — AOK €45bn scenario (24 Aug 2026), accessed 2026-11-14 [B]
- https://www.pharmazeutische-zeitung.de/erstattungsdebatte-geht-in-die-naechste-runde-167471/ — DAG position, DMP implementation lagging (10 Aug 2026), accessed 2026-11-14 [B]
- https://www.g-ba.de/downloads/39-261-7917/2026-07-08_IQWIG-Beauftragung_Leitliniensynopse-DMP-Adipositas-Erwachsene.pdf — DMP obesity adults guideline update commission, accessed 2026-11-14 [A]
- https://www.apotheke-adhoc.de/nachrichten/detail/politik/gericht-kasse-muss-mounjaro-nicht-bezahlen/ — § 34 SGB V exclusion upheld (7 Feb 2025), accessed 2026-11-14 [B]
- https://www.apotheke-adhoc.de/nachrichten/detail/internationales/semaglutid-generika-riesen-gehen-in-stellung/ — EU protection to 19 Mar 2031, India ~$15/month (26 May 2026), accessed 2026-11-14 [B]
- https://www.apotheke-adhoc.de/nachrichten/detail/panorama/abnehmspritze-problemlos-rezepte-fuer-normalgewichtige/ — SWR test of online portals, TUM expert quote (2 Oct 2025), accessed 2026-11-14 [B]
- https://www.justiz.bayern.de/gerichte-und-behoerden/landgericht/muenchen-1/presse/2025/3.php — LG München I 4 HK O 15458/24 press release, accessed 2026-11-14 [A]
- https://www.verbraucherzentrale.de/faq/glp1werbung-fuer-nahrungsergaenzungsmittel-108473 — GLP-1 supplement ads usually unlawful; § 10 HWG, accessed 2026-11-14 [B]
- https://knowledge4policy.ec.europa.eu/dietary-protein_en — protein nutrition claim thresholds and authorised claim types, accessed 2026-11-14 [A]
- https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=mdcg_2019_11_guidance_qualification_classification_software_en.pdf — MDCG 2019-11 rev.1 (Jun 2025), dosage software = MDSW, accessed 2026-11-14 [A]
- https://www.golighter.de/ , https://www.golighter.de/p/care-pakete , https://www.golighter.de/p/ernaehrungsberatung , https://www.golighter.de/p/abnehm-app , https://www.golighter.de/fakten-unternehmen — GoLighter offer, free extras tied to drug, care package prices, zanadio, entity facts, accessed 2026-11-14 [B]
- https://www.apotheke-adhoc.de/branchennews/alle-branchennews/branchennews-detail/golighter-und-weight-watchers-begleitung-fuer-glp-1-patienten/ — GoLighter × WW from 1 Sep 2026 (vendor release), accessed 2026-11-14 [B]
- https://www.apotheke-adhoc.de/branchennews/alle-branchennews/branchennews-detail/adipositas-therapie-mit-golighter/ — "ab 99 Euro monatlich" (vendor text, 29 Sep 2025), accessed 2026-11-14 [B]
- https://www.apotheke-adhoc.de/branchennews/alle-branchennews/branchennews-detail/studie-zeigt-hohe-alltagstauglichkeit-digitaler-behandlungen/ — Wellster real-world survey claims (vendor text, 16 Oct 2025), accessed 2026-11-14 [B]
- https://www.lobbyregister.bundestag.de/media/a1/95/704698/E_11037725_2024_18983_TA1_Testat-Wellster_dt.pdf — Wellster 2024 audited accounts (revenue €9.94m, loss €3.12m, 51 FTE, advertising up), accessed 2026-11-14 [A]
- https://www.wellsterhealth.com/impressum , https://www.wellsterhealth.com/newsroom — imprint (Monheim), newsroom headlines (Series B $60m; "aus München erstmals profitabel"), accessed 2026-11-14 [B]
- https://inforcapital.com/news/wellster-healthtech-expands-debt-facility-to-eur10-million-with-claret-capital-to-fund-international-expansion-1 — 2025 "EUR50 million in revenue", profitability, debt facility (23 Mar 2026), accessed 2026-11-14 [B]
- https://www.weightwatchers.com/de/preise , https://www.weightwatchers.com/de/so-funktionierts/glp-1-programm — WW GLP-1 programme content and prices, accessed 2026-11-14 [B]
- https://www.myvoy.de/ — Voy programme prices, accessed 2026-11-14 [B]
- https://pulse2.com/hims-hers-completes-eucalyptus-acquisition-and-expands-weight-management-care-in-germany/ — Hims & Hers completes Eucalyptus/Juniper acquisition (6 Jun 2026), accessed 2026-11-14 [B]
- https://data.sec.gov/api/xbrl/companyfacts/CIK0001773751.json — Hims & Hers FY2025 revenue $2,347.6m, marketing $919.3m (10-K XBRL), accessed 2026-11-14 [A]
- https://www.ptaheute.de/aktuelles/2026/03/04/diga-bei-adipositas-lebensstilintervention-mit-evidenz — obesity DiGAs, BMI 30–40, zanadio >50,000 prescriptions, Oviva >800,000 patients (4 Mar 2026), accessed 2026-11-14 [B]
- https://www.gerresheimer.com/en/customer/products-solutions/pharma/digital-solutions/digital-therapeutics/glp-1-support-app — white-label GLP-1 support app for pharma, accessed 2026-11-14 [B]
- https://nachderspritze.de/wissen/muskelabbau-abnehmspritze/ — 12-week maintenance programme waitlist "unter 129 €", accessed 2026-11-14 [B]
- https://nupo.de/blogs/glp-1-ratgeber/muskelabbau-abnehmspritze-protein , https://nupo.de/products.json — Nupo GLP-1 content, product prices, accessed 2026-11-14 [B]
- https://www.esn.com/products.json — whey protein price €49.90/908 g, accessed 2026-11-14 [B]
- https://www.t-online.de/finanzen/aktuelles/id_101467624/abnehmspritze-wird-in-deutschland-bald-weniger-gegessen-.html — Arla quote, YouGov food-spend effects (dpa, 6 Oct 2026), accessed 2026-11-14 [B]
- https://itunes.apple.com/de/rss/customerreviews/page=1/id=6499510249/sortby=mostrecent/json (pages 1–3) — Shotsy DE reviews, accessed 2026-11-14 [C]
- https://itunes.apple.com/de/rss/customerreviews/page=1/id=1661064221/sortby=mostrecent/json — Juniper DE reviews, accessed 2026-11-14 [C]
- https://itunes.apple.com/search?term=GLP-1&country=de&entity=software&limit=15 (and terms abnehmspritze, mounjaro, wegovy, ozempic+tracker, juniper, oviva, zanadio) — app counts and ratings, accessed 2026-11-14 [C]
- https://glp-1forum.de/ , https://glp-1forum.de/forum/ — German self-help forum, members, tools, accessed 2026-11-14 [C]
- `research/consumer-health-scan.md`, `research/futrue-benchmark.md`, `research/munich-ecosystem.md` — repo files (fact-checked) for NemV/LMIV, PharmaSGP marketing share, contract-maker MOQ, grants and investors

## Gaps / [UNVERIFIED]
- No 2025/2026 count of German self-payers; the 100,000 figure is IQVIA end-2024 and >1 year old. YouGov household figures include reimbursed diabetes use and are self-reported. They do not reconcile with the claims data (550,000 statutory users plus ~100,000 private users = ~650,000 people, vs ~2m households).
- No persistence data for German self-payers; no repeat or churn data for any companion product.
- No category acquisition cost; the €70–83 allowance is derived from company-wide marketing shares.
- Wellster: press "EUR50 million" for 2025 vs audited GmbH revenue €9.94m for 2024 not reconciled (different entity or gross vs net is likely, not confirmed).
- Juniper DE prices (search snippet, site 403); Herbalife and Nestlé US launches (search results, not opened); Meta/Google ad rules; OLG München appeal; exact Reg. 432/2012 claim wording (EUR-Lex bot check); hair-loss frequency on tirzepatide (Lilly page 403).
- Legal question for a lawyer: may a food or coaching service name "Abnehmspritze" users as its target group in ads?
