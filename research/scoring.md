# Scoring framework (Stage B)

CEO decision 2026-11-07 (chat): keep the 9 criteria, add knock-outs K1/K2, and rank by confidence (rules R1–R4) instead of exact totals. Basis: `research/reviews/2026-11-07-redteam-scoring.md`.

## Step 1: knock-outs (any one → not in the top 5; list the row with the reason)
| # | Knock-out | Test |
|---|---|---|
| K1 | **No buyer with proven spend** | No tender, contract, budget line, price list or observed paid purchase in the category. "Payer unclear" = out. |
| K2 | **No startup-accessible first sale in ≤12 months** | Every known buyer route needs turnover, references or certificates a new company lacks, and there is no direct-award-sized pilot (≤€100k; Art. 20 BayWiVG for Bavarian public buyers, ≤€50k federal from 1 Jul 2026), private buyer, or channel/subcontract route. Cite the selection criteria you checked. |

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
- **R1** Tag every score **H/M/L**. H = ≥1 [A]/[B] item directly on point and no counter-source. M = indirect [B] or inference from [A]. L = [C] only, snippet only, or inference.
- **R2** An **L** score counts as **at most 3** in the total. Unknown = L = no bonus.
- **R3** Criterion 3 or 5 at **L** → row marked **"unproven"**. It may enter the top 5 only with a named cheap test to run before Stage C.
- **R4** Sensitivity: re-rank with every L score −1. Report a row as top 5 only if it stays in the top 7. Present **tiers (A/B/C)**, not exact ranks, and publish the sensitivity check next to the ranking.

## Output (`research/shortlist.md`)
Knock-out list with reasons; scoring table (score, confidence, evidence link per cell); tiers; sensitivity check; top 5 with reasoning.
