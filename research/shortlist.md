# Shortlist: scoring of the 27-row long list and top 5
Task: B1 | Date: 2026-11-08 | Status: draft

Method: `research/scoring.md` as it stands on `main` (v3 + A25), applied as written. CEO-approved fixes 1–6 are in. S1–S4, the "≤5 years" measurement, the Sep 2027 clock and K1 "in force by then" are **not decided**. They are not applied here; each one is a caveat below, with its effect on the ranks. Unit of scoring = the A18 wedge (`research/longlist-scoring-fields.md`). The caveats from `research/reviews/2026-11-08-longlist-scoring-fields-A23-A25.md` and `research/reviews/2026-11-07-redteam-longlist-fields.md` are applied where the scoring text already requires them (G1/G2 = "same signer, same job"), and listed otherwise. A24/A26 desk tests were **not** run (CEO 2026-11-07); they appear as open checks.

## Findings
- **No row reaches tier A. All 10 K1/K2 survivors are "unproven".** No row has a sourced young comparable that was paid within ≤12 months, and no open procurement is accessible to a new company. So criterion 5 is L everywhere (R1), and R3 marks every row "unproven". As `scoring.md` predicted, the top 5 is then the base-total order.
- **Top 5 (as written, by base total):**
  1. **L01** employer eldercare benefit: 66 base / 62 R4
  2. **L07** hospital MD-audit case defence: 63 / 58
  3. **L06** LLM discharge letters: 62 / 55
  4. **L03** § 45 online carer course for Pflegekassen: 59 / 52
  5. **L13** AI phone assistant for practices: 59 / 54

  L29 (57 / 53) is 6th.
