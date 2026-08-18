# Charter — Company definition (Malte)

## Purpose

Turn the job-marketplace idea (see `docs/brief/`) into a **complete, evidence-based company definition** so engineering can build from Figma + specs without rediscovering strategy.

This repo is the **deliverable** and the **source of truth**. Chat is ephemeral; decisions and artifacts land here.

## Roles


| Role       | Responsibility                                                                                        |
| ---------- | ----------------------------------------------------------------------------------------------------- |
| **Daniel** | Approves gates; co-owns strategy in weekly sessions; final accept of handoff pack                     |
| **Malte**  | Owns research, proposals, phase folders, Figma, models; documents everything here; proposes decisions; **updates [STATUS.md](STATUS.md) after every weekly** |




## Scope (in)

1. Market & category (sourced)
2. Competitive landscape
3. Beachhead (niche × geography)
4. Go-to-market
5. Brand principles (lean but binding for UI)
6. Product concept + **full Figma UI/functionality** for **MVP, V2, and V3**
7. Data model + acquisition + matching specification
8. Ops / headcount model (crawlers, sales, support, run costs inputs)
9. Monetization & financial projections to milestones
10. Risk, compliance, assumptions
11. Engineering handoff pack in `docs/phases/11-handoff/`



## Scope (out)

- Coded frontend or backend
- Production infrastructure
- Live crawling or signed vendor contracts (due diligence OK; execution later)
- Closing real customers (design the motion; do not run a sales org yet)



## Research standard

- **Desk-first, fact-based:** public data, reports, pricing pages, filings, job-volume proxies — with **citations** (URL + access date).
- Full rules: [RESEARCH-STANDARD.md](RESEARCH-STANDARD.md).
- Interviews are optional and light; they are not the primary evidence base.
- Unsupported claims do not pass a gate.



## Working model

- **Decision-first spiral:** lock beachhead → GTM → brand principles → then deep product UI and data/matching → ops → finance → risk → handoff.
- **One weekly working session** (Malte leads, **60 min max**): informed discussion of findings after T-24 upload; Malte proposes 2–3 decisions with pros/cons; **Daniel chooses**.
- **Formal gates** for milestone locks happen **in that same weekly slot** (Malte proposes, Daniel decides). No extra review or gate meetings.
- Every material decision → [decisions/DECISION-LOG.md](decisions/DECISION-LOG.md).



## Success criteria (end of program)

1. Beachhead, GTM shape, and brand principles are **gated and logged**.
2. Figma covers **MVP + V2 + V3** with annotated functionality and states.
3. Data & matching specs are implementable by an engineer without a strategy call.
4. Finance model shows costs, revenue mechanics, and projections to named milestones.
5. `docs/phases/11-handoff/` is a single entry point an engineer can follow.
6. Repo is consistent: phase statuses, decision log, and meeting minutes match reality.



## Timeline

**16 weeks total:** **14 weeks** planned work + **2 weeks buffer** (slip, rework after gates, or deepen weak evidence). See [PLAN.md](PLAN.md) and day-to-day [PLAN-WEEKS.md](PLAN-WEEKS.md).