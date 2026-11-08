# Fact-check: research/longlist-scoring-fields.md (A18), research/longlist.md (A23 changes), research/scoring.md (A25 changes)
Date: 2026-11-08 | Verdict: **pass with minor fixes (caveats only, see rule 14)** | Sources checked: 49 of ~75 (all 26 A18 vendor/statistics URLs that the tables rely on, all 6 new A25 URLs, 9 of 9 A23 URLs, plus 4 TED API queries). Not opened: Google-search-only items marked snippet-only in the files.

Scope: files changed since the last fact-check (2026-11-07-scoring-v3-and-A22.md, run 8): `longlist-scoring-fields.md` (never fact-checked; red-teamed only), `longlist.md` (A18 pointer + A23 restructure: 30 → 27 rows, "spend on the job" column, clusters, L25, L02, L10/L19/L30 decisions), `scoring.md` (A25). Other research files are unchanged since their last review. The long list and scoring.md have had their fix round (rule 14), so remaining issues below are **caveats for the CEO, not tasks**. No issue changes a CEO decision outright, so no `ceo` task was added.

Fetch note: WebFetch could not resolve most hosts; all pages were fetched with curl (HTTP 200) and read as text. PDFs were read with pdftotext.

## Critical issues (must fix)
None. No fabricated quote, customer or number found. The A25 fixes (8 of 8 from the last review) are applied correctly.

## Caveats (listed for the CEO and B1; no new tasks)
1. **"Seven wedges now have a young vendor with a named customer" is overstated (longlist-scoring-fields.md, Findings, first bullet).** The table under it lists seven vendors, but two have no named customer by its own columns: CrewLinQ (`">100 Pflegeeinrichtungen", none named`) and calliora (`Still no named hospital`). The CrewLinQ PDF confirms only "In über 100 Pflegeeinrichtungen wird der Matching-Algorithmus ..." and a staff quote from an unnamed-organisation context. At most five wedges (voize, heycare, Gesundheit von Morgen, Flinn, Recare) have a named customer, and two of those fail or leave open the age test (voize 2020; Recare founding year not found; Gesundheit von Morgen founding year not found). Only heycare and Flinn pass today. B1 should read the table, not the headline.
2. **"Category leader (S2): Yes" for Recare and Flinn has no source for "leader" (Table 1 findings; L08 and L29 rows).** The cited Flinn page calls Flinn "the leading provider of AI-powered software ..." (company self-description). For Recare, no opened source says it leads; the files only show a Köln award and 12 Knappschaftskliniken. The criterion-8 reductions that rest on "leader" are therefore inference. voize "leader" rests on the earlier $50m / 1,100 facilities data (not re-opened).
3. **Flinn "$20m Series A" (longlist-scoring-fields.md, L29 row) is not in the cited source.** The LISAvienna page says "Flinn receives $20 million" and "secures an additional $20 million"; the string "Series A" does not appear. Drop the label or source it. (Customers Carl Zeiss, Philips, Paul Hartmann and the Hartmann SVP quote, 19 Feb 2026, are supported; "formed earlier this year" in tech.eu, 20 Dec 2022, is supported.)
4. **L23 evidence mixes two kinds of MD AI tender (longlist.md L23 row; scoring-fields Table 2 L23).** L23 is "MD care-need assessments". TED 762721-2026 (MD Nordrhein, deadline 3 Dec 2026, re-run: matches) is titled "KI-gestützte Gutachtenerstellung im medizinischen Fachbereich **Behandlungsfehler**", i.e. malpractice reviews, not care assessments. `pain-industry.md` says this correctly; the L23 row does not. Also, TED 343840-2025 (cited in `pain-industry.md` as MD Nordrhein malpractice) is an **MD Rheinland-Pfalz** "Gutachtenerstellung Pflege" notice per the TED API (buyer-name check). So only the MD RLP procedure (closed) is care-assessment evidence; the open MD Nordrhein tender is a neighbouring job. Counts reproduce: 53 MD notices since 1 Jan 2026 (match) and 9 MD notices with "KI/Künstliche" in the title since 2025 (match; buyers: Bayern 2, Nordrhein 2, RLP 5). The file says these "cover 5 procedures", which is a reasonable grouping.
5. **"TED shows no award notice" for MD RLP (longlist.md Findings) is imprecise.** TED has a result notice (`can-standard`) from MD RLP dated 24 Jul 2025 on the same subject (483916-2025). The API returns no winner for it, which is consistent with "no award", but the sentence should say "a result notice without a winner". MD Nordrhein 95051-2025 (`can-standard`, 12 Feb 2025) does return a winner flagged "small".
6. **"Proven spend" label for L01 rests on a vendor claim.** L01 counts as *proven* because heycare's customers are named "laut Unternehmen" (Munich Startup and Trending Topics both say "According to the company" / "Zu den Kunden zählen bereits"). No contract, tender or customer statement was seen. L09 is *proven* for rostering software (a different product from the shift-pool wedge), and L29 rests on a customer quote from a press release the vendor issued. The "8 of 27" count is arithmetically right (8 + 4 commissioned + 3 vendor-market + 12 other = 27; 13 clusters, 6 single-row: matches), but 3 of the 8 are weaker than L07/L21/L22 (awards, notices).
7. **Hospital row L05 trigger (RLP § 19a) is vendor-sourced (as the file says).** Verified against the voize blog: in force "seit dem 1. Oktober 2026", signed "am 22. September 2026", "0,5 Vollzeitstellen, davon 0,4 Pflegefachkräfte und 0,1 Pflegehilfskräfte" (§ 19a Abs. 3). The blog also claims "bis zu 37.000 € pro Jahr" refinancing; the file does not repeat that number, which is right.
8. **Mobil Krankenkasse date.** The press release is dated "Hamburg, 07.05.2026" in the text; the page metadata says published 2026-05-04 / updated 04.05.2026. The file uses 7 May, matching the dateline. Fine.
9. **Stale/old data not flagged inline:** ~375 health offices (2020, flagged "stale"), ~266 live-in agencies (2017, `[UNVERIFIED]`, flagged), DEVAP 91 % (Jan 2023, flagged). Care-home counts are 15 Dec 2023 (flagged). No further staleness issues.

