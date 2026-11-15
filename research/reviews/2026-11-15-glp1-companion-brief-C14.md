# Fact-check: ventures/glp1-companion/brief.md (after C14)
Date 2026-11-15 | Verdict: **pass with caveats** (one misread trial result; caveats only, rule 14) | Sources checked: 16 of 16 new or changed citations opened (all of them, not a sample) + 3 PubMed abstracts via NCBI E-utilities + App Store lookup re-run + all section 5 arithmetic re-computed

Scope: the C14 revision (commit 6921264), i.e. the fixes for `research/reviews/2026-11-15-glp1-companion-brief.md` (fact-check) and `research/reviews/2026-11-15-redteam-glp1-companion-brief.md` (red team), plus the ~15 sources the researcher added. Sources unchanged since the first fact-check were not re-opened. This is the second look after the one fix round, so remaining issues are **caveats for the CEO, not new tasks** (CLAUDE.md rule 14). None of them changes decision C12.

**Summary for the CEO:** the fix round worked. All 12 first-round issues are fixed: one price (€129 per 12-week programme) is now used everywhere, and the pass mark, kill lines and allowance all follow from it; the arithmetic re-computes exactly. Every new source says what the brief says, with one exception: the Danish trial (S-LiTE) cited as "the closest evidence" that exercise helps people keep weight off after stopping. The brief says people who exercised *during* the drug regained 6.0 kg less than those on the drug alone. The 6.0 kg is for people who exercised *without* the drug. People who combined exercise with the drug regained 2.5 kg less, and that difference was not statistically significant. So the product's best evidence is weaker than written. This supports the brief's own recommendation (drop, C12 option d); it does not reverse it.

## Critical issues (must fix)
None that change a decision. Per rule 14 the following is a **caveat**, not a fix task:

