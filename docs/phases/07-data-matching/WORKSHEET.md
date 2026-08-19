# Phase 07 — Data profiles, acquisition & matching — Worksheet

**Status:** not-started  
**Unlocks:** Data v0 with product scope (Week 7); depth Weeks 8–11 (parallel to Figma); **Gate 4** Week 12 with Phase 06  
**Depends on:** Product scope (align with Phase 06); beachhead from Gate 1  
**Seeded start:** [DATA-DICTIONARY.md](DATA-DICTIONARY.md), [SEARCH-DIMENSIONS.md](SEARCH-DIMENSIONS.md), [DATA-ACQUISITION.md](DATA-ACQUISITION.md)  

## How this file works

This is **progress tracking**, not an exam. Tick **Ready** when you can talk about that area in the weekly. Put notes wherever you like and paste the path under **Your notes**.

Read [task files](tasks/README.md) for context and example questions. Each brief has the same thread: **why it exists → guideline → what came before → what we're doing now → why it matters.**

Decide keep/cut/add and write specs in the seeded stubs (or elsewhere). Do **not** fill Answer/Proof slots here or in the task files. Dictionary keep/cut/add is **inspiration for deciding** — update the dictionary itself, not a form on this page. Cite sources when external claims matter ([RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)).

## Learn (orientation)

### What this phase is

Define **what data exists**, **where it comes from**, and **how matching uses it** so an engineer can implement without a strategy workshop. Both sides have a **search profile**. Start from the seeded dictionary — mark **keep / cut / add** — then specify acquisition, dimensions, hard vs soft rules, privacy, and fairness.

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Search profile** | Structured preferences + constraints to find the other side | Same idea both sides |
| **Hard filter** | Must-pass rule | Commute max, work auth, must-have language |
| **Soft score** | Weighted preference after hard filters | Nice-to-have skills, culture tags |
| **Acquisition method** | User, feed/API, crawl, enrichment, inferred, computed | Confidence + legal notes differ |
| **Inferred** | Derived (e.g. from job text), not typed by employer | Must be labeled; lower confidence |
| **Top-X** | Short ranked list above a threshold | Fewer, better — not infinite inbox |
| **Explainability** | Short “why this match” | Trust; not a black-box score |
| **Asymmetric preference** | One side cares; the other doesn’t store it | Needs geo + computation (e.g. commute) |
| **Fairness / prohibited criteria** | Rules you will not automate or will constrain | Legal + brand trust |

### Common mistakes

- Every preference as a hard filter (liquidity dies)  
- Inventing salary or culture facts  
- Sending raw home address to employers  
- Soft “culture fit” with no definition  
- Dictionary fields no MVP screen collects  
- Matching spec an engineer cannot implement  
- Skipping fairness / prohibited automated criteria  

## Progress

| Task | Focus | Task file | Your notes | Ready |
| --- | --- | --- | --- | --- |
| **07-T1** | Search profiles & dictionary keep/cut/add | [07-T1-DICTIONARY.md](tasks/07-T1-DICTIONARY.md) | | [ ] |
| **07-T2** | Search dimensions both sides | [07-T2-SEARCH-DIMENSIONS.md](tasks/07-T2-SEARCH-DIMENSIONS.md) | | [ ] |
| **07-T3** | Acquisition per field | [07-T3-ACQUISITION.md](tasks/07-T3-ACQUISITION.md) | | [ ] |
| **07-T4** | Matching rules | [07-T4-MATCHING-RULES.md](tasks/07-T4-MATCHING-RULES.md) | | [ ] |
| **07-T5** | Privacy (commute/home) & fairness | [07-T5-PRIVACY-FAIRNESS.md](tasks/07-T5-PRIVACY-FAIRNESS.md) | | [ ] |

## Gate / checkpoint pack — Gate 4 (Week 12; with Phase 06)

- [ ] Human search profile fields complete (type, required, example, privacy)  
- [ ] Company / job requirement fields complete  
- [ ] Search dimensions both sides  
- [ ] Acquisition method per field (+ confidence + legal note + fallback)  
- [ ] Matching: hard/soft, Top-X, thresholds, explainability, zero-match  
- [ ] Commute/home privacy + fairness constraints documented  
- [ ] Dictionary ↔ MVP/V2 screen inventories synced (checkpoint Week 10)  
- [ ] Engineer can implement **MVP (+ gated V2)** without a strategy workshop  

**Gate 4 product scope:** MVP + V2 build-ready Figma; V3 directional only.

**Daniel only** locks Gate 4 in the decision log.

## Handoff to next phase

Phase 08 (ops) will consume:

- Which fields come from feed vs crawl vs inference (ops load)  
- Freshness needs implied by matching (stale listings hurt trust)  
- Consent/opt-out expectations that ops must support  

Phase 06 Figma must stay synced with final field names and explainability/consent screens.  
