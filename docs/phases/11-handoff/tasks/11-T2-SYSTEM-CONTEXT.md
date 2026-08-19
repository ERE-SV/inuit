# 11-T2 — System context + technical overview

| Field | Value |
| --- | --- |
| **Task ID** | `11-T2` |
| **Phase** | [11-handoff](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [SYSTEM-CONTEXT.md](../SYSTEM-CONTEXT.md) |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

A new engineer needs a short what/why/for whom **and** a technical entry point — not “read the whole repo.” T2 produces the first stop in the Gate 6 walkthrough: product loop plus ingestion/matching architecture pointers.

---

## Our guideline

- **≤5 sentences for the product loop.** Primary value, explicit non-goals — keep it short.
- **One paragraph: matching.** Hard filters, soft scores, Top-X, explainability — from [MATCHING-SPEC.md](../../07-data-matching/MATCHING-SPEC.md).
- **One paragraph: supply / ingestion.** MVP feed/crawl/first-party mix — from Phase 08 + Phase 07 acquisition; link [05-tech-feasibility.md](../../../brief/05-tech-feasibility.md) for subsystem sketch.
- **Pull from locked decisions.** Charter, beachhead, VERSION-MAP — do not invent new scope.
- **MVP / V2 / V3 one line each.** What ships when — from VERSION-MAP. V3 is roadmap unless Gate 6 says otherwise.
- **Gate 1 decision ID.** Beachhead niche × geography with locked decision reference.

---

## What we have done before

**11-T1** — handoff index confirms which gated artifacts exist:

- [11-T1-HANDOFF-INDEX.md](11-T1-HANDOFF-INDEX.md) — artifact paths and gate IDs  

**Gates 1–5** — beachhead, GTM, brand, product scope, matching spec, ops, finance.

---

## What we're doing now

**Goal:** Write SYSTEM-CONTEXT covering product loop, beachhead, version scope, matching, supply, and technical overview pointers.

Example questions — skip what stays thin after an honest pass.

- ≤5 sentences: product loop, primary value, explicit non-goals?
- Beachhead niche × geography + Gate 1 decision ID?
- One line each: MVP / V2 / V3 (what ships)?
- Matching in one paragraph (hard filters, soft scores, Top-X, human confirm)?
- Supply in one paragraph (MVP feeds/API vs crawl + Phase 2/3 direction)?
- Technical overview: link [05-tech-feasibility.md](../../../brief/05-tech-feasibility.md); note ingestion subsystem boundaries and what is **out of MVP build scope** (no production infra in this program).

**Start here**

1. Draft SYSTEM-CONTEXT from locked decisions + brief tech feasibility.  
2. Keep it short — eng orientation, not architecture review.  
3. Link on worksheet.

---

## Why it matters

**For the rest of Phase 11:** [T3](11-T3-MVP-SCOPE.md) details must-build; [T7](11-T7-GATE6-PACK.md) opens the walkthrough here.

**For Daniel:** First stop in Gate 6 — product + technical picture in one place.

**For engineers:** SYSTEM-CONTEXT is the orientation doc before touching Figma or code.
