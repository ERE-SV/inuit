# Phase 07 — Data profiles, acquisition & matching — Worksheet

**Status:** not-started  
**Unlocks:** Data v0 with product scope (Week 7); depth Weeks 10–11; **Gate 4** with Phase 06  
**Primary path:** this file  
**Seeded start:** [DATA-DICTIONARY.md](DATA-DICTIONARY.md), [SEARCH-DIMENSIONS.md](SEARCH-DIMENSIONS.md), [DATA-ACQUISITION.md](DATA-ACQUISITION.md)  

## Learn (read before working)

### What this phase is

You define **what data exists**, **where it comes from**, and **how matching uses it** so an engineer can implement without a strategy workshop. Both sides have a **search profile**: seekers search for jobs; companies search for people. Start from the seeded dictionary — mark **keep / cut / add** — then specify acquisition, dimensions, hard vs soft rules, privacy, and fairness.

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Search profile** | Structured preferences + constraints used to find the other side | Same idea both sides; not only a CV or a job ad |
| **Profile fields** | Facts about the person or company/job (education, skills, locations) | What users enter or what we ingest |
| **Hard filter** | Must-pass rule (fail → not shown / not ranked) | Commute max, work auth, must-have language |
| **Soft score** | Weighted preference that raises/lowers rank when hard filters pass | Nice-to-have skills, culture tags |
| **Acquisition method** | How a field gets filled: user input, feed/API, crawl, enrichment, inferred, computed | Confidence + legal notes differ by method |
| **Inferred** | Derived (e.g. LLM from job text), not typed by employer | Must be labeled in UI; lower confidence |
| **Top-X** | Short ranked list above a threshold | Product promise: fewer, better — not infinite inbox |
| **Explainability** | Short “why this match” (criteria hit/miss) | Trust; not a black-box score |
| **Asymmetric preference** | One side cares about a dimension the other doesn’t store (e.g. commute) | Needs workplace geo + seeker home + computation |
| **Fairness / prohibited criteria** | Rules you will not automate or will constrain | Legal + brand trust |

### Acquisition methods (student level)

| Method | Meaning | Typical use here |
| --- | --- | --- |
| **User input** | Person or company types it | Seeker profile; first-party job requirements |
| **Feed / API** | Licensed or official listing data | Bootstrap job title, location, raw description |
| **Crawl** | Fetch pages on an allowlist (fragile; legal care) | Gap-filler career pages — not primary scale plan |
| **Enrichment** | Third-party or public datasets | Salary bands, transit — contracts + caution |
| **Inferred** | Model extracts structure from text | P1 requirements from listings |
| **Computed** | Calculated from other fields | Commute minutes from home + workplace |

### Common beginner mistakes

- Treating every preference as a hard filter (liquidity dies)  
- Inventing salary or culture facts when enrichment is missing  
- Sending raw home address to employers  
- Soft “culture fit” with no definition → bias risk  
- Dictionary fields that no MVP screen collects or shows  
- Matching spec that an engineer cannot implement (vague weights, no fail behavior)  
- Skipping fairness / prohibited automated criteria  

## How to prove answers

- Field decisions → updated rows in DATA-DICTIONARY / SEARCH-DIMENSIONS / DATA-ACQUISITION / MATCHING-SPEC  
- Legal/privacy notes are **product constraints to flag**, not legal advice  
- Label inferences; cite URLs for any external enrichment source claims  
- Follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)  

## Tasks

### [ ] 07-T1 — Search profiles & dictionary keep/cut/add

**Done when:** Seeker profile, seeker search, company profile, and job requirement tables are decided (keep/cut/add) with types and privacy notes.  
**Unlocks / feeds:** Week 7 alignment with product screens; Gate 4  

#### Sub-questions

- [ ] **07-T1-Q1.** In your own words: what is a **search profile**, and why do **both** seekers and companies have one?
  - **Answer:**  
  - **Proof:** (path: brief `02-product.md`)  

- [ ] **07-T1-Q2.** For every row in **Seeker — profile fields** in [DATA-DICTIONARY.md](DATA-DICTIONARY.md): mark **keep / cut / add**. Summarize cuts and any new fields.
  - **Answer:**  
  - **Proof:** (path: updated dictionary)  

- [ ] **07-T1-Q3.** Same for **Seeker — search / constraint fields**.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T1-Q4.** Same for **Company — profile** and **Job — requirement** tables. For each kept job field, is it **must**, **nice**, or **n/a**?
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T1-Q5.** Which kept fields are **required** before matching can run for (a) seeker, (b) job? What happens if missing?
  - **Answer:**  
  - **Proof:**  

### [ ] 07-T2 — Search dimensions both sides

**Done when:** [SEARCH-DIMENSIONS.md](SEARCH-DIMENSIONS.md) lists what each side filters/scores, marked hard vs soft.  
**Unlocks / feeds:** Matching-spec weights; Figma filter UI  

