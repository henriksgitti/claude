# Scoring framework (Stage B)
Task: A20 (v3) | Date: 2026-11-07 | Status: draft

CEO decision 2026-11-07 (chat): keep the 9 criteria, add knock-outs K1/K2, and rank by confidence (rules R1–R4) instead of exact totals. Basis: `research/reviews/2026-11-07-redteam-scoring.md`. **v3 (A20):** must-fix 1–6 from `research/reviews/2026-11-07-redteam-scoring-v2.md` applied (CEO decision 2026-11-07, `decisions/2026-11-07-scoring-v2-and-timeline.md`); should-fix 7–10 not applied. Calibration note at the end.

## Step 1: knock-outs (any one → not in the top 5; list the row with the reason)
**Unit of scoring (fix 3):** K1, K2 and all scores apply to the row's A18 wedge (one signer + one product). If a problem has several wedges, score each as its own row.

| # | Knock-out | Test |
|---|---|---|
| K1 | **No buyer with proven spend** | No tender, contract, budget line, price list or observed paid purchase in the category. "Payer unclear" = out. **"Category" (fix 4)** = the wedge's signer type pays today for the same job, sourced [A]/[B]. A price list counts only with a named paying customer. A budget line counts only if it is in force today (not a bill or draft). |
| K2 | **No startup-accessible first sale in ≤12 months** | Every known buyer route needs turnover, references or certificates a new company lacks, and there is no direct-award-sized pilot, private buyer, or channel/subcontract route. Cite the selection criteria you checked. **Thresholds (fix 2):** see the direct-award table below; state which one applies per buyer, `[UNVERIFIED]` if unclear. Tender rows with thresholds "unknown" count as closed. **Evidence (fix 1):** a route counts only with a sourced example for this signer type: a company ≤5 years old with a named paying customer, a published direct-award/PoC call open to new companies, or a named channel/prime partner. A route that is only legally possible = **"K2 unproven"**: criteria 3 and 5 are tagged L (R2 cap, R3 "unproven"). |

**Direct-award limits per buyer type (no tender needed; supplies and services, net of VAT):**
| Buyer | Limit | Source |
|---|---|---|
| Bavarian state and municipal buyers | ≤ €100,000 | Art. 20 Abs. 1 BayWiVG ("ein Direktauftrag ist bis zu einer Wertgrenze von einschließlich 100 000 € ohne Umsatzsteuer zulässig"; text valid from 1 May 2026) [A] |
| Federal buyers | ≤ €50,000 since 1 Jul 2026 | Vergabebeschleunigungsgesetz (BGBl. 2026 I Nr. 137), IHK Schwerin [B]; in force 1 Jul 2026, BAS circular 1 Jun 2026 [A] |
| Statutory health and care insurers (all social-insurance bodies) | ≤ €50,000 since 1 Jul 2026 (before: €15,000 under a temporary rule) | § 22 Abs. 2 SVHV: "Direktauftrag … Der Auftraggeber soll zwischen den beauftragten Unternehmen wechseln" [A]; changed by Art. 14 Vergabebeschleunigungsgesetz (BAS circular 1 Jun 2026) [A]; €15,000 for 2026 per BAS circular 7 Jan 2026 [A] |
| Medizinische Dienste (15 MDs) | ≤ €50,000 (same as insurers) | § 280 Abs. 3 SGB V applies "die auf Grund des § 78 des Vierten Buches erlassenen Rechtsverordnungen entsprechend"; the SVHV is issued "Auf Grund des § 78 des Vierten Buches" [A]. *Inference:* § 22 Abs. 2 SVHV applies to MDs |
| Bavarian university hospitals (6, Anstalten under BayUniKlinG Art. 1) | **No statutory limit found; `[UNVERIFIED]`** | Art. 5 Abs. 1 BayUniKlinG: "die Vorschriften der Bayerischen Haushaltsordnung finden mit Ausnahme der Art. 88 bis 104 und 111 keine Anwendung" [A]. Art. 20 Abs. 4 BayWiVG extends the limits to legal persons "im Sinne des Art. 105 Abs. 2" BayHO [A]. Whether that reaches the university hospitals is unclear (inference: they are below-threshold rule-free by law, but bound by their own purchasing rules, which were not found) |
| Municipal hospital GmbHs (e.g. München Klinik), private and church hospitals | No statutory below-threshold limit found; `[UNVERIFIED]` | Not found in this session. Above the EU threshold (€216,000 for 2026–27, per `research/reviews/2026-11-07-redteam-scoring.md`, not re-opened) public-owned GmbHs can be bound by GWB procurement law |

## Step 2: scored criteria
Score each remaining problem 1–5 per criterion. Weighted total = Σ(score × weight). **Every score needs an evidence link and a confidence tag (Step 3).**

