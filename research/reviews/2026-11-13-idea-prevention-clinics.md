# Fact-check: research/idea-prevention-clinics.md (researcher C2, idea check)
Date: 2026-11-13 | Verdict: **pass (minor fixes)** | Sources checked: 50 of 50 listed URLs opened (all), plus the 3 TED notices the file uses

Scope: new since the last fact-check run. The C4 revision of `ventures/eldercare-navigator/brief.md` reached `main` during this run and is covered in `2026-11-13-eldercare-navigator-brief-C4.md`. Mode FACT-CHECK only: the business idea and the scores as judgement are not assessed here.

How opened: 47 URLs by curl with local text extraction; TED through the v3 API; the Atomico job ad through WebFetch (curl: 403); the PubMed abstract through NCBI E-utilities (the page shows a bot check).

**Summary.** No fabrication. Every quote I checked is verbatim and traceable. All figures behind the verdict reproduce: YEARS prices, Neko 2025 accounts, the Aware insolvency and the €100,000 sale, Art. 18 HKaG, Aeon in Munich, Neko's 2027 plan, the Cochrane and Eur Radiol results, the tax rule, both TED notices and the Präventionsbericht amounts. The score arithmetic is correct. No critical issue. Eight minor points follow; none changes the verdict "drop the clinic" or the CEO options in C5.

**Counts re-run (2026-11-13): all match.**
- App Store, Aware (id 1609437818): 60 ratings, average 4.3; feed has 21 reviews: 11 five-star, 7 one-star, 2 two-star, 1 three-star. Themes in the 9 low reviews: price 6, appointments or sites 4. The three excerpts are verbatim with the stated month.
- App Store, wellabe: 41 ratings, average 4.68. Seller name "Mavie Work Deutschland GmbH".
- Hacker News item 40235129: 53 comments, 10 top-level; the quote is verbatim.
- TED: 594202-2026 (WBM, contract notice, 28 Aug 2026), 370897-2026 and 664823-2026 (IKK classic, contract notice and award) return as described.
- Score math (weights 3,2,3,2,2,1,2,2,1): A = 50, B = 52, C = 54, R4 for C = 49. Shortlist placements (L01 66/62, L07 63/58 and the rest) match `research/shortlist.md`.

## Critical issues (must fix)
None.

## Minor issues (caveats; no fix task)
1. **Stale sources not flagged; two support "proven spend" for the employer wedge.**
   - TUM "Manager-Check" brochure: the PDF was created on 6 Jul 2017 (file metadata). Sections 2 and 5 and the K1 cell "Pass (WBM, IKK classic, TUM)" use it in the present tense.
   - AXA wellabe flyer: print code "(6.21)", PDF from July 2021. Section 5 says wellabe is "sold through AXA's bKV". That predates the sale to Mavie (Sep 2024); whether AXA still sells it is not shown.
   - BÄK "Leistungen auf Verlangen": a Deutsches Ärzteblatt text of 14 Jun 2002. Bayerisches Ärzteblatt: 10/2015 (the statute itself was checked in its current version, so this one is harmless).
   - Effect: K1 for wedge C still passes on the two 2026 TED notices alone.
2. **IKK classic €604,750 is a framework value, not money spent.** Notice 664823-2026: "Eine Abrufverpflichtung der Auftraggeberin aus der Rahmenvereinbarung besteht nicht ... Verbindliche Umsatzvolumen werden nicht garantiert." The Findings line "awarded ... for €604,750" and the label "Proven spend" should say "framework, no purchase obligation". WBM is a contract notice only: no award and no value yet (the file says "tendered", which is correct).
3. **Finding 3 is firmer than the file's own gap list.** "A non-physician founder with €10k cannot own the clinic. A physician must own and run the practice, or the company only brokers." Art. 18 Abs. 1 Satz 2 HKaG is quoted correctly. But section 3 marks the § 30 GewO route `[UNVERIFIED]`, the Gaps section says "not researched; legal opinion needed", and the file's own sources show a third route: an MVZ "kann ... auch als GmbH geführt werden" (Bayerisches Ärzteblatt 10/2015), which investors reach by buying a hospital (Capital 3/2024). Correct wording: a company cannot run a practice directly; the other routes are out of reach at €10k or unverified. The practical conclusion holds.
4. **Snippet-only prices sit in a row graded [B] without the `[UNVERIFIED]` tag.** AYUN "CHF 3,134 starter" and Function Health "$365 a year" are marked "(snippet only)"; neither appears on the cited page. Rule 1 asks for the tag. Function's price is also missing from the Gaps list. Neither number is used in arithmetic.
5. **"Must be marked on the bill" is not in the cited BÄK text.** The page says a private bill must show the service, fee position, multiplier and amount, and that GOÄ rules apply to services on request. The marking duty is not stated there (it would need § 12 Abs. 3 GOÄ, not cited). Partially supported.
6. **MRI running cost: the source contradicts itself.** medizinio's text gives "ca. 180.000 € netto/Jahr (Strom, Helium, Wasserkühlung)"; its own cost table gives "Betriebskosten ... ca. 20.000 € (pro Jahr)". The page is an undated lead-generation portal, so [B] is generous. The inference "seven-figure sum before the first customer" holds on purchase plus installation alone (€750,000 + €350,000).
7. **Small overstatements.**
   - "GKV pays only the statutory check-up (§ 25 SGB V) [A]": § 25 states the entitlement; "only" is the researcher's inference.
   - bKV "60,600 firms and over 2.8m people": the PKV page counts "betriebliche Kranken- oder Pflegeversicherung"; 450,000 of the 2.8m hold care insurance.
   - "PKV (8.74m fully insured)": this is the 2024 figure (press release of 4 Jun 2025); no year given.
   - Hacker News "most are sceptical or questioning": of the 10 top-level comments, 3 are bare links and 2 only quote the article; about 5 are sceptical or questioning.
   - Neko "New York" and "no MRI": not in the cited TechCrunch or heise pages (TechCrunch, Jan 2025: US clinics are being prepared). "No MRI" appears only as a quote inside the HN thread [C].
   - "Check-up imaging must be MRI or ultrasound": inference from § 84 StrlSchG; ordinances under § 84 Abs. 2 can allow specific X-ray screening. Not checked further.
