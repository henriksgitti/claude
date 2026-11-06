# Review: research/pain-professionals.md (A4)
Date: 2026-11-06 | Verdict: needs work (minor-to-moderate; fix before A7/B1)

Careful file. It pairs interest-group self-estimates with measured data (DKI 3 h vs DMW 93 min), states its own counter-evidence, and keeps kununu machine summaries at [C]. 21 sources and 4 TED notices were re-opened on 2026-11-06, and all checked numbers match. The issues are the same tender-access gap as in A5, one mislabelled tender with regulatory consequences, and small counting inconsistencies.

## Critical issues (must fix)
1. **The tenders behind "High WTP" (S1, S3, S8) exclude newcomers.** Selection criteria I opened (TED v3, `selection-criterion-description-lot`):
   - Charité coding 186365-2025: "Nachzuweisen sind 3 Referenzen … Mind. zwei Unternehmensreferenzen sind ein deutsches Universitätsklinikum. Mind. eine … ein deutscher Maximalversorger".
   - MUL Lausitz AI coding 214386-2026: annual turnover "in dem Tätigkeitsbereich des Auftrages … pro Jahr mind. **1.000.000 EUR**" for the last three years.
   - Helios discharge platform 24618-2025: a "KHZG-Zertifikat des Bundesamtes für Soziale Sicherung" and at least one reference from a hospital group.

   S3's "**High** WTP … fits the CEO's automation profile" and the Findings inference "revenue protection gives this the clearest budget owner" stay true for *incumbents*. For a pre-revenue startup, these buyers are unreachable by direct tender in year 1. Add per-tender eligibility thresholds and an "accessible to startup?" judgement. Name the non-tender route (pilot below the EU threshold, private hospital groups, subcontracting), or say none is known. A11 should pick this up.
2. **Harzklinikum 492877-2025 is a clinical decision-support system, not only discharge-letter drafting** (Findings bullet 3; Details S1 "AI discharge letters"). The notice describes "ein automatisiertes klinisches Entscheidungsunterstützungssystem … sollen in Echtzeit patientenindividuelle Hinweise zu möglichen Erkrankungen, Komplikationen oder Risiken generiert" (KHZG project 4.01). Software that generates patient-specific diagnostic or risk hints is likely medical-device software under MDR (classification rule 11). This is my inference and needs a primary source (MDR Annex VIII / MDCG 2019-11) before it is relied on. If it holds, it means certification cost and time for anyone selling into this tender type. Re-label it, and add a one-line regulatory caveat to S1: "documentation-only" tools vs CDSS features.

