# Source map: where healthcare pain and market signals show up (DE/EU)
Task: A2 | Date: 2026-11-06 | Status: draft

Access tested on 2026-11-06 from this session. `curl` = HTTP via the agent proxy (browser user agent). `WebFetch` = the built-in fetch tool. `Search` = WebSearch result snippets (not an opened source; claims from it get `[UNVERIFIED]` per rule 1). Grades follow `CLAUDE.md` rule 2. Bot checks were **not** bypassed. When curl met a bot check, the source is listed as blocked.

## Findings
- **Reddit is effectively unusable as a primary source in this setup.** Every reddit.com URL returns a JS bot challenge (`/r/Pflege/`: an 8 KB "Reddit" challenge page; `.json` endpoints: HTTP 403), and WebFetch refuses the host. Of 3 German `site:reddit.com` searches, **none** returned a reddit.com result. An English search returned only third-party mirror snapshots, which were not opened: reading Reddit through mirrors would route around Reddit's block, and the sandbox denied it. *Inference:* A3–A5 must lean on German forums, review sites and job/tender data. A Reddit API key created by the CEO remains the only clean route (already an open question).
- **Hard willingness-to-pay data is openly accessible, and it is the strongest new signal type.** The TED EU tender API (no key needed) returned **637** German notices since 1 Jan 2025 for software/IT services (CPV 48000000/72000000) whose full text matches "Krankenhaus". Among them: "Einführung eines Patientenportals (Aufnahme- und Behandlungsmanagement)" (Krankenhäuser Landkreis Freudenstadt) and "Einführung einer digitalen Pflege- und Behandlungsdokumentation" (Geomed-Kreisklinik) [A] ([TED API](https://api.ted.europa.eu/v3/notices/search)). The G-BA Innovationsfonds project list shows **861** funded projects [A] ([G-BA](https://innovationsfonds.g-ba.de/projekte/)).
- **Staff pain at scale is readable through employee reviews and job ads.** kununu works by curl: Helios Kliniken has "2855 Erfahrungen", average "3,1 von 5 Punkten … unter dem Durchschnitt der Branche" ([kununu](https://www.kununu.com/de/helios-kliniken/kommentare)); Korian Deutschland has 2017 reviews ([kununu](https://www.kununu.com/de/korian-deutschland/kommentare)) [C]. LinkedIn Jobs (logged out) shows "Medizinische Dokumentation Jobs in Germany (6,000+ Open Roles)" and "Medizinische Fachangestellte Jobs in München (1,000+ Open Roles)"; StepStone shows "326 Jobs" for MFA in München [B]. Indeed, Glassdoor and the BA Jobsuche API are blocked (403).
- **Patient pain from app reviews works through official endpoints.** The Apple App Store search API and the review RSS feed (50 most recent reviews per app, with date and star rating) work for DiGA apps. Example: somnio has 3,197 ratings with an average of 4.66; recent 1-star titles include "Anstrengend und hängt sich auf" ([iTunes RSS](https://itunes.apple.com/de/rss/customerreviews/id=1523016446/sortBy=mostRecent/json)) [C]. Google Play detail pages render review text server-side [C]. Trustpilot is blocked (curl 403, WebFetch DNS); search snippets only.
- **Science and statistics APIs work. Use them for [A] backing instead of the blocked web front ends.** Europe PMC REST (392 hits for `"nursing documentation" AND germany`), PubMed E-utilities, the ClinicalTrials.gov v2 API, the Eurostat API, the OECD SDMX API, Destatis, GBE-Bund and DRKS all work. The europepmc.org and oecd.org websites show a Cloudflare check and should not be used.
- **WebFetch is broadly broken in this session** (DNS `ENOTFOUND` for trustpilot, indeed, oecd, gutefrage, allnurses; reddit refused). Treat curl + local text extraction as the default fetch route. This confirms the A1 lesson.

## Details

Legend for Access: **works** = content readable via curl; **partial** = page loads but the key content is JS-rendered, login-walled or truncated; **blocked** = bot check / 403 / connection failure; **snippet** = only WebSearch snippets available.

### 1. Communities & forums (signal: pain, workarounds; grade [C])
| Source | Signal | Access | Recipe |
|---|---|---|---|
| Reddit (r/Pflege, r/medizin, r/germany, r/nursing, r/medicine, r/CaregiverSupport) | pain, workarounds (EN strong, DE weak) | **blocked** (JS challenge; JSON 403; WebFetch refused). Search: 0 reddit.com hits in 3 DE queries; EN hits = third-party mirrors only (not used) | Needs a Reddit API key (CEO). Until then, do not use it |
| krankenschwester.de forum (XenForo, nursing) | nurse pain (hospital, Altenpflege, Recht) | **works** (home + subforum index; robots allows threads) | Find threads via the forum's own pages. `site:krankenschwester.de` search returned nothing |
| medi-learn.de/foren (med students, junior doctors) | junior-doctor pain, workload | **works** | browse subforums "Arbeitsalltag" etc. |
| krebs-kompass.de (oncology patients/relatives, since 1997) | patient/caregiver pain | **works** (e.g. pancreatic cancer subforum `forumdisplay.php?f=10`) | browse by tumour subforum; no identifying details |
| rheuma-online.de, diabetes-forum.de, diabetes-online.de (Diabetes-Anker), onmeda.de/forum, medizin-forum.de, psychic.de, hilferuf.de | chronic-disease patient pain | **works** (home pages; thread URLs need to be taken from the index) | browse latest threads; count distinct threads per problem |
| alzheimer-forum.de, wegweiser-demenz.de, wir-pflegen.net, angehoerige-pflegen.de, BIVA, VdK | family caregiver pain, advice content | **works** | caregiver Q&A / Ratgeber pages + association position papers ([B]) |
| patient.info forums, HealthUnlocked, studentdoctor.net, Sermo (public pages) | EN patient/clinician pain | **works** (patient.info carers forum, HealthUnlocked search) | global fallback |
| gutefrage.net, rehakids.de, mumsnet, allnurses.com | DE Q&A, parents of disabled kids, nurses | **blocked** (Cloudflare) | snippet only |
| pflegeboard.de, altenpflegeforum.de, mfa-forum.de, pflegeforum.de, forum.alzheimer-forum.de, med-kolleg.de, facharzt.de | nursing/MFA/physician forums | **blocked** (502 / connection reset / TLS error) | retry later; snippet only |
| ALZConnected, Mayo Clinic Connect | EN caregiver pain | partial (ALZConnected 404 on tested link) / blocked (403) | snippet only |
| Facebook groups, LinkedIn posts/feed | care-staff and founder chatter | **blocked** (login wall; LinkedIn feed Cloudflare) | not usable; no sign-ups (rule 5) |
| DocCheck (community/news) | physician news, community | partial (home/news load; community is login-walled) | news only |

### 2. Reviews (signal: pain with existing solutions, competitor weaknesses; grade [C])
| Source | Signal | Access | Recipe |
|---|---|---|---|
| kununu (employers: hospital chains, care-home operators, Pflegedienste, practices) | staff pain: understaffing, documentation, management; ratings vs industry average | **works** (aggregate text + review text incl. "Verbesserungsvorschläge") | `kununu.com/de/<company>/kommentare`; search via `kununu.com/de/search?q=pflegedienst`. Count recurring themes; never quote names |
| Apple App Store (health apps, DiGA, practice apps) | patient pain with apps, onboarding friction, competitor gaps | **works** via `itunes.apple.com/search?term=…&country=de&entity=software` (rating counts) + `itunes.apple.com/de/rss/customerreviews/id=<id>/sortBy=mostRecent/json` (50 recent reviews) | pull 1–2-star reviews per competitor; tally complaint types |
| Google Play | same | **works** (detail page has rating, count and review text server-side) | `play.google.com/store/apps/details?id=<pkg>&hl=de`; search page lists package IDs |
| Trustpilot (insurers, Doctolib, telemedicine) | payer/service pain | **blocked** (curl 403, WebFetch DNS); **snippet** works (e.g. insurer pages with ratings/counts in snippets) | `site:trustpilot.com <Kasse>`; mark `[UNVERIFIED]` |
| Jameda, Doctolib | patient reviews of practices | partial (Jameda home works; tested search URLs 404) | find practice URLs via search, then curl |
| klinikbewertungen.de, sanego.de | hospital/clinic reviews | **works** (home); deep URLs must come from the site's own links | patient experience by department |
| werkenntdenbesten.de, reviewhero.io | care-home reviews (aggregated Google reviews) | snippet seen in search | test before use |
| Google Maps reviews | provider reviews | partial (JS shell, reviews not extractable) | not usable |
| Glassdoor | staff pain | **blocked** (403) | use kununu instead |
| Capterra.com.de, G2, TrustRadius | B2B software reviews (practice/clinic/care software) = competitor weaknesses | Capterra DE **works**; G2/TrustRadius **blocked** | Capterra DE category pages for Praxissoftware / Pflegesoftware |

### 3. Job postings (signal: what providers cannot staff or still do by hand; [B] for counts, [C] for interpretation)
| Source | Access | Recipe |
|---|---|---|
| LinkedIn Jobs (logged-out search) | **works** (title gives count, e.g. "6,000+ Open Roles") | `linkedin.com/jobs/search?keywords=<role>&location=<place>`; compare counts across roles (Kodierfachkraft, Medizincontroller, Study Nurse, Pflegedokumentation, Entlassmanagement) |
| StepStone | **works** (e.g. "326 Jobs" MFA München) | `stepstone.de/jobs/<role>/in-<city>` |
| XING Jobs, medi-jobs.de, praktischarzt.de, kliniken.de | **works** | sector-specific boards |
| BA Jobsuche (web) | **works** (home); REST API **blocked** (403 even with the public header) | web search UI only |
| Indeed, Monster | **blocked** (security check / 403) | snippet only |

Caution: counts are rough (duplicates, ranges like "1,000+"), so use them only for relative comparisons. Read job descriptions for manual tasks, e.g. "Dokumentation", "Kodierung", "Terminmanagement".

### 4. Public tenders (signal: real budgets = willingness to pay; grade [A])
| Source | Access | Recipe |
|---|---|---|
| TED (EU tenders) API v3 | **works**, no key: `POST https://api.ted.europa.eu/v3/notices/search` with an expert query, e.g. `classification-cpv IN (48000000 72000000) AND buyer-country=DEU AND publication-date>=20250101 AND FT~"Krankenhaus"` → 637 notices | swap the FT term (Pflege, Pflegeheim, Krankenkasse, Telemedizin, KI) and the CPV (33000000 medical devices, 85000000 health services, 48180000 medical software); read titles + buyer names. The ted.europa.eu website returns 202/empty (bot check) |
| service.bund.de Ausschreibungen | **works** (search UI; a "Krankenhaus Software" query returned 1 result page) | federal/Länder tenders below EU thresholds |
| DTVP | **works** (search page) | many hospital/municipal buyers |
| evergabe-online.de | partial (cookie wall) | — |

### 5. Funding & innovation data (signal: what gets funded, competition; [A] public, [B] commercial)
| Source | Access | Recipe |
|---|---|---|
| G-BA Innovationsfonds projects | **works** ("861 Ergebnisse") | filter by Versorgungsform/topic; results/recommendations ("Rückmeldungen") show what the G-BA wants transferred into standard care |
| CORDIS | **works**, incl. JSON: `cordis.europa.eu/search/en?q=contenttype='project' AND '<term>'&format=json` ("nursing" → 164 projects) | EU-funded consortia = competitors/partners |
| EU Funding & Tenders portal (SEDIA search API) | **works** (`api.tech.ec.europa.eu/search-api/prod/rest/search?apiKey=SEDIA&text=…`) | open EIC/Horizon/EU4Health calls (A6) |
| Förderkatalog Bund (foerderportal.bund.de/foekat) | **blocked** (connection refused) | snippet only |
| foerderdatenbank.de | **blocked** (Radware captcha) | snippet only |
| Crunchbase, Dealroom | **blocked** (Cloudflare) | snippet only; mark `[UNVERIFIED]` |
| North Data, Handelsregister, Unternehmensregister, Bundesanzeiger | North Data **429** after 1 request; others **work** (home) | company filings/financials of competitors ([A] filings) |
| Munich Startup platform, healthcare-startups.de, deutsche-startups.de, Gründerszene, tech.eu | **works** | Munich/DE health startup lists, funding news ([B]) |
| sifted.eu, eu-startups.com | **blocked** (Cloudflare) | snippet only |
| UnternehmerTUM, BioM, EIT Health, Bayern Kapital, LfA, EXIST, BMFTR Gesundheitsforschung, StMGP, StMWi, IHK München, Bayern Innovativ | **works** | A6 inputs |
| Medical Valley EMN, digitalhealth-bayern.de | **blocked** (502) | snippet only |

### 6. Policy & payers (signal: rules, money flows, payer priorities; [A] official, [B] insurer/association reports)
| Source | Access | Recipe |
|---|---|---|
| BMG (incl. "Gesetze und Verordnungen 21. LP"), G-BA (Beschlüsse), BfArM (DiGA pages), GKV-Spitzenverband, KBV, Zi, IQWiG, IQTIG, gematik, RKI, BÄK | **works** | Referentenentwürfe, Beschlüsse, press releases. Note: the DiGA-Verzeichnis web app needs JS and its FHIR API returns 401 |
| Bundestag: bundestag.de, Drucksachen PDFs (`dserver.bundestag.de/btd/21/…`) | **works** | Kleine Anfragen = official answers with data |
| DIP API | partial: key required. The Bundestag publishes the current public key on its JS help page, which could not be read as text. The info sheet confirms the key requirement ([PDF](https://dip.bundestag.de/documents/informationsblatt_zur_dip_api.pdf)) | use dip.bundestag.de web UI or Drucksachen PDFs |
| Insurers: TK press/topics, AOK-Presse + WIdO, BARMER + bifg, DAK, vdek, BKK Dachverband, IKK classic, PKV-Verband | **works** (the DAK report URL tested was 404; find the current one via search) | Reports (Pflegereport, Arztreport, Gesundheitsreport) = [B]; WIdO/bifg studies = [B], or [A] if peer-reviewed |
| Associations: DKG, bpa, DBfK, Hausärzteverband, VMF, Hartmannbund, Marburger Bund, BVMed, vfa, BPI, Bitkom, BVDW | **works** | position papers, surveys ([B]) |
| SVDGV (digital health association) | **blocked** (TLS/502) | snippet only |
| gesetze-im-internet.de, eur-lex.europa.eu | **works** (home; A1 had failures, so deep links need retesting) | primary law text |
| BAS (Bundesamt für Soziale Sicherung) | **blocked** (connection reset) | snippet only |

### 7. Statistics & science (signal: problem size; grade [A])
| Source | Access | Recipe |
|---|---|---|
| Destatis (press releases, pages) | **works** | press releases + tables; GENESIS-Online web is JS |
| GBE-Bund | **works** (home) | health reporting tables |
| Eurostat (site + `ec.europa.eu/eurostat/api/dissemination/statistics/1.0/data/<dataset>`) | **works** | EU comparisons |
| OECD | website **blocked** (Cloudflare); **SDMX API works** (`sdmx.oecd.org/public/rest/…`) | Health Statistics via SDMX |
| PubMed | E-utilities **work** (`eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi?db=pubmed&term=…&retmode=json`; a test query returned 24 hits); web front end loads but showed a bot check earlier (lessons) | use E-utilities for IDs/abstracts |
| Europe PMC | REST API **works** (`ebi.ac.uk/europepmc/webservices/rest/search?query=…&format=json`); europepmc.org web **blocked** | full-text OA via API |
| Springer Medizin, Thieme, Ärzte Zeitung | **blocked** (client challenge / DNS) | snippet only |

### 8. Trade press & events (signal: trends, competitor launches, buyer priorities; grade [B])
| Source | Access |
|---|---|
| Ärzteblatt, kma-online (incl. "IT & Digital Health"), PZ, DAZ, apotheke adhoc, zm-online, Medical Tribune, bibliomed-pflege, altenheim.net, HCM, E-HEALTH-COM, healthcare-in-europe, mednic, DeviceMed, Healthrelations, Pharma Relations, mta-dialog, STAT News | **works** |
| DMEA (programme page), YouTube search (titles in page JSON), Apple Podcasts, ARD Audiothek | **works** (DMEA programme = what buyers and vendors talk about) |
| Handelsblatt Inside Digital Health | partial (paywall stub) |
| Tagesspiegel Background Gesundheit, Ärzte Zeitung, FierceHealthcare/FierceBiotech, MobiHealthNews, Clinical Trials Arena | **blocked** (Cloudflare / 403) → snippet only |
| care-invest.net | **blocked** (TLS) |

### 9. Demand signals (signal: interest, competition, R&D activity)
| Source | Signal / grade | Access |
|---|---|---|
| Google Trends | relative search interest [B] (relative only, never market size) | **blocked** (429 on explore; API endpoint 404) |
| Google Patents | competition/R&D [A] | partial (JS shell) |
| DPMAregister | DE patents [A] | **works** (basic search page) |
| Espacenet | EP patents [A] | **blocked** (403) |
| Lens.org | patents + scholarly [A] | **works** (home; search UI is JS, untested) |
| ClinicalTrials.gov v2 API | trial activity, sponsors [A] | **works** (e.g. `query.locn=Munich&filter.overallStatus=RECRUITING` → totalCount 300) |
| EU CTIS (euclinicaltrials.eu) | EU trials [A] | partial (page loads; search is JS) |
| DRKS | DE trials [A] | **works** |

### Recommended recipe per upcoming task (inference)
- **A3 patients & caregivers:** DE forums (krebs-kompass, rheuma-online, diabetes forums, alzheimer-forum, onmeda) + App Store/Play reviews of DiGA and of caregiver apps + association pages (VdK, BIVA, wir pflegen) for [C]. Back with Destatis, GBE and insurer reports for [A]/[B]. For each problem, count distinct threads/reviews, not posts.
- **A4 professionals:** kununu (top hospital chains, care-home operators, ambulante Dienste, MVZ chains) + LinkedIn/StepStone role counts + krankenschwester.de/medi-learn for [C/B]. Use TED tenders for what hospitals actually buy [A]. Trade press (kma, bibliomed-pflege, Ärzteblatt) [B]. Use KBV/Zi/DKG surveys and PubMed via E-utilities for [A]/[B] backing.
- **A5 industry/payers:** TED + service.bund (payer and public-health tenders), ClinicalTrials.gov/DRKS/CTIS (trial ops), LinkedIn role counts (Study Nurse, CRA, Medical Writer, Kodierfachkraft), Capterra DE (incumbent software complaints), insurer reports, vfa/BPI/BVMed papers.
- **A6/A9:** EU F&T SEDIA API, EXIST, BMFTR, StMWi/StMGP, Bayern Kapital, LfA, BMG/BfArM/GKV-SV, Bundestag Drucksachen. Crunchbase/Dealroom are snippet-only, so investor claims there must be confirmed on investor websites.

## Gaps / [UNVERIFIED]
- Reddit content: not accessible (see Findings). Third-party Reddit mirrors appeared in search results; they were deliberately not opened. Their snippet content is not used anywhere.
- Facebook/LinkedIn groups and posts: not accessible without login, and logging in would need a sign-up (rule 5).
- Google Trends: no working route found.
- Deep-page access was tested on samples only. A host that "works" on its home page can still fail on deep links (e.g. Jameda/klinikbewertungen search URLs returned 404 because the URL pattern was wrong, not because of a block). Test deep URLs per task.
- Blocked statuses are one-time tests and may be transient (502s, connection resets). Retest before giving up on a host.
- Indeed/Glassdoor/Trustpilot/Crunchbase/Dealroom/OECD web: blocked by bot checks. They were not bypassed and would need an allowlist change or a different access route.
- Trustpilot insurer ratings seen in search snippets (e.g. KKH "906" reviews) are `[UNVERIFIED]`: snippet only.

## Sources
All accessed 2026-11-06 via curl unless noted.
- https://www.reddit.com/r/Pflege/ — JS bot challenge page (access test)
- https://www.reddit.com/r/Pflege/top.json?t=year&limit=2 — HTTP 403 (access test)
- https://api.ted.europa.eu/v3/notices/search — 637 DE notices (CPV 48000000/72000000, since 2025-01-01, FT "Krankenhaus"); notice titles and buyers quoted
- https://innovationsfonds.g-ba.de/projekte/ — "861 Ergebnisse" funded projects
- https://cordis.europa.eu/search/en?q=contenttype%3D%27project%27%20AND%20%27nursing%27&format=json&p=1&num=1 — 164 hits
- https://api.tech.ec.europa.eu/search-api/prod/rest/search?apiKey=SEDIA&text=health%20digital&pageSize=1&pageNumber=1 — EU F&T search API works
- https://www.kununu.com/de/helios-kliniken/kommentare — 2855 reviews, 3.1/5, below industry average
- https://www.kununu.com/de/korian-deutschland/kommentare — 2017 reviews; review text incl. Verbesserungsvorschläge readable
- https://www.linkedin.com/jobs/search?keywords=Medizinische%20Dokumentation&location=Germany — "6,000+ Open Roles"
- https://www.linkedin.com/jobs/search?keywords=Medizinische%20Fachangestellte&location=M%C3%BCnchen — "1,000+ Open Roles"
- https://www.stepstone.de/jobs/medizinische-fachangestellte/in-muenchen — "326 Jobs"
- https://itunes.apple.com/search?term=diga&country=de&entity=software&limit=5 — App Store search API (somnio 3197 ratings, avg 4.66; Oviva 23625)
- https://itunes.apple.com/de/rss/customerreviews/id=1523016446/sortBy=mostRecent/json — 50 recent reviews with ratings/dates
- https://play.google.com/store/apps/details?id=de.mementor.somnio&hl=de — rating 4.5, review text server-side
- https://www.ebi.ac.uk/europepmc/webservices/rest/search?query=%22nursing%20documentation%22%20AND%20germany&format=json&pageSize=2&resultType=lite — hitCount 392
- https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi?db=pubmed&term=nursing+documentation+burden+germany&retmode=json — count 24
- https://clinicaltrials.gov/api/v2/studies?query.locn=Munich&filter.overallStatus=RECRUITING&countTotal=true&pageSize=1&fields=NCTId — totalCount 300
- https://sdmx.oecd.org/public/rest/dataflow/all — OECD SDMX API works
- https://dip.bundestag.de/documents/informationsblatt_zur_dip_api.pdf — DIP API needs a key (Stand März 2023)
- https://www.krankenschwester.de/forum/ and https://www.krankenschwester.de/robots.txt — forum structure and crawl rules
- https://www.krebs-kompass.de/forumdisplay.php?f=10 — patient forum subforum readable
- https://patient.info/forums/discuss/browse/carers-2125 — EN carers forum readable
- https://www.service.bund.de/Content/DE/Ausschreibungen/Suche/Formular.html — tender search works
- https://www.youtube.com/results?search_query=pflegedokumentation — titles readable from page JSON
- Access status of the other hosts (~200 URLs tested in total) listed in the tables: home or listed URLs tested on 2026-11-06 (HTTP status + page title). The raw log is not kept in the repo.
- WebSearch (snippet only, not opened): `site:reddit.com Pflege Dokumentation Zeit Patienten`, `site:reddit.com r/medizin Praxis Bürokratie Termin`, `reddit r/Pflege Dokumentation "keine Zeit"` (0 reddit.com hits); `site:reddit.com nurses charting takes too long` (mirror hits only); `site:trustpilot.com Krankenkasse Bewertung Bearbeitung` (Trustpilot snippets available)