1. **S-LiTE result misread (section 1; repeated in the `progress.md` C14 log entry).** Brief: "people who had done supervised exercise *during* a year of liraglutide regained 6.0 kg less in the year after stopping than those on the drug alone". The abstract ([PMID 38544798](https://pubmed.ncbi.nlm.nih.gov/38544798/)) says: "weight regain was 6.0 kg [2.1; 10.0] larger after termination of liraglutide compared with after termination of supervised exercise and 2.5 kg [-1.5 to 6.5] compared with after termination of combination treatment." The 6.0 kg compares exercise **alone** (no drug) with liraglutide alone. For exercise **plus** the drug, the regain difference was 2.5 kg with a confidence interval that crosses zero. What the trial does support for the combination: one year after stopping, the combination group weighed 5.1 kg less than the liraglutide-only group, measured from randomisation (P = 0.040), and more of them kept ≥10 % weight loss (OR 4.2). Correct reading: "In S-LiTE, people who combined exercise with liraglutide regained 2.5 kg less after stopping than those on liraglutide alone (not significant), and were 5.1 kg lighter one year later. The 6.0 kg difference was for exercise without the drug." Effect on the brief: the "Unproven" label in section 1 stays right and gets stronger. The section 12 and 13 numbers do not depend on it.

## Other issues (minor, caveats)
2. **ZEPmedi-doc "phases the drug out" (bottom line) / "a clinical, in-person route to 'stop well'" (section 6).** The TOPFIT 2/2026 interview describes a multimodal programme *with* the drug (check-ups every 4–6 weeks, coaching). It reports that the first patients "konnten … nach einigen Monaten auf die Inkretine-Mimetika verzichten, ohne wieder nennenswert zuzunehmen". It describes no structured taper or exit programme. Partially supported: a programme in which some patients came off the drug, not a phase-out programme.
3. **Gerresheimer residue in section 7 (i):** "Gerresheimer offers white-label software to pharma". Section 6 was fixed to the page's wording ("We are developing a GLP-1 obesity support app … ready for customization to the individual requirements of a pharma company"). Section 7 still says "offers white-label". Read as "is developing customisable software for pharma".
4. **nachderspritze.de "one-person project" (section 6, Funding / size column).** The page writes in the plural ("wir") and gives one personal contact address. "One-person" is an inference without a tag. It does not matter for any conclusion.
5. **Meta quote is from a WebFetch summary, not the page text** (the brief says so). Curl returns HTTP 400. My WebFetch summary renders the age rule as "must be targeted to people at least 18 years or older"; the brief has "aged at least 18 years or older". Same meaning; treat the wording as not verbatim-verified. Revision 22 Jul 2026 confirmed; the page does not mention coaching services (also as the brief says).

## Source check (new or changed citations)
| Claim | Source | Verdict | Note |
|---|---|---|---|
| Regain "0.4 kg" a month; 37 studies, 9,341 participants; markers to baseline "within 1.4 years"; faster than after behavioural programmes "by 0.3 kg" a month | BMJ 2026, PMID 41500720 | supported | All numbers verbatim in the abstract. Brief grades [A]: correct |
| S-LiTE: exercise during liraglutide → 6.0 kg less regain vs drug alone; 109 at follow-up | EClinicalMedicine 2024, PMID 38544798 | **not supported as worded** | 109 correct. 6.0 kg = exercise alone vs liraglutide alone; combination vs liraglutide = 2.5 kg, n.s. (issue 1) |
| SURMOUNT-MAINTAIN: −16.6 % (5 mg) vs −21.9 % (MTD) vs −9.9 % (placebo) at week 112; 378 randomised; USA; Lilly-funded | Lancet 2026, PMID 42119587 | supported | "Reducing to 5 mg tirzepatide might provide a valuable alternative to discontinuation" in the interpretation. Brief's "kept most of the weight off" is a fair reading |
| Juniper UK: "on average, for 183 days"; cost 38.7 %, results 16.8 %, side effects 15.4 %, goal achieved 7.3 %; 24 Mar 2026 | eucalyptus.health research page | supported | Page says "Juniper UK patients" and "real-world study" where patients pay. [B] as a company summary is right |
| Hims & Hers–Eucalyptus "up to $1.15 billion", ~$240m cash at closing; 21 Feb 2026 | Pulse 2.0 | supported | Fixes first-round issue 6 |
| nachderspritze.de: 2 × 30 min strength, protein target, small-portion recipes, weight corridor, weekly e-mail check-in "auf deine Fragen antwortet ein Mensch", "unter 129 €", still a waitlist, protein + creatine starter-pack interest, does not promise to prevent the "Jojo-Effekt" | nachderspritze.de home page | supported | All verbatim. "One-person project": issue 4 |
| formoline "Gewicht halten nach der Abnehmspritze"; free app My-formoline; class III device; Certmedica, Aschaffenburg | glp-1-weiterdenken.de, /patient/ | supported | "Medizinprodukt Klasse III (CE 0123)" |
| formoline to doctors: "Bei Therapieabbruch der Abnehmspritze" | DocCheck advertorial | supported | |
| formoline L112 EXTRA €95.79 / 192 tablets, UVP €123.90; 2 × 2 a day, 2 a day for weight control → €30–60/month | shop-apotheke.com | supported | Arithmetic: 95.79/96×30 = 29.9; 95.79/48×30 = 59.9. Match |
| ZEPmedi-doc, Barmherzige Brüder München; check-ups every 4–6 weeks; "verzichten, ohne wieder nennenswert zuzunehmen" | TOPFIT 2/2026 PDF | partially | Quote and facts verbatim; "phases the drug out" overstated (issue 2) |
| WW US: "Members who stayed engaged with Weight Watchers after discontinuing their medication continued to see results"; 14 Sep 2026 | WW US blog | supported | Visible date 14 Sep 2026 (JSON-LD 15 Sep UTC). Company claim; [B] fine |
| glp-1forum.de article "Abnehmspritze absetzen: Muss man ein Leben lang spritzen?" 14 Nov 2026 | glp-1forum.de | supported | [C] correct |
| zanadio "Medizinprodukt der Klasse 2a" | golighter.de/p/abnehm-app | supported | Fixes first-round issue 7 |
| Gerresheimer "We are developing a GLP-1 obesity support app …"; "ready for customization …" | gerresheimer.com | supported (section 6) | Section 7 residue: issue 3 |
| YouGov: "Bereits mehr als vier Millionen Haushalte nutzen in Deutschland GLP-1-Medikamente oder ziehen ihre Nutzung in Betracht" | YouGov 53896 | supported | Now verbatim (first-round issue 5 fixed) |
| Voy "Ab 248 € 173 € pro Monat", €100 off first 2 months; no leaver programme on home page | myvoy.de | supported | No "absetzen"/maintenance-after-stop text on the home page |
| Meta weight-loss ad rules (18+, no side-by-side, no negative self-perception, Rx → drugs policy); revision 22 Jul 2026 | transparency.meta.com | supported via WebFetch | Curl HTTP 400; wording not verbatim-verified (issue 5) |

**Re-run counts (App Store lookup, 2026-11-15)**
| Count | Brief | Re-run | Result |
|---|---|---|---|
| Shotsy DE ratings | 1,738 | 1,742 | match (+4 in a day) |
| Juniper DE ratings / average | 96 / 3.79 | 96 / 3.79 | match |

**Arithmetic (section 5, 12, 13 after C14)**
| Item | Re-computed | Result |
|---|---|---|
| €129 / 2.8 months | €46.1/month | match |
| TAM 100k / 300k / 550k × €129 | €12.9m / €38.7m / €71.0m | match |
| Three salaries: 180,000 / 0.4 = 450,000; / 129 | 3,488 | match |
| €1m / 129 | 7,752 (7.8 % of 100,000) | match |
| Allowance 0.39 × 129 / 0.46 × 129 | €50.3 / €59.3 | match |
| Sensitivity 129 × 1.3 = 167.7 → €65–77; €90 → €35–41 | | match |
| COGS 20 % × 129 | €25.8 | match |
| Pass ≥10 paid for €300 (≤ €30); kill < 6 (> €50) | 300/10 = 30; 300/6 = 50 | match; consistent with the €50–59 allowance and R1/R2 |
| Marketing for €1m at 39–46 % | €390–460k | match |

**First-round issues (2026-11-15 fact-check), status**
| # | Issue | Status |
|---|---|---|
| 1–3 | One price; per-theme pass mark; R2 kill vs allowance | fixed (one price €129; single-theme test; R1/R2 kill at €50 / €59) |
| 4 | YouGov 53834 date | fixed (13 Jan 2026) |
| 5 | YouGov 53896 quote | fixed (verbatim) |
| 6 | Juniper $1.15bn | fixed (Pulse 2.0, 21 Feb 2026) |
| 7 | zanadio class IIa | fixed (GoLighter page) |
| 8 | Gerresheimer wording | fixed in section 6; residue in section 7 (issue 3) |
| 9 | Voy list vs promo | fixed |
| 10 | Herbalife opened | fixed |
| 11 | Forum as free substitute | fixed (section 6 row) |
| 12 | BayDiGuP "no 2026 call" | fixed |

## Evidence grades
- New [A] items (BMJ meta-analysis, S-LiTE RCT, SURMOUNT-MAINTAIN RCT) are peer-reviewed: [A] correct. SURMOUNT-MAINTAIN is sponsor-run (Lilly), which the brief states.
- Eucalyptus summary of its own study at [B] (company source) is right; the brief says "company-reported" and "UK, not DE".
- formoline, DocCheck advertorial, WW US blog, ZEP clinic magazine at [B]: vendor or house media; acceptable as evidence that the offers exist, not of outcomes. The brief uses them only for existence.
- No market size rests on [C]. No new data older than 3 years drives a conclusion (S-LiTE 2024 is under 3 years old).

## [UNVERIFIED] items
| Item | Treated as fact or built on? |
|---|---|
| Search ads on stop-related queries allowed (section 13) | No: listed as a channel option to check |
| Naming the target group in ads; MDR reading of the positioning; pre-order consumer law (lawyer question) | No: the test is conditional on the lawyer hour |
| Juniper DE prices (snippet), OLG appeal, GDPR details, Google ad rules, contract-maker unit price, pflueger.de | No |
| Seller set-up needs (trade registration, employer consent) labelled *inference; not checked* | No: listed as preconditions |

No fabrication found: all new quotes trace to opened pages; no interviews claimed.