## Should fix
- **KHZG money is a one-off fund in its tail, not a recurring budget.** "Hospitals buy documentation tooling with public money" (Findings bullet 3) rests on 2025–26 tenders funded from KHZG (application rounds 2021–). The file correctly notes that the penalty shifts to *use*. Also state that new KHZG purchase money is not recurring. KHZG funding deadlines are `[UNVERIFIED]` here: verify with the BAS/KHSFV source in A9/A11.
- **"Leadership/communication complaints for 9 of 9"** (Findings bullet 5; table S9 "9/9 critical of leadership"). The S9 table itself marks Charité "mixed". Make it 8 of 9, or explain.
- **S2 "~1.8m professional nurses (DBfK)"**: no DBfK URL is given. The nearest opened source, [BT-Drs. 21/5270](https://dserver.bundestag.de/btd/21/052/2105270.pdf), gives 1,767,799 employees in *all* nursing occupations, hospitals included, so it is not a long-term/home-care headcount. Using it as "who has it" for S2 overstates the segment. Use Pflegestatistik staff counts for Pflegedienste and Pflegeheime.
- **S4 "~150,000 office-based physicians"** comes from the 2016 Ärzteblatt piece, which is stale. `research/trends.md` cites KBV 191,875 participants (incl. psychotherapists) for 2025/26. Use one current, defined number.
- **DKI's sample** is "400 Krankenhäuser" answering for their staff, i.e. management estimates. The file says so. Also note that the 38 %/35 % FTE equivalents are arithmetic on a self-estimate, so they should not appear in any sizing.
- **voize JMIR study:** the file flags conflict of interest ("check the authors' conflicts"), but this was not done. Either check it or tag the result "manufacturer-associated, unverified independence".

## Source check (re-opened 2026-11-06)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| 3 h / 2.8 h; 66,300 of 176,800 (38 %); 137,000 of 391,000 (35 %); 22,097 / 48,938; 88 %; n=400 | DKI 2025 PDF | supported | Management self-estimate |
| 93.1 min/day, 19.4 %, internists 120.2 min, 9 physicians, 216 h | DMW 2024 (Europe PMC) | supported | |
| n=528; 45 % 2.5–5 h; 52 % software helps "wenig bis gar nicht" | Landespflegekammer via DKG | supported | |
| Charité coding framework | TED 186365-2025 | supported | Reference requirement (issue 1) |
| Lausitz AI coding | TED 214386-2026 | supported | ≥€1m/yr in-field turnover (issue 1) |
| Harzklinikum "LLM-basierte Arztbriefschreibung", KHZG | TED 492877-2025 | partially | Scope is CDSS (issue 2) |
| Helios central discharge platform | TED 24618-2025 | supported | KHZG certificate + group reference |
| KHZG penalty ≤2 %; use weight 20 % (2027) → 80 % (2031) | GKV-SV/DKG agreement 2024 | supported | |
| Pflegebudget 2.5 % flat 2025; 2027 base minus 86 %; overruns not refinanced from 2027 | buzer § 6a KHEntgG | supported | |
| >2m working hours of free-form requests | KBV PM Mar 2025 | supported | |
| 23 proposals, ~€400m, 8 ten-hour days per practice | KBV Aug 2026 | supported | "BMG adopted 3" not re-checked |
| >50 % weekly/daily TI outages; 13 % mostly digital with hospitals; 87 % e-letters | KBV PraxisBarometer 2025 | supported | |
| MB-Monitor 9,649; 49 % overloaded; 28 % consider leaving; 59 % staffing poor; 42 % posts cut; ⅔ dissatisfied with IT | zm-online, praktischArzt | supported | |
| Agency nurses 42,649 (2023) → 31,503 (1.8 %); Bavaria 3,174 | BT-Drs. 21/5270 | supported | |
| voize −15 min/shift, 52 nurses, 14 facilities, 770 h | JMIR 2026 | supported | COI not checked (should-fix) |
| AI scribes −16.0 min / 8 h; after-hours unchanged; 8,581 clinicians | JAMA 2026 | supported | US *ambulatory* academic clinicians. Transfer to German inpatient wards is an assumption |
| voize $50m, 1,100 facilities | HealthCapital | supported | Company figures |
| Phone AI €9–229/month | medizinio | supported | Vendor-adjacent comparison site |
| BEEP passed 6 Nov 2025; documentation "auf das notwendige Maß" | BMG PM | supported | |
| 32,000 nursing / 13,900 physician recognitions 2025 | Destatis Aug 2026 | supported | |
| krankenschwester.de quotes ("Doppeldoku", "weit weniger intelligent", "unleserlich", "konkurrenzfähig", "Cloud-Server-Software … untersagt", "insgesamt gut"); medi-learn coding quote | forum threads | supported | Verbatim; no usernames in the file |
| Not re-opened: JAMIA 2026, ScanProCare!, Fraunhofer IML, DBfK 2026, RWI/idw, HNO survey, BA 2026, DKG DigitalRadar, GKV-SV audit page, kununu summaries, 2016 Bureaucracy Index | — | not checked | Sample-based |

## [UNVERIFIED] items
- MB-Monitor "3 h/day admin": labelled, not built on.
- KHVVG sample audits from 2027 and BStabG audit quota 10 %→15 %: labelled. **But S3's "rules change 2027" (summary table) leans on them.** Keep the table cell tied to the `[UNVERIFIED]` tag until A11 verifies them.
- Competitors myScribe, Doctolib scribe, Recare: snippet only, labelled.
- MFA shortage score, recruiter fees, § 8(8) SGB XI uptake: labelled, not built on.

## Missing evidence
- **MD audit volumes and repayment sums** (GKV-SV XLSX not opened). This is the size of S3's pain in euros, and it is the one number that would turn S3 from "budget owner exists" into a sizeable market. Covered by A11.
- **Coding/CDI incumbents and their prices** (A11).
- **Private and church hospital groups as non-tender buyers.** Most evidence is public tenders. Private chains (Helios, Asklepios, Sana, AMEOS) buy through group IT and are reachable without EU tenders below thresholds, but this is not explored.
- **Measured German inpatient effect of AI documentation.** Only ScanProCare! is German and inpatient. The JAMA and JAMIA studies are US ambulatory.

## Assumptions to challenge
- "Every audited euro is hospital revenue, so willingness to pay is direct" (S3). Hospitals already pay coders and medical controllers. The question is whether a startup tool beats the existing coding software plus outsourced coders. The Lausitz tender shows AI coding is already a tendered *product category*, i.e. incumbents exist.
- "The addressable slice is the hospital→practice discharge-letter flow" (S6). Through KIM and the ePA, this flow is being standardised by gematik. Check whether a startup layer survives the standard.
- Absence in kununu AI summaries ("Documentation/IT named: —") is not evidence of absence: the summaries are machine-written and cover only ~6 paragraphs. The file mostly treats it correctly ("do not let documentation tools borrow this pain"), but the 9-employer table should carry that caveat in its header.
