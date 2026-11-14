# Fact-check: research/parked-ideas-screen.md
Date 2026-11-14 | Mode: FACT-CHECK | Verdict: **pass, minor fixes** | Sources checked: 17 of 18 opened-source entries (all except § 393 SGB V: gesetze-im-internet.de returned a connection reset and HTTP 503 this run). TED recipe re-run for 7 of 10 notice numbers.

## Critical issues (must fix)
None. Every price, count and award that drives the ranking matches its source, and all customer-count arithmetic re-computes. No quote without a traceable URL. [UNVERIFIED] items are not built on.

## Issues to note (minor; caveats for the CEO)
1. **Price range misstated.** Findings and L13: "October 2026 price lists: €69–229 a month (10 vendors)". The medizinio page says the prices "reichen von 9 € bis 229 € pro Monat", and the file's own list includes Eterno €9, VITAS €49 + €0.28 per conversation and Mediform €75 + €0.15/min. The low end is €9 (standalone) or €49, not €69. This strengthens the file's own "price is collapsing" point. It does not change the L13 verdict.
2. **Gross vs net prices are mixed.** IONOS All-Flat Advanced €99 is **brutto** (gross, incl. VAT) in the kopfundstift table, while the medizinio prices are mostly **netto**. The comparison "€99 flat" vs "€99–199" slightly overstates IONOS's price relative to others. Minor.
3. **Grade borderline:** kopfundstift is a blog comparison table, graded [B, blog]. Acceptable because the file labels it, but the IONOS price could be confirmed on ionos.de in one fetch.
4. **"calliora ($6m pre-seed …)" [B]:** the cited startupvalley interview supports the Max Planck PhDs and "Häuser in fünf Bundesländern", but the $6m figure was not found on the two cited pages. It is presumably carried over from the repo; the file should mark it "(repo)".
5. **Not re-checked:** the Lausitz "mind. 1.000.000 EUR" turnover requirement (214386-2026) and the Stuttgart PIN wording (515360-2026). The notices exist with the stated buyer and notice type; the full text was not opened in this run.

## Source check
| Claim | Source | Verdict | Note |
|---|---|---|---|
| LMU Klinikum award to Tiplu (57060-2025) | TED API | supported | can-standard, winner Tiplu GmbH |
| UK Würzburg award to Tiplu, €545,250 (278914-2025) | TED API | supported | tender-value 545250.00 |
| MU Lausitz award to Tiplu, 60 months, value withheld (552501-2026) | TED API | supported | tender-value −1, duration 60 |
| Lausitz CN (214386-2026), Stuttgart PIN (515360-2026), Caritas VEAT (366802-2026) | TED API | supported (existence, buyer, type) | Wording not re-read (issue 5) |
| Harzklinikum LLM-letter tender (492877-2025, 28 Jul 2025), no award | TED API | supported | Re-query by buyer since Aug 2025: 4 notices. The only CAN (568406-2025) is a PDMS award to NEXUS, a different procedure |
| LOGEX to become sole shareholder of Tiplu, 8 Jul 2026 | Thoma Bravo | supported | [B] correct |
| calliora: hospitals in five states, unnamed; Max Planck PhDs | startupvalley | supported | $6m not found (issue 4) |
| calliora.com names no customer | calliora.com | supported | |
| 10 vendor prices, "Datenstand: Herstellerangaben, Oktober 2026" | medizinio | supported | Range misstated (issue 1) |
| IONOS All-Flat €99, all calls; table dated 13 Nov 2026 | kopfundstift | supported | Gross price (issue 2) |
| fonio founded autumn 2024, >7,000 customers, ARR "knapp unter 7 Millionen Dollar", €14.6m seed, €120m valuation, >€20m total | Trending Topics | supported | |
| One100: "zehn Einrichtungen", >300 practices by end of 2026 | Trending Topics | supported | |
| Sinalis: TUM.ai hackathon, €10,000 prize money | Munich Startup | supported | |
| SVLFG Q1 2026: account 04510 Pflegekurse €52,792.33; benefits €254,940,956.39 | SVLFG PV45 | supported | [A] correct |
| SPV benefits 2025 €70.42bn | BMG Finanzentwicklung | supported | |
| PflegeBetreuer, Mobil Krankenkasse, 7 May 2026 | Mobil Krankenkasse | supported | Page now loads; the date matches |
| curendo "Kostenfrei dank Übernahme durch Ihre Pflegekasse" | pflege.de | supported | |
| Dragon Copilot GA 7 Oct 2025; Charité, Mannheim, Stuttgart, Halle, Hannover | Microsoft News | supported | |
| "Trusted by 200+ global MedTech & IVD Leaders" | flinn.ai | supported | Self-claim [B] |
| MDR proposal 16 Dec 2025: PSUR in year 1, then every two years | Arthur Cox | supported | |
| MDCG 2019-11 rev. 1 (Jun 2025), "simple search" exclusion | MDCG PDF | supported | [A] correct |
| C5 attestation, Type 1 for 18 months then Type 2 | § 393 SGB V | unverifiable | Site down this run (503); not contradicted |

**Arithmetic re-run (all match):** L07 €180k / €60.6k = 3.0, / €40k = 4.5 → 3–5; €1m / €60.6k–40k = 16.5–25 → 17–25. L13 €180k / €2,388–1,188 = 75–152; €1m → 419–842; year-2 practice-years 63–125. L03 52,792.33 / 254,940,956.39 = 0.0207 % × €70.42bn = €14.6m. Cash: €10k + €90k + €30k + €36k = €166k. fonio $7m / 7,000 ≈ $1,000.

## [UNVERIFIED] items
| Item | Treated as fact later? |
|---|---|
| C5 audit cost | No |
| Number of independent (non-chain) private hospitals | No; the file says the L07 pool is "not counted" |
| Hospital sales-cycle length | No; stated as inference |
| AI Act Art. 50 date (snippet) | No |
| Mediform €1.5m (snippet) | No; labelled snippet |
| L29 price €10–30k and L06 €30–100k (unsourced A18 guesses) | Used for counts but labelled "unsourced" in the table; the verdicts (drop) do not rest on them |

No fix task added: no critical issue. Issue 1 is a one-line correction the researcher can make in any later edit of the file.