8. **Small attribution points.**
   - Gaps: "FG Nürnberg ruling on check-ups (revision VI R 9/25 pending): snippet only". The IWW article already cited contains it, and it concerns "einem mehrwöchigen Gesundheitstraining", not check-ups.
   - The YEARS press release carries the note "This is a paid press release"; the Allianz sentence is YEARS' own claim.
   - Forward: Maginative says $400m raised; the Capital article in the same source list says "667 Mio. Dollar". Pick one and name it.
   - Eur Radiol: the abstract adds "Most studies had a moderate to serious risk of bias"; worth one clause next to the 1.57 %.
   - K1 "Pass" for wedges A and B cites "YEARS, Aeon" (a price list and vendor statements). Under `scoring.md` fix 4 a price list counts only with a paying customer. The paid-purchase evidence in the file is Aware (€450 membership; paying users in the reviews [C]) and IGeL turnover [B]. Does not matter for the outcome: A and B are dropped.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| YEARS €1,990 / €7,600 / €16,900; 87 to 230+ biomarkers; MRI, liquid biopsy, genome | years.co cost page | supported | Page updated 16 Oct 2026 |
| Lanserhof €7,000–50,000+; Preventicum €2,000–7,000; Deutsche Klinik für Prävention, Oberaudorf | years.co cost page | supported | Competitor's estimates, as the file says |
| Metamedicum (ex Preventicum), Essen and Düsseldorf; Aeon via partner clinics | years.co overview | supported | |
| YEARS: two years open, capacity +50 %, Allianz bKV | webdisclosure press release, 28 Sep 2026 | supported | Paid press release |
| Neko 2025: revenue SEK 157m, net loss SEK 677m (from 215m), staff 161 → 433, €150m convertible loan | Finwire/Placera, 10 Jul 2026 | supported | |
| Neko $260m Series B at $1.8bn; waitlist above 100,000; £300 | TechCrunch, 22 Jan 2025 | supported | |
| Neko about €240 in Sweden | heise, 23 Jan 2025 | supported | SEK 2,750 |
| "Germany represents Neko's next international market, with launch planned for 2027"; Berlin; 28 May 2026 | Atomico careers | supported | Via WebFetch |
| Cochrane: "little or no effect on the risk of death from any cause (high-certainty evidence)"; 15 trials, 251,891 participants | cochrane.org | supported | 17 trials included, 15 with outcome data; search to 31 Jan 2018 (flagged in Gaps) |
| Whole-body MRI: 1.57 %, 10 studies, 9,024 people, "may lead to unnecessary investigations" | PubMed 40884613 | supported | Eur Radiol 2026;36(3):1813 |
| Aware: insolvency May 2026, about $15m in 2022, €450 a year, 99 biomarkers, 25 sites | Apotheke Adhoc, 1 Jun 2026 | supported | Provisional proceedings opened 21 May |
| Aware: 45 sites, tests €9.95–69.95, sold to Aeon "für gerade einmal 100.000 Euro" | Apotheke Adhoc, 6 Oct 2026 | supported | |
| Forward: $400m raised, 19 clinics, under $100m revenue, closed Nov 2024 | Maginative, 13 Nov 2024 | supported | See minor 8 |
| Art. 18 Abs. 1 Satz 2 HKaG quote; "Text gilt ab: 01.01.2025" | gesetze-bayern.de | supported | |
| Bavarian Constitutional Court upheld the ban in 1999 | Bayerisches Ärzteblatt 10/2015 | supported | Ruling of 13 Dec 1999 |
| § 95 Abs. 1a SGB V founders of an MVZ | gesetze-im-internet.de | supported | |
| Investors buy a hospital first | Capital 3/2024 | supported | |
| § 30 GewO concession for private clinics | gesetze-im-internet.de | supported | Applicability `[UNVERIFIED]`, as marked |
| § 84 Abs. 1 and § 5 Abs. 16 StrlSchG quotes | gesetze-im-internet.de | supported | |
| Aeon terms: "Wir vermitteln dir medizinische Behandlungen ..." | aeon.life terms | supported | |
| Aeon Munich: Beyond Imaging, Rosenheimer Str. 30; seven German cities | aeon.life | supported | Prices not in the page text, as stated |
| Aeon €8.2m seed (Jun 2025); total above $14m; founded 2023; "live in Germany since early 2026"; Aware assets | tech.eu, TFN | supported | |
| Aeon own data on 2,731 people, 2022–2026 | aeon.life/de | supported | "Interne Daten" |
| AYUN "More than 1,500 clients, CHF 2.7 million in revenue"; crowdfunding | ayun.ch | supported | CHF 3,134: not on page |
| Function Health $298m Series B at $2.5bn; MRI at 130 sites | TechCrunch, 19 Nov 2025 | supported | $365: not on page |
| IGeL "mindestens 2,4 Milliarden Euro"; 2,013 insured; forsa | Ärzteblatt, 3 Dec 2024 | supported | |
| Check-up use 19.2 %, AOK NordWest, Schleswig-Holstein, 2024 | AOK press release, 13 Aug 2025 | supported | |
| Prevention spending 2024: €686,182,779; €281,956,037; €218,409,854; €185,816,888 | Präventionsbericht 2025 | supported | |
| MB/KK § 1: "nach gesetzlich eingeführten Programmen" | pkv.de PDF | supported | |
| 8.74m fully insured | PKV press release, 4 Jun 2025 | supported | 2024 figure |
| Services on request must be marked on the bill | BÄK GOÄ-Ratgeber | partially | Minor 5; text from 2002 |
| TUM: billed by GOÄ; "Die Kosten trägt das jeweilige Unternehmen auf Basis eines Rahmenvertrags" | TUM brochure | supported, stale | PDF from 2017 |
| WBM framework for executive check-ups, Aug 2026; references required | TED 594202-2026 | supported | Two references; contract notice |
| IKK classic, insa Gesundheitsmanagement, €604,750, 4 bids; references required | TED 664823-2026, 370897-2026 | supported | Framework without purchase obligation (minor 2) |
| bKV: 60,600 firms, over 2.8m people, +16 %; Allianz new business +58 % | pkv.de, Allianz release 19 May 2026 | supported | Includes care insurance (minor 7) |
| § 3 Nr. 34 EStG: €600, §§ 20 and 20b SGB V | gesetze-im-internet.de | supported | |
| BMF 2021 Rz. 37 quote; 1982 ruling removed from the 2026 wage-tax notes | IWW, 28 Jul 2026 | supported | |
| MRI €750,000 to over €3,500,000; used from €160,000; installation €350,000; maintenance €85,000 | medizinio | supported | |
| MRI running cost €180,000 a year | medizinio | partially | Table on the same page says €20,000 (minor 6) |
| Diagnostik München "Pionier der modernen Vorsorgemedizin" | kliniken.de | supported | Self-description |
| wellabe: founded 2018, "around 100 B2B customers", Mavie bought 60 % | Munich Startup, 3 Sep 2024 | supported | |
| wellabe: 60 values in 20 minutes; sold through AXA's bKV | AXA flyer | supported, stale | 2021 |
| Präventionsfonds: up to €500,000, max. 90 %, sketches by 16 Oct 2026, exercise promotion | StMGP call | supported | |
| Aware reviews, wellabe ratings, HN thread | iTunes, HN API | supported | Counts match |