- **Slots 1–3 are robust; slots 4–5 are fragile.** S1 (rank by R4), S4 (one wedge per signer cluster: L01 and L03 are both C5), or re-scoring L03's pain on the course rather than lost work hours: each of these swaps L03 for L29 (MDR/IVDR post-market AI for device SMEs). If L06's K1 is read strictly (one KHZG tender, no award notice), L06 drops out and L29 enters. No other open question changes the top 5.
- **Only L01 combines an open buyer route, a young vendor with named customers and a €100m+ ceiling.** Employers ≥250 staff: 18,632 [A] × €5–20k (inference) ≈ €93–373m/yr. But the category has incumbents. pme Familienservice offers "Homecare-Eldercare" and says "Mehr als 1400 Unternehmen vertrauen auf unsere EAP-Lösungen" [B] ([pme](https://www.familienservice.de)). heycare (Munich, 2022) covers "elderly relatives" [B] ([Munich Startup](https://www.munich-startup.de/en/news/heycare-raises-4-million-euros-in-growth-capital)). Aon sells a "betriebliche Pflegelösung" with "Individuelles Pflege-Case Management" [B] ([Aon](https://www.aon.com/germany/gesundheit-vorsorge/betriebliche-pflegeloesung)). AOK PLUS trains in-company "Pflegelotsen" for free [B] ([AOK](https://www.aok.de/pp/pflege-vor-ort/aok-setzt-impulse/pflegelotsen/)).
- **17 of 27 rows fail K1** when K1 evidence must name the wedge's signer *and* job (fix 4; red team G1/G2). The scoring text already requires this, so it is applied, not a new rule. No row fails K2 outright, because every survivor has at least a legally possible route (private buyer or ≤€50k direct award).
- **New evidence opened in B1** (changes three K1 verdicts or criterion-8 scores):
  - § 106b SGB XI pays care facilities a monthly "TI-Pauschale" for TI equipment and running costs [A] ([§ 106b](https://www.gesetze-im-internet.de/sgb_11/__106b.html)). L05 K1 passes on this budget line, not on voize.
  - Practices pay for AI phone assistants. One group practice says "Die Kosten für den VoiceBot entsprechen dabei der Hälfte der ansonsten anfallenden Personalkosten". Another practice is cancelling: of ten callers, "konnten im Schnitt zwei" be handled [B] ([Ärzteblatt 7/2024](https://www.aerzteblatt.de/archiv/blickwinkel-wie-hilfreich-sind-telefonassistenten-067741f5-096d-4658-8eb0-34b7cc18b626)). L13 K1 passes.
  - Clariness has a "multi-year partnership with Boehringer Ingelheim Pharma & Co" in Germany [B] ([CTA](https://www.clinicaltrialsarena.com/contractors/clinical-trial-patient-recruitment/clariness/pressreleases/clariness-boehringer-ingelheim/)), and recruits in Germany for Servier's German subsidiary (Q1 2022) [B] ([CTA](https://www.clinicaltrialsarena.com/contractors/clinical-trial-patient-recruitment/clariness/pressreleases/phase-ii-study-servier-than/)). L26 K1 passes.
  - DORA applies to "Versicherungs- und Rückversicherungsunternehmen" and has applied since 17 Jan 2025 [A] ([Reg. (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R2554), Art. 2(1)(n), Art. 64). This confirms red-team G5 for L24.

## Readings used where the text is silent (my interpretation, flagged)
| Point | Reading applied | Why |
|---|---|---|
| "≤5 years old" (K2) | Vendor age **today** | Plain present tense; `scoring.md` calibration reads it this way ("voize … is now >5 years old"). CEO question open (caveat C1) |
| "named paying customer" | A customer named by the vendor counts ("laut Unternehmen", heycare), flagged; an unnamed claim does not (calliora, CrewLinQ) | Text says "named"; fact-check caveat 6 notes the weakness |
| K1 "pays today" | A tender, contract or named purchase by the wedge's signer type for the same job, dated 2024+, or a budget line in force. Vendor scale claims without a named buyer = K1 not shown | "Price list counts only with a named paying customer" |
| K2 example | A past published PoC call open to new companies counts as an example of the route (L23), even if closed | Text does not require it to be open |
| Criterion 5 "paid within ≤12 months" | First named paid customer within 12 months of the vendor's founding. None is shown for any row → L | R1 wording |
| Criterion 2 tag | M if buyer count [A]/[B] **and** a sourced price anchor (tender value, price list, DKI budget); else L | A18: unanchored ACVs "should tag them L" |
| Criterion 4 | All M (founder-access question unanswered). 4 = AI/automation workflow, gap = CTO; 3 = core also needs a domain specialist (clinician, coder, care-IT); 2 = core is regulatory/physician expertise | `founder-brief.md` "Gaps" |
| 12-month clock | From today (text silent) | CEO question open (caveat C6) |
| Top-5 fill | Tier B by **base** total | R4 as written (S1 not approved) |

## Step 1: knock-outs (17 rows)
| # | Wedge (A18) | Out on | Reason |
|---|---|---|---|
| L02 | None (care capacity search) | K1 | No payer for search; supply is the constraint ([longlist](longlist.md) L02) |
| L04 | Compliance software for live-in agencies | K1 | No purchase of software observed; money buys labour |
| L08 | Transition medication-list niche → hospital | K1 | No purchase of this product. Discharge-platform buys (Helios, Köln→Recare) are a different product and used one-off KHZG money (G1). Status quo also misses the ePA medication list (snippet only, red team) |
| L09 | Shift-cover pool app → care operator | K1 | Rostering purchases are a different job (G2). CrewLinQ ">100 Pflegeeinrichtungen" names no customer [B] |
| L11 | Recognition case management → employer | K1 | No purchase observed; fees `[UNVERIFIED]`. **Not searched** (A26 test deferred): may wrongly fail (red team) |
| L12 | AI pre-fill of payer forms → practices | K1 | "Practice opex, no observed purchase" (G2) |
| L14 | None | K1 | TSVG money is physician fees (§ 87a Abs. 3 SGB V [A]) |
| L15 | None | K1 | Not product-solvable; no buyer |
| L16 | Trial-access/orientation service → PKV | K1 | Debeka × iuvando is a cooperation with no fee stated [B]; no budget line. iuvando (2019) also fails the age test |
| L17 | Lung-LDCT eligibility tool → GP/radiology | K1 | No purchase observed; the benefit pays for the exam, not outreach |
| L18 | Pharma patient finding | K1 | Spend `[UNVERIFIED]` |
| L20 | Shortage assistant → pharmacies | K1 | "Pharmacy opex, no purchase" (G2); 3 searches found no paid tool (A18). A26 test deferred |
| L21 | Classification module → BPO | K1 | Evidence is Kassen buying BPO services, not a BPO buying a tool (G1). As a Kasse wedge, K1 passes but every tender needs ISO 27001 + references |
| L24 | GOÄ-2028 invoice check → PKV | K1 | No observed purchase (G2). DORA third-party rules apply to insurers [A] (G5). GOÄ is planned, not in force |
| L25 | Local health office | K1 | Budget ended in 2026 (BT-Drs. 21/8237 [A]) |
| L27 | Site start-up pack → CRO | K1 | Adjacent spend only |
| L28 | AI PICO scoping → biotech | K1 | Consultancies sell JCA work, but no named buyer is in the repo ("vendor market"). Founder fit 2 in any case |

K2 knock-outs: none. L22 is closest: every tender needs turnover, references or a consortium, but a ≤€50k MD direct award is legally possible, so "unproven".

## Step 2–3: scoring table (10 survivors)
Format: raw score, confidence. **Bold** = an L score counted at 3 under R2. Weights 3/2/3/2/2/1/2/2/1. Evidence keys are listed under the table.

| # | Wedge → first buyer | K1 / K2 | Pain ×3 | Market ×2 (buyer count) | WTP ×3 | Fit ×2 | Achiev. ×2 | Reg ×1 | Fund ×2 | Comp ×2 | Future ×1 | Base | R4 | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| L01 | Eldercare navigator as employee benefit → employer ≥250 staff | Pass [e1–e4] / **Pass** (heycare 2022, named employers, vendor claim) [e2] | 4 M [e5][e6] | **4 L** (18,632 [A]; ACV inference) [e7] | 4 M [e2][e3][e4] | 4 M | **4 L** | 5 M | 4 M (heycare €4m round) [e2] | 2 H (pme, heycare, Aon, AOK) [e1–e4] | 5 H [e8] | **66** | **62** | unproven (crit. 5) |
| L07 | MD-audit case defence → private hospital <300 beds | Pass [e9][e10] / unproven (calliora unnamed) [e11] | 5 H [e12] | 3 M (1,603 IKs × DKI €40k ≈ €64m, DE-specific) [e10] | **4 L** | 3 M (coding expert needed) | **3 L** | 4 M | 4 M (calliora €5.3m) [e11] | 2 H (Tiplu/LOGEX, ID Berlin, Dedalus, calliora) [e13] | 5 H [e12] | **63** | **58** | unproven |
| L06 | LLM discharge letters → hospital | Pass, weak (one KHZG tender, no award) [e14] / unproven | 5 H [e15][e16] | **4 L** (1,807 hospitals [A]; ACV inference) [e17] | **4 L** | 3 M (clinical content + KIS integration) | **3 L** | 3 H (CDSS → MDR IIa+) [e15] | 4 M (Tandem, Telekom) [e18] | 2 M (Tandem, Microsoft/Nuance, in-house UKE/Leipzig) [e18][e19] | 5 H | **62** | **55** | unproven |
| L03 | § 45 online carer course → Pflegekasse | Pass on budget line [e20] / unproven (vendor age unknown) [e21] | 4 M [e6] | **2 L** (92 Kassen × ≤€50k) [e22] | **3 L** | 4 M | **3 L** | 5 M | 3 M | 2 M (curendo, PflegeBetreuer, in-house) [e21][e23] | 5 H | **59** | **52** | unproven |
| L13 | AI phone assistant → practices | Pass (2 practices pay, 2024) [e24] / unproven | 4 M [e24][e25] | 4 M (~103k practices × €9–229/month) [e25][e26] | **4 L** | 4 M | **4 L** | 4 M | 3 M (Doctolib bought aaron.ai) [e27] | 1 H (10 vendors incl. Doctolib) [e25] | 4 M | **59** | **54** | unproven |
| L29 | AI PMS/literature → device SME | Pass (Flinn × Hartmann) [e28] / **Pass** (Flinn 2022) [e29] | 4 M [e30] | **3 L** (1,480 firms; ACV inference) [e31] | 4 M [e28] | 2 M (RA core) | **2 L** | 4 M | 4 M (Flinn $20m) [e28] | 2 M (Flinn "leading", self-description) | 3 M (MDR revision may shrink pain) | 57 | 53 | unproven |
| L23 | AI care-assessment drafting → one MD | Pass (MD RLP PoC tender) [e32] / Pass on a past call (closed 5 Sep 2025, no winner) [e32] | 4 H [e33] | 1 M (15 MDs × ≤€50k ≈ €0.75m) | 3 M | 3 M | **3 L** (no open call) | 4 M | 3 M | **3 L** | 4 H | 55 | 51 | unproven |
| L26 | DE recruitment service + software → sponsor | Pass (BI, Servier DE) [e34] / unproven | 3 M (counter-source: sites rank patient ID low) [e35] | **4 L** (668 new commercial EU trials with DE sites [A]; ACV inference) | **4 L** | 3 M | 2 L | 4 M | 3 M | 2 H (Clariness+SubjectWell, TriNetX, CROs) [e36] | 4 H (5 % rule 2027) [e35] | 52 | 45 | unproven |
| L05 | TI/KIM onboarding service → small care operator | Pass on § 106b [e37] / unproven | 3 M (50 % with activated TI card) [e38] | **2 L** (~32k facilities; ACV inference) [e39] | **3 L** | 3 M | **4 L** | 5 M | 2 M (service business) | 2 L (suite vendors, snippet only) | 2 M (one-off wave) | 49 | 40 | unproven |
| L22 | Review services / consortium → MD | Pass [e40] / unproven (consortium only; MD-IT bids 2 Dec 2026) | 4 H [e40] | 3 M (15 MDs; €88m framework) [e40] | **4 L** | 2 M (physician review firm) | 1 L | 4 M | 2 M | 2 H (QuantCo, review firms) [e40] | 4 H | 49 | 46 | unproven; conflicts with L07 |

Math, two examples. L01 base = 4×3 + 3×2 (L cap) + 4×3 + 4×2 + 3×2 (L cap) + 5 + 4×2 + 2×2 + 5 = 12+6+12+8+6+5+8+4+5 = **66**; R4 = 66 − 2 (market 3→2) − 2 (achievability 3→2) = **62**. L03 = 12+4+9+8+6+5+6+4+5 = 59; R4 = 59 − 2 − 3 − 2 = 52 (same as the `scoring.md` calibration). All totals were computed by script and checked by hand.

**Changes against the `scoring.md` calibration (illustrative scores, A20):** L06 70 → 62 (market tagged L, no price anchor; fit 3; competition 2 M after Tandem). L07 67 → 63 (market 3: the audit regime is German only; fit 3: needs a coding expert). L21 is out at K1 (BPO wedge, G1). L03 is unchanged at 59.

## Tiers and sensitivity (R4)
| Rank | Base run | R4 run (every L −1) | Tier |
|---|---|---|---|
| 1 | L01 66 | L01 62 | B (unproven) |
| 2 | L07 63 | L07 58 | B |
| 3 | L06 62 | L06 55 | B |
| 4 | L03 59 / L13 59 (tie) | L13 54 | B |
| 5 | (tie above) | **L29 53** | B |
| 6 | L29 57 | L03 52 | B |
| 7 | L23 55 | L23 51 | B |
| 8–10 | L26 52, L05 49, L22 49 | L22 46, L26 45, L05 40 | B (unproven ⇒ tier B by definition) |

Tier A: none. Tier C: none (R4: "Tier B = … or unproven"). Under R4 as written, the top 5 is filled by base total, so L03 and L13 (both 59) take slots 4–5.

## Caveats for the CEO: open questions and their effect on ranks
| # | Open question (not decided) | Applied as written | If decided the other way | Rank effect |
|---|---|---|---|---|
| C1 | "≤5 years": today vs at the time of the sale | Today | At the sale: voize (2020; Caritas Jan 2022) passes. MIA (2019) would pass for L07 **if** it is the UK Frankfurt winner (name match `[UNVERIFIED]`) | **None in the top 5** for A18 wedges. If MIA is confirmed: L07 WTP 4 M → 66/64, tied 1st with L01. Voice-documentation wedge of L05 (not an A18 wedge, voize's product): 64 today, 67 at the sale. It would rank 2nd or 1st, with competition 1 (see C5) |
| C2 | S1: fill from tier B by R4 total | Base total | R4 order | **L03 out, L29 in** (L13 4th, L29 5th) |
| C3 | S2: K2 example vendor sits in criterion 8, leader → ≤2 | Not applied | heycare (L01) and Flinn (L29) are already at 2 | None |
| C4 | S3: channel must be open to new entrants | Not applied | No survivor passes K2 via a channel | None |
| C5 | S4: wedges fixed in A18, ≤1 wedge per signer cluster | Not applied (A18 wedges used anyway) | L01 and L03 are both C5, so L03 drops | **L03 out, L29 in.** S4 also blocks the L05 voice wedge (C1) |
| C6 | 12-month clock starts Sep 2027 (S6) | From today | Criterion 5 is already L everywhere. L07's trigger (quotas 1 Jan 2027) is 9 months before the founder starts, so incumbents get a head start (G4). *Inference:* L07 competition 2 → 1 (−2 → 61) | None (L07 stays 2nd–3rd) |
| C7 | K1 "in force by then" (start of the clock) | In force today | Rows whose K1 failed only because of a bill: none among the A18 wedges. L24 fails on "no observed purchase", L25 on "budget ended". L05 already passes on § 106b | None |

Other caveats from the reviews (no CEO decision needed):
- **L06 K1 rests on one tender.** Harzklinikum (KHZG project "4.01"), request deadline 25 Aug 2025. TED shows only the contract notice, no award, as of 8 Nov 2026 [A] (TED 492877-2025, re-queried). A18 labelled the budget "adjacent" (red team G1 → K1 fail); A23 relabelled it "tendered". If K1 fails, **L06 out, L29 in**.
- **L01 K2 rests on a vendor claim** ("According to the company", fact-check caveat 6). If it is not accepted, L01 = 63 / 56: still 1st–2nd.
- **L03 pain:** the red team says not to score a course on "45 % cut hours". With pain 3, L03 = 56: **out, L29 in**.
- **L13 K1** rests on two practices in one 2024 article, and one of them is cancelling.
- **Headline counts:** five wedges, not seven, have a named customer; only heycare and Flinn pass the age test today (fact-check caveat 1). The "leader" labels for Recare and Flinn are inference or self-description (caveat 2). Flinn's "$20m" is not labelled "Series A" (caveat 3).
- **L23:** only the MD RLP procedure (closed, result notice without a winner) is care-assessment evidence. The open MD Nordrhein tender is malpractice review (caveats 4–5).
- **Ceiling (G3):** buyer count × A18 ACV guess, 100 % share, my arithmetic, all L:
  - L01: €93–373m/yr
  - L13: €124–247m/yr (commodity)
  - L06: €54–180m/yr
  - L07: €36–72m/yr (DKI pool ~€64m)
  - L29: €15–44m/yr
  - L03: €4.6m (pilot ceiling)
- **Founder access** (criterion 4) is unanswered, so criterion 4 is M on every row and separates little (red team S8).
- **L07 vs L22** are opposite sides of one market. Only L07 is in the top 5.

## Top 5: reasoning, sketch, open checks
**1. L01: Eldercare navigator as an employee benefit (66 / 62)**
- **Why:** It is the only row where a private buyer is reachable without procurement, a young vendor shows named customers, and the ceiling is €100m+. Pain is documented: 3 % use statutory counselling [A]; 46.9 % of employed carers are "hoch belastet" [B]. The weak points are incumbents (pme: 1,400+ firms; heycare; Aon; free AOK Pflegelotsen) and no observed stand-alone eldercare price.
- **Sketch:** A German-language AI + human care navigator ("Pflegefall in 48 h organised") sold to HR at firms with ≥250 staff. It helps employees with a care grade application, relief budget, respite care and finding services, and reports anonymised usage to HR. The first pilot is a Munich employer with a works council. Later, it plugs into benefit platforms and adds the § 45 Pflegekasse course (L03) as a second payer. The edge to test is depth on statutory benefits plus AI case handling, against pme's broad EAP.
- **Open checks:**
  - (A26) One dated, named employer contract with a price for eldercare (pme, heycare, Aon or other).
  - Do employers buy eldercare only inside bundled EAPs?
  - heycare's first-sale date.
  - CEO 10-minute check: do you know one HR/benefits lead at a ≥250-staff firm?

**2. L07: MD-audit case defence for private hospitals (63 / 58)**
- **Why:** It has the strongest pain and job budget. €1.58bn of revenue is at risk [A], quotas reach up to 40 % from 1 Jan 2027 [A], and the DKI median is €40k of planned spend [B]. Private hospitals buy without tenders. Against it: crowded (Tiplu "MBEG-Assistent" in ~30 hospitals, calliora €5.3m in Munich), it needs a coding/medical-controlling co-founder, and the trigger precedes the founder's start (G4).
- **Sketch:** An AI tool that checks each MD-audited case file and drafts the objection or justification (the MBEG reply). It is sold to independent private hospitals <300 beds at ~€20–40k/yr, with a medical-controlling co-founder. The angle is medical-necessity and length-of-stay arguments (68 % of audit reasons [A]), not coding.
- **Open checks:**
  - (A26) Count independent private hospitals with ≥1 MD audit per quarter (GKV-SV XLSX).
  - A named calliora hospital (none found so far).
  - Is the UK Frankfurt winner MIA (2019)?
  - A17 data after 1 Dec 2026 (Q3 statistics, Bundesrat 20 Nov).

**3. L06: LLM discharge-letter drafting (62 / 55)**
- **Why:** Very high documented pain: 93.1 min/day measured [A], 3 h/day self-reported [B]. But K1 rests on one KHZG tender, Tandem Health (>10,000 facilities, Telekom-backed) and the KIS vendors hold the channel, and university hospitals build in-house.
- **Sketch:** Letter drafting from structured KIS data for small private hospitals, via a KIS-vendor partnership.
- **Open checks:**
  - Have private chains (Helios, Asklepios, Sana, Schön) bought LLM letters from a ≤5-year-old firm?
  - Harzklinikum award (winner).
  - Private-hospital purchasing rules `[UNVERIFIED]`.
  - MDR status of drafting vs CDSS.

**4. L03: § 45 SGB XI online carer course for Pflegekassen (59 / 52)**
- **Why:** The budget line is in force and Kassen already commission online courses (Mobil Krankenkasse, ZF BKK). But the ceiling is tiny (92 × ≤€50k; "soll … wechseln"), and the slot is fragile (C2, C5).
- **Sketch:** A personalised online course for family carers, commissioned by BKK-size Pflegekassen. Best as the second payer of the L01 venture, not a company on its own.
- **Open checks:**
  - (A26) A price or contract value for a Kassen-funded online course.
  - Gesundheit von Morgen's founding year.
  - Tender path after the pilot.

**5. L13: AI phone assistant for practices (59 / 54)**
- **Why:** Practices pay (half of staff cost in one practice [B]), there are ~103k practices, it is self-serve, and AI agents are the founder's daily work. But it is a commodity: 10 vendors at €9–229/month incl. Doctolib. Churn is visible: one practice cancelled after 2 of 10 calls were handled.
- **Sketch:** Specialist-niche voice agent (e.g. one specialty with a PVS integration) as a cheap founder-fit test, not a standalone venture case.
- **Open checks:**
  - Funding of the top 3 vendors (red team).
  - One young vendor with a named practice.
  - Which PVS systems offer booking interfaces?

**Runner-up L29 (57 / 53):** It enters under S1, S4 or a strict L06 K1 reading. Pass K1/K2 cleanly (Flinn × Hartmann). Weak founder fit (RA expertise core); Flinn ($20m) holds the wedge.

**Open checks not tied to the top 5** (A24/A26, deferred): AMNOG procedures per year (L26), care-suite AI documentation (L05), nursing recognitions by country (L11), the L20 pharmacy test, the L11 per-hire fee test.

## Recommendation (inference)
Deep-dive **L01 (with L03 as the second payer, one "carer support" brief)** and **L07**. L01 is the only row that fits "big but achievable" for a part-time founder with €10k. L07 has the strongest proven budget, but needs a domain co-founder and has a Munich competitor. Optional third: L13 as a fast, cheap founder-fit test, not as a venture case. Before picking, the founder-access check (10 min) would turn criterion 4 into a real separator.

## Gaps / [UNVERIFIED]
- A24/A26 desk tests not run (CEO). Results could flip L11 and L20 K1, and L07 K2.
- No sourced price for any wedge except L13 (price lists), L07 (DKI budget) and the €50k caps. Market scores are L where unanchored.
- MIA = UK Frankfurt winner, Gesundheit von Morgen and Recare founding years, private/municipal-GmbH hospital purchasing rules: `[UNVERIFIED]`.
- Snippet only (not used as fact): Hallesche "FEELcare" employer care plan (PDF opened, but dated 08/21 and >3 years old, so used only as an incumbent pointer); ePA medication list for L08; Insiders Technologies for L21/L24; employer-eldercare market overviews (2 searches, no market size found).
- [C] layer thin (Reddit blocked). Pain scores rest on [A]/[B] surveys.

## Sources
Opened in B1 (accessed 2026-11-08):
- https://www.gesetze-im-internet.de/sgb_11/__106b.html — TI-Pauschale for care facilities (equipment and running costs) [A] [e37]
- https://www.familienservice.de — pme: "Homecare-Eldercare", ">1400 Unternehmen" on EAP [B] [e1]
- https://www.munich-startup.de/en/news/heycare-raises-4-million-euros-in-growth-capital — heycare: care for children, elderly relatives; named customers "according to the company"; €4m [B] [e2]
- https://www.aon.com/germany/gesundheit-vorsorge/betriebliche-pflegeloesung — Aon employer care solution with case management [B] [e3]
- https://www.aok.de/pp/pflege-vor-ort/aok-setzt-impulse/pflegelotsen/ — AOK PLUS free in-company Pflegelotsen [B] [e4]
- https://hallesche.de/-/media/dokumente/hallesche/vbh/lvm/infoblatt-feelcare-ueberblick-vbh35-lvm.pdf — Hallesche FEELcare employer care plan (dated 08/21, >3 years) [B]
- https://www.aerzteblatt.de/archiv/blickwinkel-wie-hilfreich-sind-telefonassistenten-067741f5-096d-4658-8eb0-34b7cc18b626 — two practices on paid AI phone assistants, issue 7/2024 [B] [e24]
- https://www.clinicaltrialsarena.com/contractors/clinical-trial-patient-recruitment/clariness/pressreleases/clariness-boehringer-ingelheim/ — Clariness × Boehringer Ingelheim, multi-year, Germany [B] [e34]
- https://www.clinicaltrialsarena.com/contractors/clinical-trial-patient-recruitment/clariness/pressreleases/phase-ii-study-servier-than/ — Clariness × Servier DE subsidiary, Q1 2022 [B] [e34]
- https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R2554 — DORA Art. 2(1)(n) insurers; applies from 17 Jan 2025 [A]
- https://api.ted.europa.eu/v3/notices/search — TED 492877-2025 (Harzklinikum LLM discharge letters, request deadline 25 Aug 2025; no award notice under procedure 7e725667-…) [A] [e14]
- WebSearch, snippets only: employer eldercare providers (personalwirtschaft, haufe, business-on); AI phone vendor pages (fonio, zeeg, famulor); ki-syndikat urgency caveat.

Carried over (not re-opened in B1; see the linked files):
- [e5] https://www.gkv-spitzenverband.de/media/dokumente/pflegeversicherung/beratung_und_betreuung/pflegeberatung/2026-06_Bericht_des_GKV-Spitzenverbandes_7a_Absatz_9_SGB_XI.pdf — 3 % use counselling [A]
- [e6] https://www.wido.de/fileadmin/user_upload/20260511_WIdO-PM_WIdOmonitor_Pflegende_Angehoerige.pdf — 46.9 % "hoch belastet", 45.2 % cut hours [B]
- [e7] https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/Unternehmensregister/Tabellen/unternehmen-beschaeftigtengroessenklassen-wz08.html — 18,632 units ≥250 staff [A]
- [e8] `research/trends.md` — care demand projections (Destatis) [A]
- [e9] `research/hospital-billing-audits.md` — UK Frankfurt €181,800 award, Charité framework (TED) [A]
- [e10] https://www.dkgev.de/fileadmin/Mediapool/1_DKG/1.7_Presse/2026-10-06__Blitzumfrage_MD-Pr%C3%BCfungen.pdf — DKI flash survey (€40k median planned spend) [B]
- [e11] https://www.munich-startup.de/news/calliora-erhaelt-ueber-5-millionen-euro — calliora 2023, no named hospital [B]
- [e12] https://www.gkv-spitzenverband.de/media/dokumente/krankenversicherung_1/krankenhaeuser/abrechnung/mdk_pruefstatistiken/jahr_2025/Statistikdaten_nach__17c_Abs._6_Satz_1_-_2025.xlsx and https://www.buzer.de/gesetz/17632/a340690.htm — 2025 audits, 2027 quotas [A]
- [e13] https://tiplu.de/generative-ki-datenbasis/ — Tiplu MBEG-Assistent in ~30 hospitals [B]
- [e15] https://www.dki.de/fileadmin//user_upload/2025-09_Buerokratiebelastung_im_Krankenhaus_-_final.pdf — 3 h/day [B]; `research/pain-professionals.md` S1 (MDR IIa+ for CDSS [A])
- [e16] https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=EXT_ID:38977000%20AND%20SRC:MED&format=json&resultType=core — 93.1 min/day [A]
- [e17] https://www.destatis.de/DE/Presse/Pressemitteilungen/2026/10/PD26_376_231.html — 1,807 hospitals [A]
- [e18] https://www.telekom.com/en/newsroom/latest-updates/media-information/2026/10/telekom-invests-in-tandem-health — Tandem >10,000 facilities incl. DE [B]
- [e19] https://www.aerzteblatt.de/nachrichten/153726/Uniklinikum-Hamburg-Eppendorf-setzt-KI-Sprachmodell-fuer-Arztbriefe-ein — UKE in-house [B]
- [e20] https://www.gesetze-im-internet.de/sgb_11/__45.html — § 45 SGB XI [A]
- [e21] https://mobil-krankenkasse.de/unternehmen/presse/pressemeldungen/Pflegebetreuer.html; https://www.zfbkk.de/en/news/details/online-nursing-courses — Kassen × Gesundheit von Morgen [B]
- [e22] https://www.gesetze-im-internet.de/svhv/__22.html; https://www.gkv-spitzenverband.de/service/krankenkassenliste/krankenkassen.jsp — ≤€50k direct award; 92 Kassen [A]
- [e23] https://www.pflege.de/pflegende-angehoerige/pflegewissen/pflegeberatung/pflegekurse/ — curendo [B]
- [e25] https://medizinio.de/digitalisierung/telefonassistent-arztpraxis — 10 vendors, €9–229/month [B]
- [e26] https://www.hartmannbund.de/wp-content/uploads/2025/11/2025-HV_Praxen-bleiben-unverzichtbare-Saeule-der-Versorgung.pdf — ~98,000 practices + ~4,900 MVZ [B]
- [e27] https://www.aerzteblatt.de/nachrichten/151593/Doctolib-uebernimmt-Telefonassistenten — Doctolib buys aaron.ai [B]
- [e28] https://www.lisavienna.at/news/detail/flinn-receives-20-million-to-automate-the-product-lifecycle-in-medtech-and-pharma-with-ai/ — Flinn customers, $20m [B]
- [e29] https://tech.eu/2022/12/20/n26/ — Flinn formed 2022 [B]
- [e30] `research/pain-industry.md` I4 — MDR certification 19.5/21.8 months, 53 % cut R&D [B]
- [e31] https://www.bvmed.de/download/positionspapier-medtech-kmu — 1,480 firms [B]
- [e32] `research/longlist.md` L23 — MD RLP PoC (TED 343840-2025 / 483916-2025 / 543912-2025) [A]
- [e33] `research/pain-industry.md` I6 — >3m care assessments 2025 [A]
- [e35] `research/trial-recruitment-de.md` — vfa barometers (2.9 %, site hurdles) [B]; § 130a Abs. 1c 5 % rule [A]
- [e36] `research/pain-industry.md` I1 — Clariness+SubjectWell merger, TriNetX/Clinerion [B]
- [e38] https://pardok.parlament-berlin.de/starweb/adis/citat/VT/19/SchrAnfr/S19-25964.pdf — 50 % of care facilities with activated TI card [A]
- [e39] https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Gesundheit/Pflege/Tabellen/pflegeeinrichtungen-deutschland.html — 16,505 + 15,549 facilities [A]
- [e40] `research/payer-processing.md` §3–4 and `research/longlist-scoring-fields.md` — MD-IT €88m framework, MD Niedersachsen €2m, TK × QuantCo [A]
