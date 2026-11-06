# Review: research/pain-industry.md (A5)
Date: 2026-11-06 | Verdict: needs work (before A7 uses I5/I6 as "high WTP")

Well-sourced file. 22 sources were re-opened on 2026-11-06 (curl, Europe PMC REST, TED API v3, ClinicalTrials.gov API). The numbers mostly match exactly, and I reproduced the own ClinicalTrials.gov count (2015: 715/4,636; 2025: 622/5,912). The problem is interpretation: the tender evidence shows that buyers have a budget. It does not show that a startup could win that budget.

## Critical issues (must fix)
1. **Tenders used as "High WTP" have eligibility criteria that exclude a startup** (Findings bullet 3, summary table I5 "**High WTP**, clear buyer", Details I5 inference "clear, recurring, public budget"). I opened the selection criteria (`selection-criterion-description-lot`) of the notices cited:
   - AOK Hessen 761998-2025: "Allgemeiner Jahresumsatz (Jahre: 2022, 2023 und 2024): **6.000.000,00 EUR** (netto/je Jahr)". Bidders below this are "für die Auftragserfüllung nicht geeignet".
   - BIG direkt gesund 189396-2025: minimum turnover €250,000 in the last financial year, plus "drei Referenzen, die mit dem Auftragsgegenstand in Art und Umfang vergleichbar sind".
   - DAK 396194-2026: requires turnover and reference declarations. The text also says the work is outsourced "**weiterhin**", so this is a re-tender with an incumbent.
   - The same pattern applies to the hospital tenders in A4 (see that review).

   So the TED notices prove that buyers have a budget. They do not prove that a startup can sell into it. The realistic routes are subcontracting to or partnering with the incumbent BPO, or selling via channel partners (caery sells via Telekom TechBoost, per [Telekom PM](https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken)). Add an "accessible to a startup?" note per tender (min. turnover, references, certificates). Downgrade I5 WTP to "high buyer budget, low direct startup access" until a route is shown.
2. **DAK €890m is the claims volume processed, not what DAK pays** (Findings bullet 3, table I5 "DAK €890m/yr through an outsourcer"). Notice text: "Das zu verarbeitende **Nettoausgabenvolumen** beträgt ca. 890 Mio. Euro pro Abrechnungsjahr". The contract value is not stated (estimated value empty). In the table, the figure reads as spend on the outsourcer. That is a TAM-inflation risk for B1. Reword it and add the contract value once award notices are read (A12).
3. **"9 buyers tendered invoice/receipt processing" mixes different services** (Findings bullet 3, I5 list). AOK Hessen's notice title is "**Scanning** – Externes Belegmanagement"; its scope is intake, imaging, data capture and archiving. AOK BW, AOK Rheinland/Hamburg and Pronova BKK are also scan services or scan software, and hkk is pharmacy billing (§ 300). Only BIG and DAK (and possibly BAHN-BKK) include actual *Prüfung*. Split the list into "scan/intake BPO" and "billing check", because only the second matches an AI-checking idea.
4. **MD assessments "up from 1.52m in 2014 ([vdek])" is not in the cited source** (Findings bullet 4). The vdek page says "Die Zahl der **Pflegebedürftigen** hat sich seit 2014 auf mehr als 5,6 Millionen verdoppelt". That is people in need of care, not assessments, and no 1.52m figure appears. Source the figure or mark it `[UNVERIFIED]`.

## Should fix
- **The CTMS count is not recruitment competition.** Table I1 lists "65 CTMS products on Capterra DE" as WTP evidence for a *recruitment* problem. CTMS/EDC tools are trial-management software, not patient-finding tools. The real recruitment competitors (Trialbee, Viomedo, Trials24, Probando) are snippet-only. I could not reproduce the "65 Ergebnisse" count: the static HTML no longer contains it.
- **Barometer share inconsistency.** Findings say 3.0 % (2024, per the 2025 barometer). Details I1 quotes the 2026 barometer, "etwa 2,9 Prozent" for 2024. State both.
- **"72 % of university sites" is the sponsors' view of sites** (24 pharma + 25 CROs), not site data. The progress log and Findings phrase it as a fact about sites. Add "according to sponsors and CROs".
- **Unsourced counts:** "93 statutory insurers" (table I5) and "15 regional MDs" (table I6, Details I6) have no URL. Both are denominators for buyer counts. Add a GKV-SV / MD Bund source.
- **Grade inconsistency:** MD Bund's press release is [B] here but [A] in `pain-patients.md`. MD Bund is a statutory body, so [A] is defensible. Make the two files consistent.
- **Founder-fit claim:** I5/I6 "matches the 'payers' interest". The founder brief's sweet spot names "administrative burden", so this is fair. But the realistic sales motion (public procurement with references, or partnering with BITMARCK/gkv informatik) is the opposite of "first paying customer within ~12 months" (founder-brief "Achievable"). Say so.

