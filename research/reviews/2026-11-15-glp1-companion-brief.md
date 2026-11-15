# Fact-check: ventures/glp1-companion/brief.md
Date 2026-11-15 | Verdict: **needs work (minor facts, one arithmetic fault in the demand test)** | Sources checked: 55 of 56 cited URLs opened (all of them, not a sample; MDCG PDF returned HTTP 503 twice) + 5 PubMed abstracts via NCBI E-utilities + Europe PMC full text PMC12612741 + SEC XBRL re-computed + App Store recipes re-run

Task C13, fact-check half. The red-team half (payer, founder fit, incumbents, pre-mortem, kill criteria) is a separate run: `research/reviews/<date>-redteam-glp1-companion-brief.md`.

**Summary for the CEO:** the facts hold. Every number the bottom line rests on matches its source: about 100,000 self-payers at end-2024 (IQVIA), €130 to just under €500 a month (Verbraucherzentrale), "below 10 %" persistence in high out-of-pocket settings (Nutrients review), lean mass 25–39 % of weight lost vs 26 % on diet (meta-analysis), GoLighter's free WW programme since 1 Sep 2026, Wellster's audited 2024 revenue of €9.94m and loss of €3.12m, Hims & Hers marketing at 39 % (2025) and 46 % (2024). No invented quotes; all App Store quotes found verbatim. What is wrong is the **demand-test arithmetic** in sections 5 and 13. The page would show a price 55 % higher than the price used to compute the pass mark. Each theme gets €150 but must reach 40 sign-ups "for €300". The cohort kill line (5 % paid conversion) is looser than the 10 % the pass mark assumes. These faults do not change the recommendation (b) "test before Stage D". They do change the numbers the CEO would approve for that test, so fix them before C12 is answered with (b).

