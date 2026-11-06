# Review: research/pain-patients.md (A3)
Date: 2026-11-06 | Verdict: pass (minor fixes)

Strong, honest file. It puts payer counter-evidence (WIdO "fehlender Bedarf") next to advocacy figures (VdK €12bn), flags stale data, and refuses to size from the VdK claim. 20 sources and 4 App Store review feeds were re-opened on 2026-11-06. All checked numbers match, and the App Store low-star counts reproduce exactly (DAK 87, BARMER 92, TK-Ident 92, 116117 61 / 26 "Termin"). The issues are about counting and selection, not fabrication.

## Critical issues (must fix)
None blocking. Should-fix items (task A14):
1. **[C] signal counts in the summary table break the table's own definition.** The header says "Signals = independent items I opened". But:
   - P1 says "9 threads (rheuma-online)", while Details P1 shows 8 of 21 *titles* on page 1 and 4 opened threads (70019, 69869, 72569, 70589).
   - P3 says "104 relative threads on krebs-kompass", which are *titles* on two index pages, 18 of them about orientation, none opened for P3.
   - P8 counts "18/104 titles" next to 5 opened threads.

   B1 will read these columns as evidence strength. Split each cell into "opened" vs "titles only".
2. **ePA onboarding (Findings bullet 5, P10): the app selection biases the result.** The three apps tallied are the worst-rated standalone ePA/ident apps (1.3–2.5★). TK-Ident's only purpose is identification, so login complaints are close to tautological. Contrast (App Store search API, 2026-11-06): several insurer main apps that describe ePA functions are rated 4.5–4.7 (IKK classic 4.51, hkk 4.46, Audi BKK 4.58, BMW BKK 4.70), while the HEK app scores 3.54. "Patients are hitting the ePA wall at identity onboarding" is a real signal, but its size is unknown. Reword it to "standalone ident/ePA apps draw heavy onboarding complaints", and add the integrated-app contrast. P10 is already deprioritised, so the impact is low.
3. **The €469/month out-of-pocket figure applies only to users of those services and is self-estimated** (Findings bullet 3; P1 WTP column "€469/month out of pocket"). WIdO: "bezogen auf diejenigen, die diese in Anspruch nehmen … Die Angaben beruhen auf einer Selbsteinschätzung". As written, it reads as an average across carer households. This matters if B1 uses it as private WTP.

## Should fix
- **P7 "~19m hospital patients/yr `[B]`"** has no URL. Either add Destatis Krankenhausstatistik or mark it `[UNVERIFIED]`.
- **P4 "25% of GKV insured wait >30 days"** (Findings): the source says "25 Prozent der **Patienten**", i.e. respondents with a specialist visit. The Findings also date the GKV-SV release "5 Jan 2026". The page I opened shows survey fieldwork 21 Feb–25 Mar 2025, and I could not confirm the release date. Check it.
- **AOK ProDialog "91% satisfied with nurses"**: the PDF text layout is garbled. "79 Prozent" for discharge questions is clear, but I could not tie 91 % to nursing satisfaction (it sits next to "endoprothetischen Eingriffen" / "Prostatakrebs-Op"). Re-check the comparison figure.
- **P1 "~4.9m people cared for at home"**: per the trends review (issue 4), this includes ~640,000 Pflegegrad-1 people who use no services. Note it as the upper bound for a navigation TAM.
- **Navigator review [A]**: the abstract was read via Europe PMC, not the full text. The verdict "no effect" is per endpoint (153 endpoints), not per project. Say "most endpoints showed no effect".

