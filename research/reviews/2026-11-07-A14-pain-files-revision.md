# Fact-check: research/pain-industry.md, pain-patients.md, pain-professionals.md (A14 revision, commit b976400)
Date: 2026-11-07 | Verdict: pass for the parts checked; NOT a full re-check | Sources checked: 24 claims/URLs sampled from the ~237 changed lines of pain-industry.md; pain-patients.md and pain-professionals.md revisions not read in full

The A14 revision merged during this run. Scope here: the new payer/MD/trial claims added to `pain-industry.md` (tender access table, I1/I5/I6 rows, MD care assessments, barometer). The pain-patients and pain-professionals edits (WTP downgrades, MDR caveat, sourced counts) are **not** fact-checked yet; see the fix task.

## Critical issues (must fix)
None found in the sample.

## Issues
1. **Propagated unverified claim.** `pain-industry.md` "Competition [B] (verified in A13)": "TriNetX owns Clinerion". A13 itself lists the TriNetX–Clinerion takeover as snippet-level; the opened source says Citeline (Norstella) bought Clinerion in 2023. See `2026-11-07-trial-recruitment-de.md` issue 1. Remove "verified" or the ownership claim.
2. **"Participants recruited in Germany fell from about 33,000 to about 24,000 (Oct 2025 deck)"** — the numbers 33,000 / 24,000 are not in the extractable text of the Oct 2025 deck (the 4.5 % → 3.0 % share and the "stagnierende Studienstarts und sinkende Teilnehmerzahlen pro Studie" text are). They may sit in a chart image; unverified by text search.
3. **PKV ombudsman figure.** The PKV page says "0,001 Prozent der Fälle" for 6,891 of >70m invoices; the file computes 0.01 %. 6,891 / 70,000,000 = 0.0098 %, so the file's own maths is right and the PKV page figure is off by 10×. Keep the file's number; add one clause saying so.
4. **MD Bund "über 3 Millionen Pflegebegutachtungen im Jahr 2025"** supported; ">5.6m, doubled since 2014" is from the vdek magazine page, not from the MD Bund press release it sits next to. Cite vdek.

## Source check (sample)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| "72 Prozent der Unikliniken unterschreiten ...", 68 %, outlook +34 → +7, 83 % | Ärzteblatt 28 Sep 2026 | supported | |
| Germany "etwa 2,9 Prozent" for 2024; 4.5 % (2014) → 3.0 % (2024) | Ärzteblatt; vfa Oct 2025 deck | supported | |
| CTIS 668 of 1,356 | own count | supported (re-run in A13 review) | |
| AOK Hessen 761998-2025: €6m annual turnover, ISO 9001, 2 references | TED | supported | |
| Pronova 177834-2026: €1,200,000 min. turnover from the tendered service | TED | supported | |
| BAHN-BKK 269243-2025: 3 references from insurers with ≥1m prescriptions / 300,000 invoices, 2 on 21c\|ng | TED | supported | |
| AOK BW 673984-2025: ≥10m scanned pages/yr reference; €10m liability | TED | supported | |
| BIG 189396-2025: €250,000 turnover, 3 references | TED | supported | |
| AOK NordWest 481787-2026 (3 references); AOK RH/HH 518174-2026 (€10m cover); MD RLP 543912-2025 (one reference, PoC counts); MD Bayern 63363-2025 (€100,000, 3 references) | TED | supported | |
| 1,431,000 care assessments in 2013 (1,123,000 + 308,000) | MDS Faktenblatt 2014 | supported | |
| 64 % of orphan-device makers: 14 of 22 | BVMed/SPECTARIS survey | supported | |
| 92 insurers (7 Nov 2026) | GKV-SV list | supported | |

## [UNVERIFIED] items
- Carried forward from the file: Trials24, Probando, GKV staff age structure, PKV automation rates. Flagged in text; none used as a fact.
