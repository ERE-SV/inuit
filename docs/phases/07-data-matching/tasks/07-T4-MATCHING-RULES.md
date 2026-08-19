# 07-T4 — Matching rules (hard, soft, Top-X, zero-match)

| Field | Value |
| --- | --- |
| **Task ID** | `07-T4` |
| **Phase** | [07-data-matching](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [MATCHING-SPEC.md](../MATCHING-SPEC.md) · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Gate 4 needs an implementable matching spec: hard filters, soft scores, Top-X, thresholds, explainability, and zero-match — aligned with Phase 06 product behavior.

---

## Our guideline

- **Implementable tables.** Hard filters (filter, rule, if fail); soft scores with weights and one-line explainability each.
- **Label weights as inference** until tested — honest hypotheses, not fake precision.
- **Top-X both ways.** Short ranked lists for seekers and companies, plus minimum score to notify / share.
- **Zero-match aligned with product.** MVP message-only vs V2 what-if must match Phase 06 screen placement.
- **Explicit MVP out-of-scope.** List matching behaviors deferred — vague “later” is not a spec.
- **No undefined culture fit.** Soft culture tags without definition → bias risk (see [T5](07-T5-PRIVACY-FAIRNESS.md)).

| Term | Plain meaning |
| --- | --- |
| **Top-X** | Short ranked list above a threshold |
| **Explainability** | Short “why this match” (criteria hit/miss) |

---

## What we have done before

Build on dimensions, acquisition, and product behavior:

- [07-T2 — Search dimensions](07-T2-SEARCH-DIMENSIONS.md) — hard/soft dimensions, asymmetries, beachhead-critical set
- [07-T3 — Acquisition](07-T3-ACQUISITION.md) — missing-field fallbacks for hard filters
- [07-T1 — Dictionary](07-T1-DICTIONARY.md) — field set matching rules reference
- [MATCHING-SPEC.md](../MATCHING-SPEC.md) — seeded spec stub
- [Phase 06 — product](../../06-product/README.md) — empty-match screen placement ([06-T3](../../06-product/tasks/06-T3-MVP-INVENTORY.md)), indicator-not-guarantee copy ([06-T1](../../06-product/tasks/06-T1-VERSIONS-JOURNEYS.md))
- [decisions/DECISION-LOG.md](../../../../decisions/DECISION-LOG.md) — scope checkpoint MVP feature set (which matching behaviors are in)

---

## What we're doing now

**Goal:** Write hard filters, soft scores, Top-X thresholds, explainability, zero-match behavior, and MVP out-of-scope list in MATCHING-SPEC.

Example questions:

- List **hard filters** (filter, rule, if fail). Include work auth, must languages/skills as applicable to the beachhead.
- List **soft scores** with hypothesized weights and one-line explainability text each. Label weights as **inference** until tested.
- Define **Top-X** for seekers and for companies, plus **minimum score** to notify / share.
- **Zero / weak match** behavior in MVP vs V2 (message only vs what-if). Align with Phase 06.
- Out of scope for MVP matching — list explicitly.

You might write tables in MATCHING-SPEC — preferred.

**Start here**

1. Dimensions from 07-T2 + Phase 06 empty-match placement.  
2. Hard filters → soft scores → Top-X / thresholds → zero-match.  
3. Explicit MVP out-of-scope list.  
4. Link from the worksheet.  

---

## Why it matters

**For the rest of Phase 07:** [T5](07-T5-PRIVACY-FAIRNESS.md) adds commute/home and fairness constraints that may affect hard filters and explainability.

**For Daniel:** [MATCHING-SPEC.md](../MATCHING-SPEC.md) ready for **Gate 4** — engineer can implement without a strategy workshop.

**For later phases:** Phase 06 explainability and match UI must display what this spec defines; Phase 10 compliance builds on fairness flags from T5.