## Source check (re-opened 2026-11-06)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| >3m assessments 2025; 9 in 10 at home; 59.6 / 11.2 / 19.3 / 9.4 % | MD Bund PM 15 Jul 2026 | supported | |
| Counselling use 3 % | GKV-SV § 7a report | supported | |
| ~⅓ non-users unaware; video <1 %; 2 % care not secured, often carer overload | GKV-SV PM 21 Jul 2026 | supported | |
| €2.95bn 2023, ~55 %; WIdO 2022 76.7 % / 38.4 %; "zu bürokratisch … zu gering" | AOK G+G 07/2024 | supported | |
| WIdO: 59 % employed; 45.2 %; 46.9 %; €469 / €677; 12.5 %; "fehlender Bedarf" 43.2 / 52 %; 55.2 % Pflegegeld-only use nothing else | WIdO PM 11 May 2026 | supported | €469 among users only (issue 3) |
| DEVAP: 150 home-care services, 91 % refused new clients, "teils jede zweite Anfrage", 9–12 months | DEVAP Jan 2023 | supported | Stale, provider association (flagged) |
| VdK Bavaria: 84 %, 93 %, 87 %, "mindestens zwölf Milliarden", 18→82 % | VdK PDF | supported | Advocacy (flagged) |
| 25 % >30 days; 30 % waits too long; 50 % vs 31 % online booking; 65 % phone/in person; n=3,520 | GKV-SV PM | supported | "Patients" not "insured"; date unclear |
| 42 days 2024 (+9); BRH €2.9bn; 40m unpaid specialist appointments | AOK G+G Apr 2026 | supported | |
| 1,514 notifications / 1,041 shortages; antipsychotics 230 days; >4m patients (lipid-lowering + antibiotics) | Zi Jan 2026 | supported | |
| 5.85m active ePA, ~8 %, 9 of 10 want to keep it | zm-online / BfDI | supported | |
| Discharge "79 Prozent" | AOK ProDialog 2025 | partially | 91 % comparison unclear |
| Navigator review: 31 projects, 153 endpoints, mostly no effect, 5 higher costs | Bundesgesundheitsbl. 2026 (abstract) | supported | |
| App Store: DAK 87 / BARMER 92 / TK-Ident 92 low-star of 100; 116117 61 low / 26 "Termin" | iTunes RSS p1+p2 | supported | Reproduced. My identification keyword set gives 49/52/51 among low-star (file: 41/47/44), which is consistent given the different regex |
| rheuma-online "Entlastungsbetrag nicht ganz"; krebs-kompass "warten, warten" | threads | supported | Verbatim |
| Not re-opened: Ärzteblatt objection rates, sonntagsblatt, AGVP/MV/NRW, Eurocarers, DAlzG, Zi TSS, vdek psychotherapy via G+G, BPtK, ABDA, Forsa, praktischArzt BARMER, Cardiolotse, intersec-CM, EJHG Rare Barometer, bpb 2015, BMG Leistungsbeträge | — | not checked | Sample-based |

## [UNVERIFIED] items
All are labelled and none is built on as fact:
- ME/CFS figures.
- Rural GP access.
- ~4m rare-disease patients in DE.
- § 39 Abs. 1a discharge duty.
- vdek "refusals ≠ undersupply".
- Psychotherapy private pay.
- 24-h care household numbers.
- Dementia home-care share.
- Employer spend on carers.

One watch item: P3's "Employers … possible B2B2C buyer" is labelled `[UNVERIFIED]`. B1 must not score P3's payer criterion on it.

## Missing evidence
- **P1's core contradiction is unresolved:** information gap (VdK: counselling lifts relief-budget use 18→82 %) vs preference (WIdO). The VdK figure is correlational. People who seek counselling may already intend to use services. No causal evidence exists either way. This is the #1 question for a care-navigation idea, and only interviews or a pilot can answer it (Stage D).
- **Who pays for P1:** the file correctly notes that raising benefit uptake *spends* Pflegekasse money in a deficit year. The only non-payer buyers named (care providers billing the relief budget, employers) have no evidence yet.
- **P2 has zero opened [C] items.** A retry of the caregiver forums, or the Reddit key, would help. Its [B] base (DEVAP 2023) is stale and comes from a provider association.
- **EU transferability:** only Eurocarers (advocacy). This is fine for Stage A, but needed before any "then EU" claim in a brief.

## Assumptions to challenge
- "Strongest patient-side problem = navigating home-care benefits." This is strong on [A] usage data, but weak on willingness to pay. Carers are not the payer, the payer would be paying to spend more, and the navigator evidence shows no cost effect. It may still be a good problem, but not an obviously fundable one.
- "Specialist access is a mass-market pain with digital workarounds" (P4). The file's own inference is right that capacity and the budget cap bind, not booking. Make sure B1 doesn't score P4 on the 25 % figure alone.
