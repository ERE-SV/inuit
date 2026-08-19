# 08-T1 — Supply approaches for this product

| Field | Value |
| --- | --- |
| **Task ID** | `08-T1` |
| **Phase** | [08-ops](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | Notes, slides, or a short memo — optional dump [OPS-MODEL.md](../OPS-MODEL.md) |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Finance and eng need a clear story of how listings get into the product before every employer has a profile. Feed vs crawl vs first-party changes cost, legal risk, and headcount. T1 is the **foundation** for the ops checkpoint — without a coherent supply mix, later headcount and cost work is guesswork.

---

## Our guideline

- **Synthesize Phase 07.** Read [07-T3 acquisition table](../../07-data-matching/tasks/07-T3-ACQUISITION.md) — name primary/secondary **mix**, do not redo per-field methods.
- **Name the mix honestly.** Primary vs secondary approach for MVP; when first-party becomes dominant.
- **Plain language.** Define ingestion, feed/API, crawl, and first-party for *this* product — not textbook definitions.
- **Flag legal and QA cost.** Crawl is not free; inferred fields need labeling and support paths.
- **Do not lock finance yet.** This is input for the ops checkpoint Daniel accepts — not eternal architecture.

---

## What we have done before

**Phase 07** — data & matching acquisition approach:

- [07-data-matching](../../07-data-matching/README.md) — feeds, crawl posture, matching inputs  
- Locked beachhead (Gate 1) and GTM motion (Gate 2) — who you sell to affects first-party timing  

Treat Phase 07 notes as hypotheses to refine, not answers to copy.

---

## What we're doing now

**Goal:** Sketch how listings get into the MVP product — primary and secondary supply approaches, with plain-language tradeoffs.

Example questions — skip what stays thin after an honest pass.

- In your own words: what are **ingestion**, **feed/API**, and **crawl** for *this* product?
- For the MVP beachhead: what is the **primary** listing supply approach, and what is **secondary**? Why?
- When do **first-party** employer profiles become the main path (GTM stage / product Phase 2)?
- What does “label inferred requirements” mean for ops (QA, support, employer complaints)?

You might sketch a comparison if helpful:

| Approach | Plain meaning | Pros | Cons |
| --- | --- | --- | --- |
| **Feed / API** | Provider sends structured job data | Fresher, clearer rights | Cost, quotas, negotiation |
| **Crawl** | Visit career pages (allowlist), extract | Fills gaps early | Breaks; ToS/robots risk; babysitting |
| **First-party** | Employer enters or pushes jobs | Highest trust | Needs sales/onboarding |
| **Inferred fields** | LLM/rules structure free text | Unlocks matching early | Lower confidence; QA cost |

**Ingestion** = discover → fetch → extract/normalize → QA → publish with lineage.

**Start here**

1. Read worksheet Learn (ingestion table).  
2. Skim Phase 07 acquisition + GTM motion.  
3. Sketch primary/secondary supply; link notes on the worksheet.

---

## Why it matters

**For the rest of Phase 08:** [T2](08-T2-OPS-MODEL.md) needs your supply mix for freshness and legal posture. [T3](08-T3-HEADCOUNT.md) and [T5](08-T5-COST-DRIVERS.md) depend on crawl vs feed cost profiles.

**For Daniel:** A coherent MVP mix he can accept as a finance input at the ops checkpoint.

**For later phases:** Phase 10 (crawl/ToS) and Phase 09 (cost drivers) start from this story.