| # | Criterion | Weight | 5 = | 1 = |
|---|---|---|---|---|
| 1 | **Pain intensity** | 3 | Many independent online signals + [A]/[B] data showing cost/harm; people already pay or hack workarounds | Rare complaints, no workaround |
| 2 | **Market size & growth** | 2 | Large (≥€1bn addressable in EU) and growing (demographics, policy); state the buyer count | Niche, flat |
| 3 | **Willingness/ability to pay** | 3 | Named budget owner with proven spend that a startup can reach (paid pilot or contract in category); not a draft law or empty route (e.g. DiPA) | Unclear who pays |
| 4 | **Founder fit** | 2 | Matches `founder-brief.md` strengths (health innovation, AI/automation, German market) | Needs deep science/clinical skills the CEO lacks |
| 5 | **Achievability** | 2 | Paid pilot or first customer in ≤12 months with a small team and ≤€500k | Needs years of trials or >€5m before revenue |
| 6 | **Regulatory burden** | 1 | No/low MDR class, no clinical trial needed | Class IIb/III or drug approval |
| 7 | **Fundability (Munich/DE)** | 2 | Fits EXIST, Bavarian programs, EU grants, active health investors | No obvious funding route |
| 8 | **Competition gap** | 2 | No strong incumbent in DACH; clear wedge | Crowded, well-funded incumbents |
| 9 | **Future relevance** | 1 | Problem grows with structural trends (ageing, workforce shortage, digitization laws) | Shrinking |

Max = 90.

## Step 3: confidence rules
- **R1** Tag every score **H/M/L**. H = ≥1 [A]/[B] item directly on point and no counter-source. **M (fix 6)** = an [A]/[B] item about the same signer type in Germany, applied by inference. **L** = [C] only, snippet only, or inference without such an item. Criterion 5 is M/H only with a sourced comparable (a young company, same buyer type, paid within ≤12 months) or an open accessible procurement. Criterion 4 is M (source: `founder-brief.md`) unless the CEO has answered the founder-access question (H). No evidence at all = score 2, tag L.
- **R2** An **L** score counts as **at most 3** in the total. Unknown = L = no bonus.
- **R3** Criterion 3 or 5 at **L** → row marked **"unproven"**. It may enter the top 5 only with a named cheap test to run before Stage C.
- **R4** Sensitivity: re-rank with every L score −1. **(fix 5)** Apply −1 after the R2 cap (floor 1), ranking only K1/K2 survivors. Tier A = top 5 in base **and** top 7 in R4 **and** not "unproven"; Tier B = top 7 in either run, or "unproven"; Tier C = rest. Top 5 = tier A, filled from tier B by base total. Publish the sensitivity check next to the ranking.

## Output (`research/shortlist.md`)
Knock-out list with reasons; scoring table (score, confidence, evidence link per cell); tiers; sensitivity check; top 5 with reasoning.

---

## Calibration note (A20): four rows under v2 vs v3
Method: the cheap test proposed in the red team. Scores are mine and illustrative (inference); the A18 wedges below are provisional because A18 has not run. To isolate the effect of fixes 1–6, the raw 1–5 scores are held constant between v2 and v3; only K1/K2, tags, caps and the R4 order change. L06 uses the red team's own worked example. Weights: 3,2,3,2,2,1,2,2,1.

**Provisional wedges and the new evidence used:**
| Row | Wedge (signer + product) | K1 (v3) | K2 (v3) evidence found this session |
|---|---|---|---|
| L06 (S1) | Hospital medical director/CIO: LLM discharge-letter drafting | **Pass**: hospitals tender speech recognition and LLM discharge letters (Harzklinikum, 8 buyers) [A] (`pain-professionals.md`) | **Unproven.** All 8 tenders "No"/"Hard"; 3 "Unknown" now count as closed. No ≤5-year-old vendor with a named paying hospital found. Counter-signal: university hospitals build in-house: UKE "Argo" for discharge letters, made by its own subsidiary IDM (Aug 2024, [B], **>2 years old**); Leipzig "UKL-GPT" in its own data centre (Mar 2026) [B]. Bavarian university hospitals are outside BayHO purchasing rules (table above), so a pilot is legally possible, but no example exists |
| L07 (S3) | Hospital commercial director / medical controlling: MD-audit case review | **Pass**: Charité, Lausitz tenders [A]; DKI median €40k planned AI spend [B] | **Unproven on the letter of fix 1.** calliora (founded 2023) says it is live in "privaten, öffentlichen und kirchlichen Krankenhäusern in fünf Bundesländern", but names no customer (vendor claim, [B] munich-startup.de) |
| L21 (I5) | Kasse head of claims: AI § 302 billing-check module | **Pass**: BIG, BAHN-BKK, DAK billing-check tenders [A] | **Pass, weakly (channel clause).** Named channel: caery is "Partner im TechBoost Start-up- und Innovationsprogramm der Telekom", which offers start-ups "Zugang zu Vertriebs- und Partnernetzwerken" [B]. No caery customer is named and caery's founding year was not found. Direct tenders closed; DAK "unknown" = closed. New § 97a Abs. 5 GWB lets buyers oblige prime contractors to consider SMEs for subcontracts [A] (BAS, 1 Jun 2026) |
| L03 (P3) | Pflegekasse: digital carer course under § 45 SGB XI | **Pass (new)**: § 45 SGB XI is in force: Pflegekassen "haben … unentgeltlich Schulungskurse durchzuführen", "sollen auch digitale Pflegekurse anbieten" and may commission "geeignete andere Einrichtungen" [A]. Observed: Mobil Krankenkasse started a cooperation with Gesundheit von Morgen GmbH (PflegeBetreuer) for online carer courses (7 May 2026) [B] | **Unproven.** The vendor's founding year was not found; the release does not state a fee |

