# 07-T2 — Search dimensions both sides

| Field | Value |
| --- | --- |
| **Task ID** | `07-T2` |
| **Phase** | [07-data-matching](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [SEARCH-DIMENSIONS.md](../SEARCH-DIMENSIONS.md) · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Matching weights and Figma filter UI need a clear list of what each side filters or scores — hard vs soft — tied to the beachhead.

---

## Our guideline

- **Hard vs soft explicitly.** Hard = must-pass (fail → not shown / not ranked). Soft = rank adjustment after hard filters pass.
- **Don’t hard-filter everything.** Treating every preference as a hard filter kills liquidity.
- **Flag asymmetries.** When one side cares about a dimension the other doesn’t store (e.g. commute), say how the system evaluates it.
- **Beachhead-critical vs later.** Tie dimensions to Gate 1 niche so MVP stays focused.
- **Update the seed file.** Prefer editing [SEARCH-DIMENSIONS.md](../SEARCH-DIMENSIONS.md) directly.

| Term | Plain meaning |
| --- | --- |
| **Hard filter** | Must-pass (fail → not shown / not ranked) |
| **Soft score** | Raises/lowers rank when hard filters pass |
| **Asymmetric preference** | One side cares about a dimension the other doesn’t store (e.g. commute) |

---

## What we have done before

Build on the decided dictionary from T1:

- [07-T1 — Dictionary keep/cut/add](07-T1-DICTIONARY.md) — kept fields, required-before-match, privacy notes
- [DATA-DICTIONARY.md](../DATA-DICTIONARY.md) — field set dimensions map to
- [SEARCH-DIMENSIONS.md](../SEARCH-DIMENSIONS.md) — seeded dimension table
- [decisions/DECISION-LOG.md](../../../../decisions/DECISION-LOG.md) — **Gate 1** niche × geography
- [Phase 03 — beachhead](../../03-beachhead/README.md) — which criteria matter for the locked wedge

---

## What we're doing now

**Goal:** List seeker and company search dimensions, mark hard/soft/both, note asymmetries, and flag beachhead-critical vs later.

Example questions:

- What does a **seeker** search for (dimensions)? Mark each hard / soft / both. Keep/cut/add vs the seed table.
- What does a **company** search for in people? Same marking.
- Name a couple of **asymmetric** cases (dimension on one side only). How will the system evaluate them?
- Which dimensions are **beachhead-critical** vs “nice later”? Tie to Gate 1 niche.

**Start here**

1. Open SEARCH-DIMENSIONS + Gate 1 niche.  
2. Mark hard/soft; note asymmetries and how they evaluate.  
3. Flag beachhead-critical vs later.  
4. Link from the worksheet.  

---

## Why it matters

**For the rest of Phase 07:** [T4](07-T4-MATCHING-RULES.md) hard filters and soft scores come from this list. [T3](07-T3-ACQUISITION.md) may need extra fields for asymmetric dimensions (e.g. computed commute).

**For Daniel:** Dimension list for MATCHING-SPEC and filter UI — beachhead-critical vs later so MVP scope stays defensible.

**For later phases:** Phase 06 filter UI and explainability copy must reflect dimensions marked hard vs soft here.
