# Fact-check: research/futrue-benchmark.md and research/consumer-health-scan.md
Date 2026-11-14 | Mode: FACT-CHECK (C10, first half; red team still open) | Verdict: **pass, minor fixes** (both files) | Sources checked: futrue-benchmark 19 of 20 (all except EUR-Lex, which the file itself says it could not open); consumer-health-scan 41 of 54 (all critical-path claims: market frame, economics, every top-5 spend and need figure, claims law; plus PubMed abstracts for 9 of 13 papers). Not opened: Mumsnet threads (3, [C]), Cochrane tinnitus, Gutenberg tinnitus, RKI migraine, WHO, IQVIA UK blog, VZ NRW, test.de, Forbes-cited Perrigo year, gesetze-im-internet.de § 5 NemV (connection reset, unverifiable this run).

## Critical issues (must fix)
None. No fabricated quote, no [C]-only sizing, no [UNVERIFIED] item used as fact. All filed numbers (PharmaSGP prospectus, ad-hoc 11 Jul 2025, Hims & Hers 10-K) match the source. The scoring table re-computes exactly (script re-run, 12 rows: base and R4 totals all match).

## Issues to note (minor; no fix task, listed for the CEO as caveats)
1. **A € figure per category was in an opened source but reported as "not found".** `consumer-health-scan.md` Gaps: "No € market size per indication". The cited Lebensmittel Praxis article (same URL as the protein claim) says, citing NielsenIQ: stomach and digestion products made **€419m in Germany in 2024**, and weight-reduction products **€204m**, the largest item in that category ([Lebensmittel Praxis, 29 Jul 2025](https://lebensmittelpraxis.de/industrie-aktuell/45294-trends-im-sortiment-kategorie-otc-bietet-chancen.html) [B]). The weight row instead relies on 2015 data and "flat at 3.0m packs". Effect: under the file's own score key (5 = brand revenue; 4 = category data) the weight and IBS spend scores do not change, so **no rank changes**; the gap line and row 4 should cite it.
2. **IBS spend 5H rests on one estimate that does not match the score key.** Score key: "Spend 5 = brand revenue in DACH". Source: Forbes "estimates" SYNformulas "generated about $100 million in revenue … in 2024" ([Forbes, 12 Sep 2025](https://www.forbes.com.au/news/billionaires/this-pharma-billionaire-is-developing-a-cannabis-painkiller-to-replace-dangerous-opioids/) [B]): a journalist's estimate for the whole company (all products, all countries), not DACH IBS revenue. 4M fits better. *My math:* IBS base 38 → 36; top 5 stays the same five rows (menopause 38, bladder 38, GLP-1 37, IBS 36, fertility 36). **No decision change.**
3. **Unsourced claim:** "seven figures (XbyX, Femna)" (§5) and "Femna" in §7. No Femna source is cited anywhere in the file. XbyX is supported (Börsen-Zeitung).
4. **Scope stretch:** "added value of devices 'very uncertain'" (row 8, §7.3). The Cochrane 2024 abstract says this of **PFMT with a resistance device vs without** (3 trials, 227 women, very low certainty). It does not test app-connected biofeedback trainers such as Perifit or Elvie. Partially supported.
5. **FUTRUE revenue series attributed to the wrong entity (partially).** `futrue-benchmark.md` §3: "Dr. Fischer Gesundheitsprodukte revenue €1.7m (2011) → … €47.5m, ~70 staff". apotheke adhoc (Oct 2015) gives this series for the "Schwesterfirma mit rund 70 Mitarbeitern", and splits it into Deseo €14m and Rubax €10m. Those are the brands of PharmaSGP's predecessor, not of Dr. Fischer Gesundheitsprodukte.
6. **Unclear claim:** "IPO June 2020 (FUTRUE sold, 90 % of offered shares)" (§1). The prospectus says FUTRUE held **90.0 % of the share capital** before the offering, and both selling shareholders sold. apotheke adhoc (Jun 2025) says the founders "gaben damals ein Drittel der Anteile ab". "90 % of offered shares" was not found.
7. **Small date/fact nits:** Natsana "founded 2020": the source says "Anfang 2020 hatten mehrere Gründer diese Marken zusammengebracht" (brands merged, not founded); acceptable. Femibion's 60 % share is "in Apotheken" under Merck (2016); the file says this correctly in context.
8. **Unverifiable this run:** pelvina (Ärzte Zeitung) now returns a JavaScript challenge page. Gesetze-im-internet.de reset the connection (§ 5 NemV). Both were cited as opened by the researcher; not contradicted.

## Source check (critical path + sample)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| FUTRUE founded 2008, >20 firms, >90 approvals, <180 staff per firm, VER-01 approved Jul 2026 | futrue.com | supported | Company self-description [B], correct grade |
| Fischer b. 1975, TUM 1995–2001, HBS 2003–05, Novartis board 2006–08; Hohlefelder b. 1981, HSG, BCG 2008 | PharmaSGP CVs 2021 | supported | |
| FUTRUE GmbH, Am Haag 14, Gräfelfing; Fischer sole shareholder | prospectus | supported | |
| Revenue €53.1m (2017) / €62.6m (2019); EBIT €15.3m / €22.4m; materials €5.9m; personnel €2.0m | prospectus | supported | 27.8/62.6 = 44.4 %, 5.9/62.6 = 9.4 % re-computed |
| Marketing €27.8m (2019) | prospectus | supported | |
| 36 third-party manufacturers; one logistics provider per country; up to 30 % of units via pharmacist/physician endorsement; 38 unused authorisations; break-even within 3–6 months or drop | prospectus | supported | |
| Homeopathic route; skepticism risk; print decline risk; "untapped demand" | prospectus | supported | Quotes verbatim |
| 2024 revenue €118.8m, adj. EBITDA margin 31.3 %; 2025 guidance €132–138m, EBITDA €37–39m | ad-hoc 11 Jul 2025 | supported | [A] correct |
| Buy-back €28/share, founders back to 90 %, delisting | apotheke adhoc Jun 2025 | supported | |
| SYNformulas ~$100m revenue, 30 % margin, $1bn fortune; Perrigo $150m | Forbes Sep 2025 | supported | Estimate; see issue 2 |
| Kijimea flop 2009, Ebeling, media-for-revenue SevenVentures, Lactostop to Dermapharm ~€15m, "Ideengeber" | apotheke adhoc Oct 2015 | supported | Revenue series: partially (issue 5) |
| Yokebe ad spend €20m = sales (2013, Nielsen); Almased just under 50 % pharmacy share; Naturwohl ~€27m; price not named | apotheke adhoc Jul 2015 | supported | Article says Yokebe introduced 2010; file notes the 2009/2010 conflict |
| 3 years' preparation; Synformulas €25m, PharmaSGP €63m (AVP); 40-person field force | apotheke adhoc Sep 2018 | supported | |
| ~€100m gross ad spend; 4-month ideal development | CHEManager 2016 | supported | |
| Sunday Natural to CVC, EV ~€800m incl. debt, Jan 2024 | Börsen-Zeitung | supported | Paywalled; teaser and date confirm |
| MOQ 2,000 units (capsules/powder) | wonnda/BIOPAK | supported | Vendor directory [B] |
| SevenVentures media-for-equity/revenue; €3m prize; Evela semi-final, 22 Oct 2025 | ProSiebenSat.1 | supported | |
| Greenforce seven-figure media-for-equity | Munich Startup | supported | |
| Private households €65bn, 12.1 % of €538.2bn (2024) | Ärzteblatt on Destatis | supported | Article also gives a 2025 estimate of €579.5bn; the file uses 2024 correctly |
| MDR Rule 21: body orifice; class IIb "in all other cases" | AESGP paper | supported | |
| Kijimea "Medizinprodukt", Synformulas GmbH | kijimea.de | supported | |
| Kijimea RCT: 443 patients, 34 % vs 19 %, RR 1.7, p = 0.0007 | PubMed 32277872 | supported | |
| OTC €6.7bn (+5 %), ~910m packs; non-Rx + health products €12.012bn (+7.1 %); self-medication €10.154bn; mail order €3.572bn (+10.7 %), 294m packs | IQVIA Q4 2024 | supported | |
| €13.8bn incl. mass market; 1.71bn packs, 40 % mass market; category pack table (11 rows) | IQVIA / Healthcare Marketing 4/2025 | supported | All 11 rows spot-checked: 602.9, 264.7, 177.3, 59.2, 39.1, 3.0 match |
| Protein products 6.8m → 11.1m units; Bayer 30 % → 100 % early 2025 | Lebensmittel Praxis | supported | Also contains €419m / €204m NIQ figures (issue 1) |
| Natsana €87m revenue, €19m loss; Bayer 30 % May 2022, full takeover; own sites, Amazon, dm/Rossmann | apotheke adhoc Jul 2024 | supported | |
| Snuggs €20m revenue 2024, positive EBITDA, ~3,000 stores, €12m funding, founded 2019 | tech.eu | supported | |
| Folic-acid products ~€86m (manufacturer prices), 3.7m packs; Femibion 60 %, Folio 14 %, Orthomol 6 % | apotheke adhoc Oct 2016 | supported | Stale (flagged in file) |
| ~100,000 private AOM users in Germany end-2024 | IQVIA blog Dec 2024 | supported | "almost 100,000" |
| >4m households use or consider GLP-1 drugs | YouGov Jan 2026 | supported | |
| Mounjaro up to €490/month, Wegovy up to €276 | ZDF | supported | |
| Lean mass 25–39 % of weight lost; 20 RCTs, n = 15,782 | PubMed 41877354 | supported | |
| "Wir sind auf dem Weg zu einem reinen Selbstzahler-Markt"; Drogerie purchases | Apotheken Umschau Feb 2026 | supported | |
| ~10m people with urinary incontinence | Deutsche Kontinenz Gesellschaft | supported | "Etwa 10 Millionen Menschen" (all forms; file notes this) |
| 48.3 % UI prevalence, women 18+ | PubMed 28401541 | supported | Stale (flagged) |
| PFMT first-line; device add-on "very uncertain" | Cochrane 2024 | partially | Issue 4 |
| Perifit FDA 510(k), Feb 2023 | FemTech Insider | supported | |
| "gibt es keine Wirknachweise … Die Werbung ist in der Regel unzulässig" | Verbraucherzentrale GLP-1 FAQ | supported | Verbatim |
| Disease claims banned for foods; plant claims unassessed | Verbraucherzentrale Klartext NEM | supported | Article 7(3) LMIV named in file; page says "Krankheitsbezug … für Lebensmittel immer" verboten |
| "Über neun Millionen Frauen" aged 40–55 | Apotheken Umschau Sep 2024 | supported | Head count, not symptom prevalence (red-team point) |
| REALISE: 57.6 % OTC use (moderate-severe VMS) | PubMed 39208496 | supported | Physician-recruited, 1,767 women |
| CBT: 16 studies, 910 women | PubMed 41462190 | supported | |
| XbyX seven-figure round, 30 Jan 2023; Evela €600k, 19 May 2025; Frieda €2.5m | Börsen-Zeitung, startbase, Maximon | supported | Femna: no source (issue 3) |
| IBS Rome IV 4.1 % internet / 1.5 % household, n = 73,076 | PubMed 32294476 | supported | |
| Minoxidil only high-evidence drug for female hair loss | PubMed 37003900 | supported | |
| Migraine supplements, 22 trials | PubMed 39404918 | supported | |
| Kalmeda price agreed with GKV-SV | apotheke adhoc Jul 2022 | supported | |
| 8 % use sleeping pills | TK Schlafstudie 2017 | supported | "Acht Prozent greifen zu Schlafmitteln"; stale (flagged) |
| Hims & Hers revenue $1,476.5m, marketing $678.8m, gross margin 79 % (82 % in 2023), CAC $594.5m, subscribers 1,537k → 2,229k | 10-K FY2024 | supported | Math re-run: 594.5 / 0.692 = $859 |
| pelvina €74.99, 80–100 % refunded | Ärzte Zeitung 2018 | unverifiable | JS challenge page this run |
| Supplement notification to BVL | § 5 NemV | unverifiable | Site reset connection this run |

**Arithmetic re-run:** 1,000,000 / 360 = 2,778 customers; 44–46 % of €1m = €440–460k; 0.8 × €30 = €24; R2/R4 scoring for all 12 rows: match.

**Grades:** correct throughout. Filings and PubMed [A]; trade press and company sites [B]; Mumsnet [C], used only as pain signal, without usernames. Snippet-only items (Nestlé US, oral semaglutide EU, Priorin, profil.at, cerascreen) are labelled as such and not built on.

## [UNVERIFIED] items
| Item | Treated as fact later? |
|---|---|
| Probiotic claim risk for IBS (claims score 2) | No; it lowers a score (conservative) |
| EU device class of pelvic-floor trainers (retailer pages only) | Partly: row 8 route "Class I device + app" and K2 "pass" rest on it. Flagged; the file's own cheapest test (EUDAMED check) covers it |
| Washable incontinence underwear as textile / class I | Same pattern, row 21 K2 pass |
| IVD self-tests need a notified body | Used only to exclude row 14 (conservative) |
| Amazon ACoS; contract-maker unit price | Not built on; €3/unit is labelled "not sourced, illustrative" |
| Oral semaglutide in the EU (2026) | Not built on |
| First-batch cost (futrue-benchmark §7) | Not built on |
| Psychotherapy wait spend (row 16) | Row excluded |

**Red team (second half of C10): open.** Not done in this run.
