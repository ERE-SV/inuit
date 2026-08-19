# 10-T1 — Privacy (product implications)

| Field | Value |
| --- | --- |
| **Task ID** | `10-T1` |
| **Phase** | [10-risk](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [COMPLIANCE-BRIEF.md](../COMPLIANCE-BRIEF.md) or your own notes |

This file is **context and inspiration**. Do not fill it in.

You are **not** a lawyer. Produce product implications + open counsel questions — not fake legal certainty.

---

## Why this exists

Matching, commute, and profiles touch personal data. Engineers need constraints; counsel needs a clear question list. T1 starts the compliance brief with product-facing privacy implications — not legal opinions.

---

## Our guideline

- **Synthesize Phase 07.** Start from [07-T5 privacy & fairness](../../07-data-matching/tasks/07-T5-PRIVACY-FAIRNESS.md) — add counsel questions, do not rewrite product flows.
- **Product implications, not legal advice.** What eng must build vs what counsel must answer.
- **Minimize and label.** Required vs optional vs deferred fields; inferred fields labeled in UI.
- **Commute without exposing home.** Server-side matching can keep raw home off employer UI — say how.
- **Cite or mark unknown.** Official pages or `unknown — counsel`. Never invent Swiss law quotes.
- **≥3 counsel questions.** Only DPO/counsel should answer these — list them explicitly.

---

## What we have done before

**Gates 1–5** — product concept, matching spec, monetization, and ops model define what data MVP needs.

**Phase 06–07** — product and data/matching specs:

- Data dictionary / matching concept — which fields exist and why  
- Phase 08 supply model — raw crawl vs derived fields  

**Brief inputs:** [05-tech-feasibility.md](../../../brief/05-tech-feasibility.md) — hypotheses to test.

---

## What we're doing now

**Goal:** Document MVP personal data types, product privacy constraints, and open counsel questions.

Example questions — skip what stays thin after an honest pass.

- Which personal data types does MVP need? Mark required / optional / deferred.
- How does commute matching work **without** employers seeing raw home address? What consent seems required?
- What can employers see by default? Retention idea for **raw crawl** vs **derived** fields (`TBD with counsel` OK)?
- How are inferred fields labeled? Correction / claim / opt-out in one sentence each?
- ≥3 open privacy questions only counsel/DPO should answer?

**Start here**

1. Skim data dictionary / product concept for fields.  
2. Draft implications + counsel questions.  
3. Link on worksheet.

---

## Why it matters

**For the rest of Phase 10:** [T7](10-T7-COMPLIANCE-BRIEF.md) folds T1 into the compliance brief. [T4](10-T4-RISK-REGISTER.md) gets privacy rows.

**For Daniel:** Privacy constraints explicit before Gate 6 — not “we'll fix later.”

**For later phases:** Phase 11 [BUILD-CONSTRAINTS.md](../../11-handoff/BUILD-CONSTRAINTS.md) and [OPEN-QUESTIONS-FOR-ENG.md](../../11-handoff/OPEN-QUESTIONS-FOR-ENG.md) consume this.
