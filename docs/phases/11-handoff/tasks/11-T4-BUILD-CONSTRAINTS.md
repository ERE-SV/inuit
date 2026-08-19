# 11-T4 — Build constraints

| Field | Value |
| --- | --- |
| **Task ID** | `11-T4` |
| **Phase** | [11-handoff](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [BUILD-CONSTRAINTS.md](../BUILD-CONSTRAINTS.md) |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Finance, ops, beachhead, and privacy **limit** eng choices. Without them, “build everything” returns. T4 translates Gates 1–5 and Phase 10 into hard build limits engineers can follow.

---

## Our guideline

- **Point at Gate 5 artifacts.** Budget/run-cost envelope from finance — no invented CHF; cite Gate 5 or `unknown`.
- **≥2 out-of-bounds choices.** Wrong cloud region, raw home on employer UI, unbounded crawl — name concrete limits.
- **Constraints are product/eng limits.** Not legal advice — privacy limits come from compliance brief as build rules.
- **Pull from Phases 08–10.** Ingestion headcount, beachhead-only scope, privacy/home-commute rules.
- **Implication column.** Each constraint should say what it means for build decisions.

---

## What we have done before

**Phase 08–10** — ops, finance, and risk limits:

- [09-finance](../../09-finance/README.md) — run-cost envelope from Gate 5  
- [08-ops](../../08-ops/README.md) — ingestion headcount and supply approach  
- [10-risk](../../10-risk/README.md) — privacy, crawl, matching constraints from compliance brief  

**Gate 1** — beachhead-only scope boundary.

---

## What we're doing now

**Goal:** Document build constraints from finance, ops, beachhead, and privacy — with ≥2 explicit out-of-bounds implementation choices.

Example questions — skip what stays thin after an honest pass.

- Constraints from budget/run-cost (Phase 09), ingestion headcount (Phase 08), beachhead-only (Gate 1), privacy/home-commute (Phase 10)?
- ≥2 implementation choices that are **out of bounds** (e.g. wrong cloud region, raw home on employer UI, unbounded crawl)?

You might use this shape:

| Constraint | Source | Implication for build |
| --- | --- | --- |
| Budget / run-cost envelope | Phase 09 |  |
| Headcount for ingestion | Phase 08 |  |
| Beachhead-only scope | Gate 1 |  |
| Privacy (home/commute) | Phase 10 |  |

**Start here**

1. Pull from Phases 08–10 + Gate 1.  
2. Add ≥2 out-of-bounds choices.  
3. Link on worksheet.

---

## Why it matters

**For the rest of Phase 11:** [T7](11-T7-GATE6-PACK.md) includes constraints in walkthrough; [T6](11-T6-CHECKLIST.md) verifies they're filled.

**For Daniel:** BUILD-CONSTRAINTS on Gate 6 pack — eng can't claim they weren't told the limits.

**For engineers:** Hard out-of-bounds list prevents expensive wrong turns on day one.