#### Sub-questions

- [ ] **07-T2-Q1.** What does a **seeker** search for (dimensions)? Mark each hard / soft / both. Keep/cut/add vs the seed table.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T2-Q2.** What does a **company** search for in people? Same marking.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T2-Q3.** Name **2 asymmetric** cases (dimension on one side only). How will the system evaluate them?
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T2-Q4.** Which dimensions are **beachhead-critical** vs “nice later”? Tie to Gate 1 niche.
  - **Answer:**  
  - **Proof:**  

### [ ] 07-T3 — Acquisition per field

**Done when:** [DATA-ACQUISITION.md](DATA-ACQUISITION.md) covers dictionary fields with method, confidence, legal note, fallback.  
**Unlocks / feeds:** Phase 08 ops; Gate 4  

#### Sub-questions

- [ ] **07-T3-Q1.** Default map: which field groups are **user**, **feed/crawl**, **inferred**, **enrichment**, **computed**? Update the acquisition table.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T3-Q2.** For **inferred** job requirements in bootstrap: what UI label and confidence rule will you use?
  - **Answer:**  
  - **Proof:** (path: product inventory screens MVP-031 / MVP-045)  

- [ ] **07-T3-Q3.** For **salary** and **culture** gaps: enrichment allowed, unknown, or first-party only? No invented numbers.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T3-Q4.** Crawl vs feed: what is primary for MVP listing supply? What is allowlist-only gap-filler?
  - **Answer:**  
  - **Proof:** (path: brief `05-tech-feasibility.md` + your choice)  

- [ ] **07-T3-Q5.** Fallback if a hard-filter field is missing: skip listing, partial match, or block? Per critical field.
  - **Answer:**  
  - **Proof:**  

### [ ] 07-T4 — Matching rules (hard, soft, Top-X, zero-match)

**Done when:** [MATCHING-SPEC.md](MATCHING-SPEC.md) is implementable: filters, scores, thresholds, explainability, zero-match.  
**Unlocks / feeds:** Gate 4; eng handoff  

#### Sub-questions

- [ ] **07-T4-Q1.** List **hard filters** (table: filter, rule, if fail). Include work auth, must languages/skills as applicable to beachhead.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T4-Q2.** List **soft scores** with hypothesized weights and one-line explainability text each. Label weights as **inference** until tested.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T4-Q3.** Define **Top-X** for seekers and for companies, plus **minimum score** to notify / share.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T4-Q4.** **Zero / weak match** behavior in MVP vs V2 (message only vs what-if). Align with Phase 06.
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T4-Q5.** Out of scope for MVP matching — list explicitly.
  - **Answer:**  
  - **Proof:**  

### [ ] 07-T5 — Privacy (commute/home) & fairness

**Done when:** Commute/home handling and fairness constraints are written so product + counsel can review.  
**Unlocks / feeds:** Gate 4; Phase 10 compliance brief  

#### Sub-questions

- [ ] **07-T5-Q1.** How is **home_location** collected, consented, stored, and used? Do employers ever see the raw address?
  - **Answer:**  
  - **Proof:** (path: MATCHING-SPEC + dictionary privacy notes)  

- [ ] **07-T5-Q2.** If the seeker **declines** commute consent, what matching still runs?
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T5-Q3.** Server-side commute: who computes minutes, and what does the company see instead of home?
  - **Answer:**  
  - **Proof:**  

- [ ] **07-T5-Q4.** **Fairness:** which criteria are prohibited or restricted for automated filtering in your beachhead (examples: protected characteristics)? Flag for legal review.
  - **Answer:**  
  - **Proof:** (constraint list — not legal advice)  

- [ ] **07-T5-Q5.** How do you reduce **gaming** or bias on soft culture tags in MVP (avoid / low weight / human confirm)?
  - **Answer:**  
  - **Proof:**  

## Gate / checkpoint pack — Gate 4 (with Phase 06)

- [ ] Human search profile fields complete (type, required, example, privacy)  
- [ ] Company / job requirement fields complete  
- [ ] Search dimensions both sides  
- [ ] Acquisition method per field (+ confidence + legal note + fallback)  
- [ ] Matching: hard/soft, Top-X, thresholds, explainability, zero-match  
- [ ] Commute/home privacy + fairness constraints documented  
- [ ] Dictionary ↔ MVP/V2 screen inventories synced  
- [ ] Engineer can implement without a strategy workshop  

**Daniel only** locks Gate 4 in the decision log.

## Handoff to next phase

Phase 08 (ops) will consume:

- Which fields come from feed vs crawl vs inference (ops load)  
- Freshness needs implied by matching (stale listings hurt trust)  
- Consent/opt-out expectations that ops must support  

Phase 06 Figma must stay synced with final field names and explainability/consent screens.  