## Critical issues (must fix)
1. **Price used for revenue ≠ price shown in the test (sections 5, 7, 13).** Section 5 says "€30 a month … and is about €129 per 12 weeks". 12 weeks ≈ 2.8 months, so €30/month ≈ **€83 per 12 weeks**, and €129 per 12 weeks ≈ **€47/month** (above WW's €45 list price). The CAC allowance (€70–83) and the pass mark use €180 per customer (6 × €30). The landing page in section 13 shows "€129 per 12 weeks". At that price a 6-month customer pays ~€279, and the allowance would be €109–128. Fix: pick one price, and use the same price in the revenue table, the CAC allowance, the pass mark and the landing page.
2. **Pass mark does not match the budget split (section 13).** "Two themes, €150 each" but "pass if a theme gets ≥40 sign-ups for €300 (≤ €7.50 each)". One theme only has €150. At €7.50 that is ≥20 sign-ups per theme. As written, 40 sign-ups for €150 is a €3.75 bar, twice as strict as the derivation. Fix the wording to "≥20 sign-ups per €150 theme (≤ €7.50 each)" or re-derive.
3. **Kill line in R2 is looser than the economics (section 12 vs 13).** The pass mark assumes 10 % of waitlist sign-ups pay. R2 kills only if paid conversion is < 5 %. At €7.50 per sign-up and 5–10 % conversion, CAC is €75–150, mostly above the €70–83 allowance. So a cohort can "survive" R2 with unaffordable acquisition. Fix: set the R2 kill at the conversion implied by the allowance and the observed cost per sign-up (CAC = cost per sign-up ÷ conversion ≤ allowance), or state the gap.

(Items 1–3 are one fix: re-derive section 13 from one price. One fix task added: C14.)

## Other issues (minor)
4. **YouGov date wrong.** Row "Spend on adjacent products" cites "[YouGov, 12–13 Nov 2026]". The article is dated **13 Jan 2026** ("Lenneke Schils - 13. Januar 2026"). Content (hair/skin/nail supplements for users; OTC digestive remedies for considerers, higher average spend) is supported.
5. **Altered text inside quotation marks.** Section 2 quotes YouGov as "über 4 Millionen Haushalte nutzen … oder ziehen ihre Nutzung in Betracht". The source says "**Bereits mehr als vier Millionen Haushalte nutzen in Deutschland GLP-1-Medikamente oder ziehen ihre Nutzung in Betracht**". The meaning is the same, but a quote must be verbatim (rule 3).
6. **Juniper "Acquisition up to $1.15bn" not in the cited source.** Pulse 2.0 (6 Jun 2026) confirms the completed Hims & Hers acquisition of Eucalyptus/Juniper, launch in DE in Mar 2023 and the "particularly … women" focus, but gives **no deal value**. Mark `[UNVERIFIED]` or cite a source that states it. Not used in any calculation.
7. **zanadio "class IIa" cited to PTAheute, which does not say so.** The class is on the GoLighter zanadio page ("Medizinprodukt der Klasse 2a"), which is in the source list. Re-attribute. PTAheute supports BMI 30–40, ">50.000-mal verordnet" and Oviva ">800.000 behandelten Patienten in Europa" (2024).
8. **Gerresheimer "(in development)" not on the page.** The page describes a GLP-1 support app that gives pharma companies real-world data. Neither "white-label" nor "in development" appears in the extracted text. Soften to what the page says, or tag.
9. **Voy "from €173/month" is a promotion.** myvoy.de shows "Ab 248 € 173 € pro Monat", i.e. €100 off the first 2 months, and its FAQ says "ab 173 €" rising to max €349; "Max" from €230. Say "€248 list, €173 promo".
10. **Herbalife can be upgraded from "search result only".** The Herbalife IR release (8 Feb 2024) opens and confirms "GLP-1 Nutrition Companion … launched first in the United States and Puerto Rico". Nestlé Vital Pursuit stays as cited via BVE/Handelsblatt (the BVE page supports "rund 20 Prozent der Käufer").
11. **Free substitute for wedge (b) not listed.** glp-1forum.de (1,200+ members, free) carries an "Absetzen" section and an article "Was passiert nach dem Absetzen von GLP-1 Medikamenten?". The brief cites the forum as a voice, not as a free alternative for leavers. Add it to section 6, or say it was considered. (This is a factual omission; whether it matters is for the red team.)
12. **BayDiGuP (section 10).** "Funds digital health projects through calls" is correct, but `research/munich-ecosystem.md` also says "no 2026 call found". Carry that over so it is not read as an open route.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| "almost 100,000 patients use AOMs privately" DE end-2024 | IQVIA blog Dec 2024 | supported | Exact wording. Stale (>1 yr) and flagged as such in the brief |
| ~2m households use GLP-1, 2m more interested; profile "eher jüngere Haushalte … Selbstoptimierung" | BVE 12.06.2026 | supported | |
| ">4m households use or consider" | YouGov 15 Jan 2026 | supported, quote altered | Issue 5 |
| GKV GLP-1 users 260k (2020) → 550k (2024); 16 % stop after first use, +20 % / 33 % within 12 / 24 months | bifg factsheet | supported | |
| €130 to "knapp 500 Euro"/month (Stand März 2026) | Verbraucherzentrale FAQ | supported | |
| Mounjaro up to €490, Wegovy up to €276 | ZDF 18.01.2026 | supported | |
| Wegovy tablet ~€170 (1.5/4 mg), ~€230 (9 mg); launch 1 Sep 2026 | zm-online 01.09.2026 | supported | |
| Germany first EU launch | FoodNavigator 06-Aug-2026 | supported | |
| Demand "noch nicht so groß" | leinetal24/dpa 06.10.2026 | supported | Quote from ABDA president |
| Lean mass 35.2 / 25.4 / 26.8 % vs lifestyle 26.2 % (p = 0.42) vs + resistance training 17.5 %; 20 RCTs, n = 15,782 | PMID 41877354 | supported | |
| Protein 0.8 g/kg/d reference; "1.2–1.6 g/kg/d" proposed during active weight reduction; "micronutrient or protein supplementation as needed" | PMID 40450457, PMC12612741 full text | supported | Full text read via Europe PMC REST |
| ~75–80 % at 12 months reimbursed T2DM vs "below 10 %" obesity/out-of-pocket (Poland, Colombia); GI intolerance and cost | PMID 42280404 | supported | Narrative review; [A] acceptable |
| 31.7 % stopped in 180 days; 26.8 % ADR, 14.4 % cost, 11.2 % non-adherence; n = 1,374 | PMID 41713959 | supported | US Kaiser cohort, semaglutide/liraglutide 2018–23, mixed diabetes/obesity: not self-payers |
| "weight regain and the deterioration of multiple cardiometabolic risk factors are common" | PMID 42168641 | supported | Verbatim |
| Hair/skin/nail supplements over-index (users); OTC digestive (considerers) | YouGov 53834 | supported, date wrong | Issue 4 |
| G-BA chair: "welche Patientengruppen …, wie lange, mit welchen Begleitmaßnahmen" (3 Aug 2026) | Apotheken Umschau | supported | Opened via WebFetch (curl bot-checked); chair Sonja Optendrenk |
| AOK chief ~€45bn/yr if all BMI ≥30 treated (24 Aug 2026) | Apotheken Umschau | supported | Carola Reimann, AOK-Bundesverband; she calls it a maximum scenario; €14bn at BMI ≥35 |
| § 34 SGB V exclusion upheld for Mounjaro (7 Feb 2025) | apotheke adhoc | supported | LSG Baden-Württemberg, interim-relief appeal |
| Semaglutide EU protection to 19 Mar 2031; India generics ~$15/month (26 May 2026) | apotheke adhoc | supported | |
| TUM Prof. Hauner quoted on online prescribing (2 Oct 2025) | apotheke adhoc (SWR) | supported | |
| G-BA commissions IQWiG guideline update DMP Adipositas, 8 Jul 2026; "Empfehlungen zu digitalen medizinischen Anwendungen" | G-BA decision PDF | supported | Report due Jul 2027 |
| DAG: DMP implementation "hapere" (10 Aug 2026) | PZ | supported | |
| LG München I 4 HK O 15458/24, 3 Mar 2025; "persönlicher ärztlicher Kontakt … erforderlich"; § 10 HWG | LG München I press release 3/2025 | supported | Also § 9 HWG (remote treatment ads); not final |
| "keine Wirknachweise … in der Regel unzulässig, da krankheitsbezogen"; § 10 HWG | Verbraucherzentrale GLP-1 supplements FAQ | supported | |
| Source of protein ≥12 % energy; high protein ≥20 %; muscle-mass claim authorised for source-of-protein foods | EC Knowledge4Policy | supported | EC page, [A] acceptable; Reg. 432/2012 wording not re-read (as the brief says) |
| MDSW that suggests dosage adjustments | MDCG 2019-11 rev.1 | unverifiable this run | HTTP 503 (curl and WebFetch). Not contradicted |
| GoLighter: free nutrition counselling with drug; free WW; "Mit einem ärztlich verschriebenen Abnehmmedikament … kostenfrei" | golighter.de, /p/ernaehrungsberatung | supported | Quote is on the home page |
| Care packages €19.99 (2 products), €32.99 (4), shipping free | golighter.de/p/care-pakete | supported | |
| GoLighter × WW from 1 Sep 2026 | apotheke adhoc branch news 01.09.2026 | supported | Vendor release; [B] with that label is fine |
| "ab 99 Euro monatlich" (29 Sep 2025) | apotheke adhoc branch news | supported | Vendor text |
| Operator facts: Monheim am Rhein | golighter.de/fakten-unternehmen | supported | |
| Wellster 2024: revenue €9,940,963; net loss €3,120,307; 51 FTE avg; "München" | Audited accounts (lobby register) | supported | Revenue is from "Betrieb von Plattformen zur Vermittlung…" (intermediation), which supports the brief's guess that the €50m is a gross or group figure. 2023 revenue was €11.56m: revenue fell in 2024 |
| 2025 "EUR50 million in revenue", "full profitability"; Mangrove, Claret | InforCapital 23 Mar 2026 | supported | Deal-aggregator; [B] is generous, keep with "not reconciled" note |
| Series B $60m; "aus München erstmals profitabel" | wellsterhealth.com/newsroom | supported | Series B dated 18 Jan 2022 |
| WW GLP-1 programme €45 / €31.50 / €11.25 (12-month, 75 % promo, "2026 Peak") | weightwatchers.com/de/preise page data | supported | GLP-1 programme is in the "Basis+" (premium) tier. The cheaper "Basis" tier (€25 / €17.50 / €10) does not list it |
| "Nach der Spritze" programme "soll unter 129 € kosten", waitlist | nachderspritze.de | supported | Its programme (2 strength sessions/week, protein target, small-portion recipes, weekly check-in) matches section 4 point by point |
| ESN Designer Whey €49.90 / 908 g | esn.com products.json (limit=250) | supported | |
| Voy €173 (up to €349; Max from €230); Menwell Ltd | myvoy.de (+ imprint/terms) | supported, promo | Issue 9 |
| Hims & Hers completes Eucalyptus/Juniper; DE since Mar 2023; "particularly … women" | Pulse 2.0 06.06.2026 | supported | Except "up to $1.15bn": not supported (issue 6) |
| Hims & Hers FY2025 revenue $2,347.6m, marketing $919.3m (39.2 %); FY2024 $1,476.5m / $678.8m (46.0 %) | SEC XBRL companyfacts | supported | Re-computed from `MarketingExpense` and `RevenueFromContractWithCustomerExcludingAssessedTax` |
| Obesity DiGA BMI 30–40; zanadio ">50.000-mal"; Oviva ">800.000" (2024) | PTAheute 04.03.2026 | supported | Class IIa not here (issue 7) |
| Gerresheimer GLP-1 support app for pharma | gerresheimer.com | partially | Issue 8 |
| Nupo GLP-1 guide; 10 bars €29.99 | nupo.de blog, products.json | supported | |
| Arla "Nutzer möchten keine Sonderrolle einnehmen" (6 Oct 2026) | t-online/dpa | supported | Verbatim (sentence continues "…sondern Teil der Gemeinschaft sein…") |
| Herbalife GLP-1 Nutrition Companion US/Puerto Rico, Feb 2024 | Herbalife IR | supported | Opened this run (issue 10) |
| glp-1forum.de: "1.200+ Mitglieder", Klick-Rechner, side-effect barometer, "Dosis splitten", founder quote "plötzlich hatte ich hundert Fragen…" | glp-1forum.de | supported | Founder named on page; the brief correctly does not name him |
| Contract maker MOQ 2,000 units, 8–12 weeks | `research/consumer-health-scan.md` (wonnda/BIOPAK) | supported (repo, fact-checked 2026-11-14) | One EU maker |
| PharmaSGP 44 % (2019) | `research/futrue-benchmark.md` | supported (repo) | |
| Start?Zuschuss! 50 %, max €36,000, round 23 25 Nov 2026 – 10 Jan 2027; EXIST to 31 Dec 2027; Calm/Storm | `research/munich-ecosystem.md` | supported (repo) | BayDiGuP: issue 12 |

**Re-run counts (App Store recipes)**
| Count | Brief | Re-run 2026-11-15 | Result |
|---|---|---|---|
| Shotsy DE review feed pages 1–3 | 150 reviews, Jun 2025 – Nov 2026 | 150, 28 Jun 2025 – 7 Nov 2026 (page 4 adds 28 older) | match |
| Shotsy keyword counts (free version / not worth it / gladly pay) | 14 / 3 / 4 | 15 / 3 / 2 with my regexes (the brief does not give its patterns) | approximate match; the counts do not drive any conclusion |
| Shotsy quotes (3) | dates and stars | 30 Oct 2026 2★; 3 Oct 2025 5★; 12 Aug 2026 5★, all verbatim | match |
| Juniper DE | 96 ratings, avg 3.79; 25 written reviews May–Nov 2026 | 96, 3.79; 25 (9 May – 10 Nov 2026); quotes at 19 Jul 2026 2★ and 29 Sep 2026 1★, verbatim | match |
| Shotsy ratings | 1,738 | 1,738 (lookup API) | match |
| GLP-1 tracker apps (5 terms) | ≥25, most 2025–26, most <60 ratings | 131 unique apps, well over 25 tracker-like; most released 2025–26 with <60 ratings; Shotsy the largest dedicated tracker (WW app far larger) | match (≥25 holds) |

**Arithmetic (section 5)**
| Item | Re-computed | Result |
|---|---|---|
| 100,000 / 300,000 / 550,000 × €180 | €18m / €54m / €99m | match |
| €1m ÷ €180 | 5,556; 5.6 % of 100,000 | match |
| 2,500 × €180 = €450,000; 0.4 × 450,000 = €180,000 | | match |
| 0.39 × 180 = 70.2; 0.46 × 180 = 82.8; 3-month case €35–41 | | match |
| €1m × 0.39–0.46 = €390–460k marketing | brief says "~€400–460k" | match (rounded) |
| €30/month ≈ €129 per 12 weeks | €30/month = ~€83 per 12 weeks | **mismatch** (issue 1) |
| Pass mark ≥40 sign-ups per theme for €300 | theme budget is €150 | **mismatch** (issue 2) |

## Evidence grades
- Grades are correct overall. The market size (€18m) rests on IQVIA [B], not on [C]. App and forum voices are tagged [C] and used only as a signal ("do not show willingness to pay").
- bifg (BARMER research institute, claims data) is graded [B]; [A] would be defensible. No change needed.
- InforCapital (deal aggregator relaying a press claim) at [B] is generous; the brief already flags the figure as not reconciled.
- Stale data: IQVIA end-2024 (under 2 years old), flagged. No item older than 3 years is used for sizing.
- Snippet-only items are labelled (pflueger.de, Juniper prices, OLG appeal, Herbalife). Herbalife is now opened (issue 10).

## [UNVERIFIED] items
| Item | Treated as fact or built on? |
|---|---|
| pflueger.de: supplements/protein alone do not prevent muscle loss | No: used as counter-evidence only |
| Juniper €172 then €299 per 28 days | No: not in any calculation |
| Contract-maker unit price | No |
| May ads name "Abnehmspritze" users (lawyer question) | No: the test plan uses neutral wording unless cleared |
| OLG München 29 U 1035/25 outcome | No |
| GDPR details | No |
| Meta/Google health-ad rules | Only as "check first" in the test plan. OK |
| 10 % waitlist-to-paid conversion (labelled *assumption*, not [UNVERIFIED]) | **Yes**: the pass mark is built on it. Labelled as an assumption, which is acceptable, but R2 contradicts it (issue 3) |
| 6-month paid life (assumption) | Yes: all of section 5. Labelled as an assumption; acceptable for a brief |

No fabrication found: every quote traces to an opened URL. There are no interviews (none claimed).

## Caveats (not fixes)
- The discontinuation-reasons study (PMID 41713959) is a US insured cohort with mixed diabetes and obesity patients. "Cost is a reason to stop" is supported, but the 14.4 % share should not be read as a German self-payer figure. The brief does not do that.
- Hims & Hers and PharmaSGP marketing shares are company-wide, mature-company averages. The brief says the allowance is "derived from company-wide marketing shares" (Gaps). Whether it is a fair benchmark for a new brand is a red-team question.