**Scores (raw score/tag; v3 changes in bold):**
| Row | Pain ×3 | Market ×2 | WTP ×3 | Fit ×2 | Achiev. ×2 | Reg ×1 | Fund ×2 | Comp ×2 | Future ×1 |
|---|---|---|---|---|---|---|---|---|---|
| L06 | 5 H | 5 M | 5 M → **L** | 4 M | 4 M → **L** | 3 H | 4 M | 3 L | 5 H |
| L07 | 5 H | 4 M | 5 M → **L** | 4 M | 4 M → **L** | 4 M | 4 M | 2 H | 5 H |
| L21 | 4 M | 4 M | 5 M | 4 M | 3 M → **L** (fix 6: no paid young comparable) | 5 M | 3 M | 3 M | 4 M |
| L03 | v2: out at K1 | **2 L** (no price) | **3 L** | **4 M** | **3 L** | **5 M** | **3 M** | **2 M** (curendo, PflegeBetreuer, Kassen's own courses) | **5 H** |

**Results:**
| Row | v2 base | v2 R4 | v2 status | v3 base | v3 R4 | v3 status |
|---|---|---|---|---|---|---|
| L06 | 78 | 76 | passes, proven | **70** | **63** | K2 unproven → "unproven" |
| L07 | 75 | 75 | passes, proven | **67** | **62** | K2 unproven → "unproven" |
| L21 | 70 | 70 | passes, proven | 70 | **68** | "unproven" (criterion 5 L) |
| L03 | out (K1) | — | knocked out | **59** | **52** | K2 unproven → "unproven" |

Math: L06 v3 = 78 − (5−3)×3 − (4−3)×2 = 70; R4 = 70 − 3 (WTP 3→2) − 2 (achiev. 3→2) − 2 (comp 3→2) = 63. L07 v3 = 75 − 6 − 2 = 67; R4 = 67 − 3 − 2 = 62. L21 v3 = 70 (achievability already 3, cap does not bind); R4 = 70 − 2 = 68. L03 v3 = 12+4+9+8+6+5+6+4+5 = 59; R4 = 59 − 2 (market 2→1) − 3 − 2 = 52.

**What changed (rank):** v2 order L06 > L07 > L21 (L03 out). v3 order L21 (70) = L06 (70) > L07 (67) > L03 (59); in the R4 run L21 (68) leads clearly. The fixes move rows. Calliora alone did not rescue L07, and L21 passes K2 only because a channel exists.

**Findings for B1 (inference):**
- **All four rows end "unproven", so none can be tier A.** Under fix 5 the top 5 is then filled from tier B by base total. Unless A18 finds young vendors with named paying customers, B1 will likely produce a shortlist with no tier-A row. That is the honest result, but the CEO should expect it.
- **Fix 1 is strict on age and naming.** voize (founded 2020, named customer BruderhausDiakonie, A18 notes) is now >5 years old; calliora is young but names no customer. Open question for the CEO: is "≤5 years old" measured today or at the time of the sale? This decides L05 (voize) and similar rows.
- **Fix 3 + 4 can revive "payer unclear" rows** by cutting a narrower wedge (L03 via § 45 SGB XI). This is intended, but B1 must not use it to pass rows on a different buyer than the one in the pain evidence.
- **The direct-award route is now buyer-specific.** For insurers and MDs it is €50,000, and the buyer "soll … wechseln", so a single direct award is a pilot, not a recurring contract (inference).

## Gaps / [UNVERIFIED]
- Whether Art. 20 Abs. 4 BayWiVG covers the six Bavarian university hospitals, and which purchasing rules municipal hospital GmbHs (e.g. München Klinik) follow below the EU threshold: `[UNVERIFIED]`.
- caery's and Gesundheit von Morgen GmbH's founding years and paying customers: not found. curendo's Kassen partners: Bosch BKK flyer seen as a search result only (PDF not retrievable).
- No ≤5-year-old vendor with a named paying hospital customer for LLM discharge letters found (2 searches, DE). Absence in search is not proof of absence.
- Calibration scores are illustrative; B1 will re-score with A18 data.

## Sources
- https://www.gesetze-bayern.de/Content/Document/BayZustWiG-20 — Art. 20 BayWiVG direct award ≤€100k; Abs. 4 extension; text valid from 1 May 2026 [A], accessed 2026-11-07
- https://www.gesetze-bayern.de/Content/Document/BayHO-105 — Art. 105 BayHO (state-supervised legal persons) [A], accessed 2026-11-07
- https://www.gesetze-bayern.de/Content/Document/BayUniKlinG/true — Art. 1 (six university hospitals as Anstalten), Art. 5 Abs. 1 (BayHO not applicable except Art. 88–104, 111) [A], accessed 2026-11-07
- https://www.gesetze-im-internet.de/svhv/__22.html — § 22 Abs. 2 SVHV direct award ≤€50,000 [A], accessed 2026-11-07
- https://www.gesetze-im-internet.de/svhv/BJNR031470977.html — SVHV issued under § 78 SGB IV (Eingangsformel); last changed by Art. 14 of the law of 12 May 2026 [A], accessed 2026-11-07
- https://www.gesetze-im-internet.de/sgb_5/__280.html — § 280 Abs. 3 SGB V: § 78 SGB IV regulations apply to the MD [A], accessed 2026-11-07
- https://www.gesetze-im-internet.de/sgb_4/__78.html — § 78 SGB IV scope (all social-insurance bodies except the BA) [A], accessed 2026-11-07
- https://www.bundesamtsozialesicherung.de/fileadmin/user_upload/20260603_Rundschreiben_Vergabebeschleunigungsgesetz_Ref_813.pdf — BAS circular 1 Jun 2026: law in force 1 Jul 2026; Art. 14 changes § 22 SVHV to €50,000; new § 97a Abs. 5 GWB [A], accessed 2026-11-07
- https://www.bundesamtsozialesicherung.de/fileadmin/redaktion/Vergabe/20260108_Vereinfachte_Vergabe.pdf — BAS circular 7 Jan 2026: €15,000 direct awards for federal social-insurance bodies until the new law [A], accessed 2026-11-07
- https://www.ihk.de/schwerin/recht/aktuelles/vergabebeschleunigungsgesetz-ab-01-07-2026-7060088 — federal direct awards ≤€50,000 net from 1 Jul 2026; not automatic for Länder/municipalities [B], accessed 2026-11-07
- https://vergabeblog.de/2026-07-03/seit-mittwoch-offiziell-gesetz-zur-beschleunigung-der-vergabe-oeffentlicher-auftraege-tritt-in-kraft/ — law in force, federal limit €50,000 [B], accessed 2026-11-07
- https://www.gesetze-im-internet.de/sgb_11/__45.html — § 45 SGB XI carer courses, digital courses, commissioning third parties [A], accessed 2026-11-07
- https://mobil-krankenkasse.de/unternehmen/presse/pressemeldungen/Pflegebetreuer.html — Mobil Krankenkasse × Gesundheit von Morgen GmbH online carer courses, 7 May 2026 [B], accessed 2026-11-07
- https://www.pflege.de/pflegende-angehoerige/pflegewissen/pflegeberatung/pflegekurse/ — curendo online course "Kostenfrei dank Übernahme durch Ihre Pflegekasse" (advertisement) [B], accessed 2026-11-07
- https://www.munich-startup.de/news/calliora-erhaelt-ueber-5-millionen-euro — calliora founded 2023; live in private, public and church hospitals in five states (company figures) [B], accessed 2026-11-07
- https://startupvalley.news/de/calliora-krankenhaeuser-ki-plattform/ — calliora interview, 6 Oct 2026; no named customer [B], accessed 2026-11-07
- https://www.telekom.com/de/newsroom/aktuelles/medieninformationen/2026/09/telekom-und-caery-revolutionieren-mit-ki-prozesse-fuer-kranken — caery as TechBoost partner, channel access; no named insurer customer [B], accessed 2026-11-07
- https://www.aerzteblatt.de/nachrichten/153726/Uniklinikum-Hamburg-Eppendorf-setzt-KI-Sprachmodell-fuer-Arztbriefe-ein — UKE in-house LLM for discharge letters, 22 Aug 2024 [B], accessed 2026-11-07
- https://www.aerzteblatt.de/news/universitatsklinikum-leipzig-setzt-auf-hausinterne-ki-plattform-70f5b9c9-0b19-490a-af84-671b4f4553f4 — Leipzig in-house "UKL-GPT", 9 Mar 2026 [B], accessed 2026-11-07