## Source check
### longlist-scoring-fields.md (A18)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| voize founded 2020 | invest-in.berlin | supported | "Founded in 2020 by twin brothers ..." |
| voize × Caritasverband Stuttgart, "Start mit voize: Januar 2022", 700 staff | voize case page | supported | "Start mit voize: Januar 2022"; "700 in der stationären Altenpflege" |
| voize × Kreszentia-Stift München, Jul 2023 | voize case page | supported | "Start mit voize: Juli 2023" |
| RLP § 19a: 0.5 FTE since 1 Oct 2026, signed 22 Sep 2026 | voize blog | supported (vendor source, contract text not opened, as stated) | |
| heycare founded 2022 as Heynanny; Daimler Truck, Douglas, Vaillant, VW Retail (Mar 2026) | munich-startup.de, trendingtopics.eu | supported | Both say customers "according to the company" |
| Gesundheit von Morgen × ZF BKK, 9 Jul 2026, free online courses | zfbkk.de | supported | Page date 09.07.2026 |
| Gesundheit von Morgen × Mobil Krankenkasse, 7 May 2026 | mobil-krankenkasse.de | supported | Dateline 07.05.2026; fee not stated |
| Flinn customers; Hartmann SVP RA quote, 19 Feb 2026 | lisavienna.at | supported | "Series A" not in source (caveat 3) |
| Flinn founded 2022 | tech.eu 20 Dec 2022 | supported | "formed earlier this year" |
| Recare × Uniklinik Köln, KHZG tender, 7 Nov 2023 | medcon PDF | supported | "Ausschreibungsverfahren im Rahmen des KHZG", dated 07.11.2023 |
| Recare: 12 Knappschaftskliniken via Telekom (Apr 2023) | telekom.com | supported | "zwölf Knappschaftskliniken", 03.04.2023 |
| CrewLinQ ">100 Pflegeeinrichtungen", no named customer | ConSozial PDF | supported | Quote "In über 100 Pflegeeinrichtungen ..."; Potsdam quote appears in the PDF (line seen), file says snippet-only: conservative |
| Tandem Health ">10,000 facilities in 14 countries incl. Germany" | telekom.com Oct 2026 | supported | Also "around 130 electronic health record" integrations |
| Tandem founded 2023 Stockholm; T-Systems KIS in >250 clinics (per Tandem) | trendingtopics.eu | supported | |
| TechBoost needs "marketable product and ... initial B2B customer projects"; Connect needs MVP + commercial register | techboost.telekom.com | supported | Exact wording |
| MPIRIQ no named paying customer | munich-startup.de | supported (absence) | Interview text opened; no customer named in the matched passages |
| Debeka × iuvando Health, 22 Oct 2025; iuvando founded 2019 | cash-online.de, uni-heidelberg.de | supported | Fee not stated |
| Apo-Mall "Bestell-Engel", ~1,100 users | apotheke-adhoc.de | supported | "rund 1100 Nutzerinnen und Nutzer" |
| Doctolib acquires aaron.ai, 22 May 2024 | aerzteblatt.de | supported | "Mittwoch, 22. Mai 2024" |
| MD Niedersachsen external DRG review, TED 383478-2026, 4 lots of €500k, deadline 3 Jul 2026 | TED API | supported | 4 lots × 500,000; deadline 2026-07-03 |
| 53 MD notices since 1 Jan 2026; 9 with KI in title since 2025 | TED API | match | Re-run counts equal |
| 1,807 hospitals: 529 public, 549 non-profit, 729 private (2025) | destatis PD26_376 | supported | |
| 16,505 care homes, 15,549 home-care services (15 Dec 2023) | destatis table | supported | |
| 42 % of care homes private (2023) | kbv.de | supported | "liegt 2023 bei 42 Prozent der Pflegeheime" |
| 18,632 legal units with ≥250 employees (2024) | destatis table | supported | "Insgesamt ... 18 632" in the 250+ column |
| ~98,000 practices, ~4,900 MVZ | Hartmannbund PDF | supported | |
| 92 Kassen | gkv-spitzenverband.de | supported | "92 Ergebnisse (Stand: 08.11.2026)" (file says 07.11): date nit |
| PKV-Verband: 39 ordinary + 10 extraordinary members | Lobbyregister PDF | supported | |
| 1,480 medtech firms >20 staff, ~12,000 micro | BVMed PDF | supported | |
| ~375 health offices (2020) | kommunalwiki | not re-checked in detail | flagged stale in file |
| Table 2 snippet-only items (AOK Hessen, adesso/Verisk, KV-Connect 170 PVS, 50-cent fee, Kulmbach, LÄKH, Decisive Consulting, CH 274 hospitals) | none opened | unverifiable | Correctly labelled "search snippet only" and not used as fact |

