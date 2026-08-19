# 11-T1 — Handoff index (gated artifacts)

| Field | Value |
| --- | --- |
| **Task ID** | `11-T1` |
| **Phase** | [11-handoff](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | Index in [README.md](../README.md) or HANDOFF-CHECKLIST |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Engineers should not dig through chat. Every major gated artifact needs a path, gate ID, and honest OK/blocker status. T1 is the **entry point** for the Gate 6 walkthrough — one index Daniel can scan in minutes.

---

## Our guideline

- **Honest status.** Link empty stubs as “OK” fails Gate 6 — mark blocker + owner instead.
- **Every gate represented.** Beachhead through risk — path, gate ID, status.
- **Decision log included.** Gates 1–6 decision IDs verifiable from the index.
- **Name blockers with owners.** What is blocked and who must finish before Gate 6?
- **Do not self-approve.** Prepared index ≠ accepted handoff.

---

## What we have done before

**Gates 1–5** — locked artifacts across phases 03–09:

- Beachhead, GTM, brand, product/Figma, data & matching, ops checkpoint, finance  

**Phase 10** — risk pack in progress for Gate 6 inputs:

- [10-risk](../../10-risk/README.md) — RISK-REGISTER, COMPLIANCE-BRIEF, ASSUMPTIONS, KILL-CRITERIA  

---

## What we're doing now

**Goal:** Build a single index of all gated artifacts with path, gate ID, and OK/blocker status.

Example questions — skip what stays thin after an honest pass.

- Status for beachhead, GTM, brand, product/Figma, data & matching, ops, finance, risk, decision log — path, gate, OK?
- If any row is not OK: what is blocked and who must finish it before Gate 6?

You might use this shape:

| Topic | Path | Gate | Status OK? |
| --- | --- | --- | --- |
| Beachhead | `../03-beachhead/` | 1 |  |
| GTM | `../04-gtm/` | 2 |  |
| Brand | `../05-brand/` | 3 |  |
| Product / Figma | `../06-product/` | 4 (+ V3) |  |
| Data & matching | `../07-data-matching/` | 4 |  |
| Ops | `../08-ops/` | checkpoint |  |
| Finance | `../09-finance/` | 5 |  |
| Risk | `../10-risk/` | 6 input |  |
| Decisions | `/decisions/DECISION-LOG.md` | 1–6 |  |

**Start here**

1. Walk each folder; check decision log IDs.  
2. Mark OK or blocker+owner.  
3. Link index on worksheet.

---

## Why it matters

**For the rest of Phase 11:** [T6](11-T6-CHECKLIST.md) and [T7](11-T7-GATE6-PACK.md) use this index for the Gate 6 walkthrough order.

**For Daniel:** Single index for Gate 6 — honest gaps before accept.

**For engineers:** After Gate 6, this index is how they find every locked artifact without re-asking strategy.
