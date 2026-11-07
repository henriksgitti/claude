# Red team: research/scoring.md (v3, A20)
Date: 2026-11-07 | Mode: RED TEAM (reasoning, not sources) | Verdict: **needs work. Small edits: S1–S4 are each one line for the CEO; the rest are B1 instructions.** Fixes 1–6 were applied correctly. The CEO's choices (9 criteria and weights kept; K3–K6, minimum bars and fixes 7–10 not applied) are not re-argued. The issues below are new: they come from the v3 text and its calibration result, and are not covered by earlier reviews.

## Fatal or near-fatal objections
**S1. When no row reaches tier A, the confidence rules stop affecting the order. The ranking falls back to the additive total the CEO wanted to avoid.**
- R4: "Top 5 = tier A, filled from tier B **by base total**."
- The calibration note predicts "All four rows end 'unproven', so none can be tier A … B1 will likely produce a shortlist with no tier-A row."
- In that case the top 5 is just the base-total order, and the R4 run (the sensitivity test) has no effect on it. Calibration example: base L06 = L21 = 70, but R4 gives L21 68 vs L06 63 and L07 62. By base total, L06 ties for first. By R4 it is clearly behind.
- **Fix (one word):** "filled from tier B by **R4** total (ties: fewer L tags first)". This keeps the CEO's design and lets the confidence layer work in the case the calibration expects.

**S2. K2's evidence rule selects crowded categories, and nothing links it to criterion 8.**
- Under fix 1, a route counts only if a young company already sells to this signer type. That evidence is also a competitor.
- The best K2 evidence found so far is the market leader in its row: voize for L05 ($50m, 1,100 facilities), calliora for L07 ($6m, Munich), Recare for L08.
- Criterion 8 (weight 2) can at most give back 8 points. So the rows with the cleanest access proof are the most contested, and empty niches are always "unproven".
- **Fix (one line, display only):** "The K2 example vendor must appear in the criterion 8 evidence; if it is the category leader (most named customers or most funding found), criterion 8 ≤ 2."

**S3. The channel clause can be met with another company's channel.**
- K2 accepts "a named channel/prime partner".
- L21 passes K2 in the calibration only because "caery is 'Partner im TechBoost …' (Telekom)". caery has no named customer and an unknown founding year.
- That proves Telekom will resell *caery*. It does not prove a channel is open to a new founder.
- **Fix:** "A channel counts only if it is open to new entrants (a published partner/accelerator intake or a prime's published subcontractor call) or has signed with ≥2 young vendors."

## Other issues B1 will trip over
| # | Issue (quote) | Why it matters | Fix / B1 instruction |
|---|---|---|---|
| S4 | Fix 3: "If a problem has several wedges, score each as its own row" | B1 can (a) choose wedges after seeing the scores, and (b) fill the top 5 with variants of one buyer bet. The long list has only ~10 signer clusters (`2026-11-07-redteam-longlist.md` F3). The calibration already warns about passing rows "on a different buyer than the one in the pain evidence" | CEO line: "Wedges are fixed in A18 before scoring; at most one wedge per signer cluster in the top 5 (show the runner-up wedge as a note)." B1: score criterion 1 on the **wedge signer's** pain (this follows from fix 3, "all scores apply to the row's A18 wedge") |
| S5 | Criterion 5: "Paid pilot or first customer in ≤12 months with a small team and **≤€500k**" | `founder-brief.md`: own money €10,000; "Ideas must reach a grant, pre-seed or paying pilot before needing more." €500k is a pre-seed round the founder does not have, and EXIST is closed while he is employed. ISO 27001 is required in every insurer tender (`pain-industry.md`). Under the anchor, rows that need certification before the first pilot can still score 4 | B1 instruction, no method change: for a 4–5, show the pilot path costs ≤€10k plus money accessible while part-time (e.g. BayStartUP prizes), or name the funding step that comes first and tag it L |
| S6 | K2 and criterion 5: "≤12 months", start date not stated | The founder is part-time until **Sep 2027**. Measured from today, the clock ends before he is full-time. Triggers starting 1 Jan 2027 (audit quotas) will be partly absorbed by incumbents by then | CEO line: "12 months count from Sep 2027; judge 'why now' triggers against Sep 2027–Sep 2028." |
| S7 | Fix 1: "a company ≤5 years old with a named paying customer" | Age alone lets incumbent offshoots count. Health Data Exchange GmbH (Tiplu + HERR DER LAGE joint venture, 2023) won the Charité coding framework (`hospital-billing-audits.md`), but it is a joint venture with an incumbent. IDM is a UKE subsidiary | Add "**independent** (not a subsidiary/JV of an incumbent or of the buyer)". See the CEO question below |
| S8 | Criterion 4 is "M (source: `founder-brief.md`) unless the CEO has answered the founder-access question (H)" | No row has founder access in the brief, so every row gets about 4 M. The criterion adds 8 points to everyone and separates nothing. Not a method flaw: the input is missing | CEO 10-minute founder-access check (see the long-list review, test 1) before B1 |
| S9 | Criterion 2: "state the buyer count" | Some rows have tiny buyer counts: 15 MDs (L23), 39 PKV full members (L24), ~58 JCAs (L28). A "≥€1bn EU" reading could still give them 3–4 | B1 instruction only (fix 8 was not approved, so not re-argued): print the buyer count next to the market score |
| S10 | Direct-award table: insurers/MD ≤€50k, "soll … wechseln" | The first sale is possible, but repeat business with the same Kasse is not. The second contract needs a tender with references and ISO certificates. Achievability of the *first* sale ≠ path to recurring revenue | B1 note per insurer/MD row: "after the pilot: tender path = …" |

## View on the two open CEO questions (progress.md)
**Q1. How is "≤5 years old" measured?** The rule exists to prove that a company **without a track record** can win this signer type. So measure it at the time of the vendor's **earliest named paid sale** to that signer type, not today. Add two guards:
- The sale is dated **2021 or later**. Procurement rules and buyer habits changed in 2026 (new thresholds), so older sales say little.
- The vendor is independent (S7).

Effect:
- voize counts if its earliest named care-operator customer is dated 2021+, which it likely is (founded 2020). The BruderhausDiakonie rollout of Dec 2025 is not its first sale.
- If voize counts, S2 applies: voize is also the category leader in L05, so criterion 8 ≤ 2.

This matches the researcher's recommendation in `progress.md` ("measure at the time of the sale"), with the two guards added.

**Q2. Do unnamed-customer vendor claims count?** Not on their own. A claim like calliora's ("private, public and church hospitals in five states"; the press note itself says "not independently verified") cannot be falsified. But accept an unnamed claim if **one independent source** confirms one customer:
- an award notice;
- the customer's own press release or annual report;
- a conference talk by customer staff;
- a case study naming the organisation.

Until then the row stays "K2 unproven". That is not a knock-out, so a strict rule costs little.

Desk test: search for "calliora" on hospital and conference sites. One named hospital settles L07.

## Cheapest tests of these fixes (researcher, ≤1 run, desk only)
- Re-run the four calibration rows with S1 (tier B ordered by R4 total): expected order L21 > L06 > L07 > L03, against base total L21 = L06 > L07 > L03.
- Apply S2 to L05 with voize as the K2 example: criterion 8 ≤ 2 (−2 to −6 weighted points against a 3–5). See whether L05 drops out of the top 7.
- Apply S3 to L21: if TechBoost has no published intake, L21 becomes "K2 unproven" and loses its lead.