### longlist.md (A23 changes)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| Last ÖGD-pact tranche €750m in 2026 "zur abschließenden Erfüllung der im Pakt für den ÖGD gemachten Zusagen" | BT-Drs. 21/8237 | supported | Text lines "Zur abschließenden Erfüllung ...", "um 750.000.000 Euro erhöht" |
| 2027: "Für den ÖGD sind null Euro eingeplant" | zm-online.de | supported | |
| KVSH "DRG-Grouper zur kostenfreien Nutzung" (25 Mar 2024) | KVSH PDF | supported | |
| KVBW grouper in member portal since 13 Feb 2025 | kvbawue.de | supported | Page dated 13 Feb 2025 |
| Verbund Pflegehilfe "berät seit 2008 kostenlos", 1.5m consultations/yr, Entlass-Manager, Ortenau/Altenburger Land, >41,000 providers | pflegehilfe.org PDF | supported | |
| § 342 Abs. 1 SGB V "zugelassene" ePA; § 291 Abs. 8 "im Benehmen mit dem BSI"; § 325 Abs. 1 approval | gesetze-im-internet | supported | Wording matches; § 325 content only counted, not quoted |
| Hybrid DRG § 115f deleted, short-stay flat rates 2028 | BR-Drs. 620/26 | supported | "§ 115f wird gestrichen"; Kurzzeitfallpauschale 2028 |
| 8 proven / 4 commissioned / 3 vendor market / 12 other = 27; 13 clusters, 6 single | own table | match | Recounted from the table |
| MD RLP re-tender closed 5 Sep 2025 | TED (earlier review) | supported | Not re-queried; see caveat 5 |