## Source check (re-opened 2026-11-06)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 72 % of university sites under-recruit ≥25 %; 68 % at max-care; outlook +34→+7; Kapazitätsinitiative incl. digital patient identification | Ärzteblatt 28 Sep 2026 | supported | Sponsor/CRO survey |
| DE share 4.5 %→3.0 %; 33k→24k participants; MFG 26 days; 5 % incentive; "geringes Hemmnis" | vfa barometer Oct 2025 PDF | supported | |
| CT.gov DE 715/4,636 (2015) → 622/5,912 (2025) | CT.gov API v2 | supported | Reproduced exactly |
| EU trials −13.5 %, 1,989→1,721/yr, mostly non-commercial and phase IV | Lancet RH Eur 2026 (Europe PMC) | supported | The decline is mainly *academic*, which weakens its use for an industry-sponsor pitch |
| 347 RCTs, 31.1 % discontinued, 45.4 % poor recruitment; UK/CH/DE/CA | JAMA Netw Open 2025 | supported | Protocols from 2016 |
| EEA share 22 %→12 % (2013–2023); recruitment times | IQVIA/EFPIA 2024 | supported | |
| Biotech Act 106→76 days; 113 vs 60 days | Jones Day | paywalled/unverifiable | Cloudflare challenge on re-fetch |
| § 4 Abs. 5 SGB V admin cap from 2027 | buzer.de | supported | |
| ~€100m savings 2027 | krankenkasseninfo | supported | |
| 2024 admin €12.63bn, €169.54, 3.86 % | GKV-SV | supported | |
| Lünendonk 32 insurers, ~60 %, 97 % AI, few short-term savings, 78 % politics | Lünendonk PDF | supported | |
| caery "bis zu 10 Milliarden" | Telekom PM | supported | Vendor claim; caery is itself a startup (TechBoost partner), which is relevant to issue 1 |
| AOK Hessen 19,257,000 invoices | TED 761998-2025 | supported | Title "Scanning"; €6m turnover minimum (issue 1, 3) |
| DAK €890m, 2.0m receipts, 97.5 % DTA | TED 396194-2026 | partially | Volume processed, not contract value; "weiterhin" (issue 2) |
| BIG § 301/302 processing | TED 189396-2025 | supported | €250k turnover + 3 references |
| MD RLP AI PoC (mobility module, phases) | TED 343840-2025 | supported | |
| MD Nordrhein AI malpractice review | TED 762721-2026 | supported | |
| >3m care assessments 2025; 59.6 % Pflegegeld | MD Bund PM 15 Jul 2026 | supported | |
| 1.52m assessments in 2014 | vdek 2025-04 | not supported | Issue 4 |
| MDR QMS 19.5 / TD 21.8 months; 90 % personnel / 7 % NB fees | MedTech Europe 2025 | supported | |
| DACH 245 manufacturers; 53 % cut R&D; >40 % no EU launch; 64 % orphan | BVMed et al. 2025 | supported | The 64 % is 14 of 22 firms (small n), so say so |
| ~58 JCAs 2026; 57 % late LOIs | pharmaphorum | supported | |
| ÖGD pact "nicht zu begründen"; "Aus für … Digitalisierungsprojekte" | Ärzteblatt Feb 2026 | supported | |
| ICSRs +0.5 % | EMA 2025 report | supported | |
| PKV >70m invoices; 6,891 complaints | PKV | supported | 0.001 % ombudsman rate is a counter-signal on customer pain, worth adding |
| GOÄ 1 Jan 2028 "erreichbar" | PKV/BÄK 31 Jul 2026 | supported | |
| FDZ 82 institutions, 53 applications, claims data only | PZ | supported | |
| ICON 2.8 / "unbezahlte Überstunden"; MD Bayern "Arbeitsverdichtung" (204 reviews); krebs-kompass "Studien bisher überhaupt nicht" | kununu, krebs-kompass | supported | Quotes verbatim, no usernames |
| Capterra "65 Ergebnisse" | Capterra DE | not reproduced | See should-fix |
| Not re-opened: Trials 2021/2024, TIRS 2026, J Neural Transm, ACT/SCRS, EFPIA PICO, GKV-SV AMNOG, MHC, BVMed Herbstumfrage, BMG GKV 2025 (checked in the trends review), § 303e, ÖGD congress, kununu BARMER/DAK/AOK PLUS | — | not checked | Sample-based |

## [UNVERIFIED] items
- DACH recruitment vendors (Trialbee, Viomedo, Trials24, Probando): labelled. They are the actual I1 competitors, so A13 must verify them before I1 is scored.
- Biotech Act COM(2025)1022, MDR revision text, HTA Regulation dates: law-firm and trade-press summaries only. Labelled. The I4 "policy risk" verdict rests on them, which is acceptable for Stage A.
- PKV customer pain (Finanztip survey): labelled. Not built on.
- GKV staff retirement numbers: labelled. But Findings bullet 3 and Lünendonk's "Ruhestandswelle" drive the "people → automation" inference. The size of the wave is unknown.

## Missing evidence
- **Award notices** for the § 302 tenders: who won, at what value, and how many bidders (TED `can-standard`). Already in A12; add eligibility thresholds there.
- **The insurer IT oligopoly as gatekeeper:** whether BITMARCK, gkv informatik and AOK Systems integrate third-party AI, or build it themselves (gkv informatik tendered its own AI infrastructure, 76741-2025).
- **Site-side view for I1:** what sites are paid per recruited patient, and whether sites, not sponsors, would buy a tool. The file assumes the sponsor is the buyer.
- **Counter-source for the industry barometers:** the file pairs I1 with registry data, but I4 relies on the industry associations' surveys only.

## Assumptions to challenge
- "The admin cap pushes insurers from people to automation." It caps *all* admin spending growth, including new software and outsourcing. Under a cap, a buyer may defer new vendors rather than add them. Lünendonk itself: "Mit kurzfristigen Kostensenkungen rechnen die Kassen dagegen kaum".
- "Regulatory approval is no longer the main bottleneck → the gap is site staff time and patient finding." Sponsors rank site *staffing* first. A software tool does not add study nurses. The industry only added digital patient identification to its wish list in Sep 2026, so it is a wish, not demonstrated demand.
- "Even at 97.5 % electronic data, checking is still outsourced" (I5 inference). The outsourced work may be rule-based checking already automated by the incumbent. The notice does not say the work is manual.
