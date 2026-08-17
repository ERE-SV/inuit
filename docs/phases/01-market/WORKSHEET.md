# Phase 01 — Market & category — Worksheet

**Status:** not-started  
**Unlocks:** Phase 02 competitive teardown; facts for Phase 03 beachhead scoring (Gate 1)  
**Primary path:** this file  

## Learn (read before working)

### What this phase is

You map how the Swiss job market actually works today — which channels people and companies use, what is changing, where demand and supply look strong or weak by segment, and which legal/product rules constrain matching, crawling, and commute features. You are collecting **evidence**, not picking a niche yet. Start from [SOURCES-STARTER.md](SOURCES-STARTER.md); log every source you use in [SOURCES.md](SOURCES.md).

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Channel** | A place where jobs are posted or found (portal, LinkedIn, career site, RAV, agency) | Niche choice depends on where volume and pain already live |
| **Demand (employer side)** | Companies needing to hire — openings, hard-to-fill roles | Beachhead needs enough paid hiring pain |
| **Supply (seeker side)** | People looking or open to roles | Matching needs enough candidates in the same niche × place |
| **Liquidity** | Enough relevant openings *and* seekers so matches happen often | Without liquidity, a marketplace feels empty |
| **So what** | One sentence: what a fact means for *this* product | Stops you collecting trivia that does not change decisions |
| **nDSG / GDPR** | Swiss (and EU) privacy rules for personal data | Commute, profiles, and auto-scores have legal constraints |
| **Inference** | Your conclusion from facts, not a fact itself | Must be labeled so Daniel can trust the evidence trail |

### Common beginner mistakes

- Writing a long essay with no URLs or access dates  
- Claiming portal prices or “talent shortage” without a source (use `unknown` or skip)  
- Listing trends with no “so what” for matchmaking / less-noise hiring  
- Ignoring public channels (`arbeit.swiss` / RAV) and company career pages  
- Treating regulatory notes as legal advice instead of **product constraints to flag for counsel**  
- Jumping to “our beachhead should be X” before Phases 02–03  

## How to prove answers

- Factual claim → URL + access date OR path under this phase folder / `evidence/`  
- Label inferences as **inference**  
- Flexible formats OK: md, table, chart image, PDF, video link — record path in Proof  
- Prefer Tier A/B sources; follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)  
- Keep a running log in [SOURCES.md](SOURCES.md)

## Tasks

### [ ] 01-T1 — Swiss hiring channels map

**Done when:** You have a filled channels table covering seekers *and* employers for the main CH (+ relevant DACH) paths.  
**Unlocks / feeds:** Phase 02 competitor list; Phase 03 volume/geography judgment  

#### Sub-questions

- [ ] **01-T1-Q1.** Which channels from [SOURCES-STARTER.md](SOURCES-STARTER.md) did you open and document (list name + URL)?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T1-Q2.** For each major portal you visited (at least jobs.ch, Indeed CH, LinkedIn, plus 2 more of your choice), what is the **seeker** job vs the **employer** job of that channel in one sentence each?
  - **Answer:**  
  - **Proof:** (path to your channels table, e.g. `MARKET-BRIEF.md` or `evidence/channels-map.md`)  

- [ ] **01-T1-Q3.** What public pricing (if any) is shown for employer products on those portals? If not public, write `unknown` — do not invent CHF numbers.
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T1-Q4.** How do **company career pages** and **public employment** (arbeit.swiss / RAV) fit into the map — when would a seeker or employer use them instead of a big portal?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T1-Q5.** In 3–5 bullets: how does multi-channel posting create cost or noise for employers? (Facts + **inference** labeled.)
  - **Answer:**  
  - **Proof:**  

### [ ] 01-T2 — Labour-market trends with “so what”

**Done when:** At least 4 trend claims each have a source and a product-relevant “so what.”  
**Unlocks / feeds:** Positioning later; beachhead pain criteria  

#### Sub-questions

- [ ] **01-T2-Q1.** What do official stats (BFS / opendata.swiss or similar) say about employment / unemployment / sector hiring that is relevant to a CH job marketplace? Summarize in ≤5 bullets.
  - **Answer:**  
  - **Proof:** (URL — accessed YYYY-MM-DD)  

- [ ] **01-T2-Q2.** What evidence exists (sourced) about apply volume, unqualified applications, or AI-generated applications / cover letters? If weak, say so.
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T2-Q3.** Skills-based hiring or structured requirements — what is changing, and **so what** for bidirectional matching (not keyword search alone)?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T2-Q4.** Salary / compensation transparency or benchmarking in CH — what can you source, and **so what** for company profiles and seeker salary floors?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T2-Q5.** Pick one more trend you judge important for *this* product. State fact → **so what** → implication if the trend is wrong (**inference**).
  - **Answer:**  
  - **Proof:**  