### scoring.md (A25 changes)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| EU threshold €216,000 (sub-central supplies/services), 2026-27 | IHK Hannover | supported | "fuer Liefer- und Dienstleistungen bei 216.000 Euro ... gelten also bis Ende 2027". The page does not mention § 106 GWB or the central-government €140,000; those come from the next row |
| "221 000 EUR" replaced by "216 000 EUR" | Delegated Reg. (EU) 2025/2152 | supported | Two replacements in the German text. The 143,000 → 140,000 central change and the "sub-central" reading were not located in the lines matched (text has two replacements of 221,000 only); treat the €140,000 as [B]/unverified |
| voize founded 2020; Caritas Stuttgart Jan 2022 | invest-in.berlin; voize case page | supported | Fixes review item 7 |
| fuer-gruender.de "Gegründet im Jahr: 2020", 6 Mar 2020 | fuer-gruender.de | not opened | Third voize source, redundant; not needed |
| L03 pain 4 M, WIdO 46.9 % "hoch belastet", 45.2 % cut hours | `pain-patients.md` P3 via WIdO PDF | supported internally | WIdO PDF not re-opened (checked in earlier reviews) |
| L21 recalculated 64 / 59; L03 59 / 52 | arithmetic | match | L21: 70 − (5−3)×3 = 64; R4 64 − 3 − 2 = 59. L03: 12+4+9+8+6+5+6+4+5 = 59; R4 59 − 2 − 3 − 2 = 52 |
| Direct-award table: €15,000 for federal-level bodies only | BAS circular (earlier review) | supported | Fix applied |
| L21 K2 → "unproven"; caery site unreachable | self-reported search | unverifiable | Not re-searched |

Arithmetic in the calibration section reproduces. All eight issues from `2026-11-07-scoring-v3-and-A22.md` are closed: (1) L03 pain cell present, (2) L03 K1 wording, (3) L21 K2 unproven, (4) UKL-GPT scoped, (5) €15,000 scope, (6) L06 wording, (7) voize sourced, (8) IHK Hannover cited. Remaining nit: the A25 line for the EU thresholds says "central government €140,000" and cites the Delegated Regulation for both amounts; only the €216,000 change was confirmed in the German text pulled here.

## [UNVERIFIED] items
All carried correctly as `[UNVERIFIED]` and not built on in later text: Bavarian university-hospital and municipal-GmbH below-threshold limits; Gesundheit von Morgen, caery, CrewLinQ (2021, aggregator), Recare founding years; ~266 live-in agencies (2017); recruiting fees (L11); pharma patient-finding spend (L18); 50-cent shortage fee; radiology approval counts; outsourcing/DORA rules for PKV; sites count for L27. Two places lean on unverified premises in a softer way: the criterion-8 "leader" label for Recare (caveat 2) and the "age test open" rows (the CEO decision on how to measure age is still open, as the file says).

## Evidence grades
Grades are plausible: vendor case pages and press releases are [B]; Destatis, TED, BT/BR documents and laws are [A]. The two vendor-sourced "customer" claims (heycare, Flinn) are correctly tagged [B] but, as "laut Unternehmen" claims, should not feed a "proven" status (caveat 6). The [C] layer is unchanged (thin; stated in the file).

## Re-run counts
| Recipe | Result |
|---|---|
| TED: MD buyer notices since 1 Jan 2026 | 53: match |
| TED: MD notices with KI/Künstliche in title since 2025 | 9: match |
| TED 383478-2026 value, lots, deadline | 4 × €500k, 3 Jul 2026: match |
| Long-list row/cluster/spend-status counts | 27 / 13 / 8-4-3-12: match |