## [UNVERIFIED] items
| Item | Where | Built on? |
|---|---|---|
| Whether § 30 GewO fits an outpatient check-up centre; management-company structure | Section 3, Gaps | Partly: Finding 3 is worded as if no company route existed (minor 3) |
| HWG / UWG rulings on longevity adverts (1 search) | Section 3 | No |
| Biogena Plaza München, opened 17 Sep 2026 (snippet) | Section 5 | No |
| Neko $700m round, New York price $499 (snippet) | Gaps | No. "New York" still appears in the section 1 table without a source |
| Zoī, Paris (snippet) | Gaps | No |
| AYUN CHF 3,134; Function $365 (snippet, not tagged) | Section 1 | No (minor 4) |
| Pabau software page (snippet) | Section 4, wedge D | No: wedge D is out at K1 |
| FG Nürnberg ruling (listed as snippet only) | Gaps | No; it is in the cited IWW article (minor 8) |
| YEARS funding and accounts; Aeon German prices | Gaps | No |

## Not checked
- Fraunhofer (TED 394188-2023) and BARMER (371071-2023): the file does not use them.
- Whether an ordinance under § 84 Abs. 2 StrlSchG allows any X-ray screening relevant to check-ups.
- The scores as judgement (red team's job). No red-team review of this file exists; it is not one of the stage deliverables in the critic's red-team scope.