### [ ] 01-T3 — Demand and supply by segment

**Done when:** You can compare at least 3 candidate segments (see brief niches) on openings + candidates with citations.  
**Unlocks / feeds:** Phase 03 scorecard liquidity rows  

#### Sub-questions

- [ ] **01-T3-Q1.** Which segments will you compare? Include at least three from the brief shortlist (e.g. specialized IT/consultants, Zurich bankers, healthcare/nurses, trades) or justify substitutes.
  - **Answer:**  
  - **Proof:** (reference [docs/brief/03-gtm-niche.md](../../brief/03-gtm-niche.md) + your choice rationale)  

- [ ] **01-T3-Q2.** For each segment: what **demand** signals can you find (openings volume, shortage reports, industry associations)? Use `unknown` where missing.
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T3-Q3.** For each segment: what **supply** signals can you find (graduates, job-seeker pools, network size proxies)? Use `unknown` where missing.
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T3-Q4.** Where is hiring geographically concentrated for each segment (city / canton / remote)? What does that imply for a Zurich-first vs CH-wide start? (**inference** OK if labeled.)
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T3-Q5.** Which segment looks strongest on *liquidity* vs strongest on *pain / cost of bad hire*? One sentence each — you are not locking a beachhead yet.
  - **Answer:**  
  - **Proof:**  

### [ ] 01-T4 — Regulatory and product constraints checklist

**Done when:** Every item in the starter regulatory checklist has a note (constraint + implication + open legal question).  
**Unlocks / feeds:** Phase 07 data/matching; Phase 10 compliance; crawl/commute design  

#### Sub-questions

- [ ] **01-T4-Q1.** Processing candidate profiles for matching — purpose limitation: what must the product be able to explain to a user in plain language?
  - **Answer:**  
  - **Proof:** (official nDSG / FDPIC or GDPR page — accessed YYYY-MM-DD)  

- [ ] **01-T4-Q2.** Home address / commute calculation — what consent, minimization, and “employers don’t see raw home address” constraints should we assume until counsel reviews?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T4-Q3.** Automated “fit” scores and notifications — what transparency / human-in-the-loop expectations should we flag?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T4-Q4.** Scraping or reusing third-party listings — what ToS / robots.txt / opt-out issues did you find for at least two sources? (Flag for counsel; do not invent legality.)
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T4-Q5.** Cross-border CH/EU data — when would this product likely touch EU rules, and what should we mark as “needs legal review before build”?
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T4-Q6.** Complete the checklist from [SOURCES-STARTER.md](SOURCES-STARTER.md) (tick there or paste status here) and list any extra constraints you discovered.
  - **Answer:**  
  - **Proof:**  

### [ ] 01-T5 — Sources log and brief quality pass

**Done when:** [SOURCES.md](SOURCES.md) lists every URL used this phase with access dates; quantitative claims are checkable.  
**Unlocks / feeds:** Credibility for Gate 1 pack later  

#### Sub-questions

- [ ] **01-T5-Q1.** Did you open 5–8 Tier A sources before leaning on press/blogs? List them.
  - **Answer:**  
  - **Proof:** ([SOURCES.md](SOURCES.md))  

- [ ] **01-T5-Q2.** Are there any numbers in your answers still without URL + access date? Fix or delete them. Confirm with yes/no + list of fixed items.
  - **Answer:**  
  - **Proof:**  

- [ ] **01-T5-Q3.** Optional dump: if you wrote a long narrative, path to [MARKET-BRIEF.md](MARKET-BRIEF.md) or `evidence/` — worksheet answers still must stand alone.
  - **Answer:**  
  - **Proof:**  

## Gate / checkpoint pack (if any)

No formal gate this phase. For the weekly with Daniel, bring:

- [ ] Channels map path filled in 01-T1  
- [ ] Trend table with “so what” (01-T2)  
- [ ] Segment demand/supply comparison (01-T3)  
- [ ] Regulatory checklist status (01-T4)  
- [ ] Updated [SOURCES.md](SOURCES.md)  

## Handoff to next phase

Phase 02 will consume:

- Your channels map (who is a “direct” vs “adjacent” competitor)  
- Segment names and volume/pain signals for competitor niche boards and agencies  
- Regulatory flags that affect positioning claims (privacy, crawl, auto-score honesty)  
- Source list patterns (keep the same citation discipline)
