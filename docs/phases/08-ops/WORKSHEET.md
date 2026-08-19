# Phase 08 — Supply & operations — Worksheet

**Status:** not-started  
**Unlocks:** **Ops checkpoint** (Weeks 10–11) — assumptions accepted as **inputs to the financial model** (Phase 09), not a forever org chart  
**Depends on:** Beachhead, GTM, data acquisition approach (Phase 07)  
**Owner:** Malte  
**Primary path:** this file  

## How this file works

This is **progress tracking**, not an exam. Tick **Ready** when you can talk about that area in the weekly. Put notes wherever you like and paste the path under **Your notes**.

Read [task files](tasks/README.md) for context and example questions. Each brief has the same thread: **why it exists → guideline → what came before → what we're doing now → why it matters.**

Facts that matter (volumes, prices, legal claims) need a URL + access date or `unknown`. Label guesses as **inference**. See [WORKSHEET-GUIDE.md](../WORKSHEET-GUIDE.md) and [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md).

## Learn (read before working)

### What this phase is

Explain how **job listings get into the product** and how many people (and tools) it takes to keep supply fresh and sell/support the beachhead. Output feeds finance: cost drivers, headcount timing, and what one person can run alone.

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Freshness** | How recently a listing was checked/updated | Stale jobs destroy seeker trust |
| **Allowlist** | Sites/employers you may crawl | Compliance-by-design |
| **Lineage** | Source URL, fetch time, parser version | Debugging + trust labels |
| **Headcount plan** | Who you hire, when, for which milestone | Finance opex |
| **Cost driver** | Something that makes spend rise with volume | Phase 09 model inputs |

### What to avoid

- Assuming crawl is free (legal + engineer time)  
- Planning a large ops team before MVP liquidity  
- Sales headcount that ignores GTM forward-motion  
- No measurable hiring trigger  
- Inventing CHF vendor costs  

Optional dumps: [OPS-MODEL.md](OPS-MODEL.md), [HEADCOUNT-PLAN.md](HEADCOUNT-PLAN.md).

## Progress

| Task | Focus | Task file | Your notes | Ready |
| --- | --- | --- | --- | --- |
| **08-T1** | Supply approaches | [08-T1-SUPPLY-APPROACHES.md](tasks/08-T1-SUPPLY-APPROACHES.md) |  | [ ] |
| **08-T2** | Ops model / freshness | [08-T2-OPS-MODEL.md](tasks/08-T2-OPS-MODEL.md) |  | [ ] |
| **08-T3** | Headcount shape | [08-T3-HEADCOUNT.md](tasks/08-T3-HEADCOUNT.md) |  | [ ] |
| **08-T4** | Hiring triggers | [08-T4-HIRING-TRIGGERS.md](tasks/08-T4-HIRING-TRIGGERS.md) |  | [ ] |
| **08-T5** | Cost drivers | [08-T5-COST-DRIVERS.md](tasks/08-T5-COST-DRIVERS.md) |  | [ ] |

## Gate / checkpoint pack — Ops checkpoint

Daniel accepts as **finance inputs** (not eternal org design):

- [ ] Listing supply approach (feeds/APIs vs crawl) + legal posture summary  
- [ ] Freshness / quality assumptions  
- [ ] Headcount: ingestion — how many, when, skills  
- [ ] Headcount: sales — how many, when, motion link to GTM  
- [ ] Support / other roles if needed for MVP  
- [ ] What one person can run vs when to hire #2  
- [ ] Cost drivers listed for Phase 09  

Only Daniel accepts the checkpoint as model inputs.

## Handoff

**Phase 09** consumes: supply cost drivers and unit drivers; headcount timing; freshness assumptions that affect retention/churn hypotheses.

**Phase 10** consumes: crawl/ToS legal posture flags; single-person bus factor on ingestion.

Update [STATUS.md](../../../STATUS.md) when the checkpoint is accepted.
