# 08-T2 — Ops model: sources, legal posture, freshness

| Field | Value |
| --- | --- |
| **Task ID** | `08-T2` |
| **Phase** | [08-ops](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [OPS-MODEL.md](../OPS-MODEL.md) or your own doc — link from worksheet |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

The ops checkpoint is not a forever org chart — it is a **supply + quality story** Daniel can hand to finance. Freshness and legal posture summaries stop “we'll crawl everything” from becoming an unchecked assumption.

---

## Our guideline

- **Build on T1.** Each source type from the supply mix gets a role, freshness assumption, and legal posture summary.
- **Plain-language legal posture.** Cite ToS/robots URLs when you claim a posture, or write `unknown — counsel`. Do not invent permissions.
- **Measurable quality.** Name metrics you'd watch — extract rate, completeness, duplicates — not vibes.
- **Opt-out and breakage.** Employers must be able to claim/remove; parsers break — name who owns response in MVP (role, not person).
- **Employer complaint path.** Inferred-field corrections, opt-out / “stop contacting us” — link to GTM [04-T3](../../04-gtm/tasks/04-T3-FORWARD-MOTION.md) and V2 claim screens.
- **Do not approve legal risk.** Summarize posture for Phase 10; this is not legal advice.

---

## What we have done before

**08-T1** — supply approaches:

- [08-T1-SUPPLY-APPROACHES.md](08-T1-SUPPLY-APPROACHES.md) — primary/secondary mix, ingestion path  

**Phase 07** — acquisition approach and allowlist thinking.

---

## What we're doing now

**Goal:** Document how supply stays fresh and trustworthy in MVP — sources, legal posture summaries, quality checks, and breakage ownership.

Example questions — skip what stays thin after an honest pass.

- Supply table: Feed/API | Crawl (allowlist) | First-party — role in MVP, legal posture **summary**, freshness assumption?
- Freshness SLA hypothesis: how often must hot listings be re-checked? What is “too stale” for the beachhead?
- Quality checks: which metrics would you watch (extract rate, field completeness, duplicate rate, …)?
- Opt-out / claim: what happens if an employer wants listings removed or corrected?
- If parsers break after a career-site relaunch — who is on-call in MVP (role, not person's name)?

You might use a shape like [OPS-MODEL.md](../OPS-MODEL.md):

| Source type | Role in MVP | Legal posture summary | Freshness assumption |
| --- | --- | --- | --- |
| Feed / API |  |  |  |
| Crawl (allowlist) |  |  |  |
| First-party employer |  |  |  |

**Start here**

1. Draft the supply table (any format).  
2. Add freshness + ≥3 quality metrics.  
3. Note opt-out and on-call; link from worksheet.

---

## Why it matters

**For the rest of Phase 08:** [T3](08-T3-HEADCOUNT.md) needs breakage/on-call load. [T5](08-T5-COST-DRIVERS.md) needs freshness-driven re-fetch costs.

**For Daniel:** Supply + freshness + quality hypotheses for the ops checkpoint.

**For later phases:** Phase 10 risk register and compliance brief consume opt-out and crawl posture from here.
