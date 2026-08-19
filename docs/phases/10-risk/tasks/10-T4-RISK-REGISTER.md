# 10-T4 — Risk register

| Field | Value |
| --- | --- |
| **Task ID** | `10-T4` |
| **Phase** | [10-risk](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [RISK-REGISTER.md](../RISK-REGISTER.md) or equivalent |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Nothing critical should live only in someone's head or chat. Gate 6 wants risks with likelihood, impact, mitigation, owner — T4 consolidates T1–T3 and finance/ops flags into one register.

---

## Our guideline

- **≥8 real rows.** Privacy, crawl/ToS, discrimination, supply freshness, unit economics, liquidity, key-person, feed vendor shock — cover the set.
- **No empty rows.** “Legal risk” without L/M/H and owner doesn't help.
- **Top 3 by severity.** One-line mitigation each for Daniel's 60-minute walkthrough.
- **Tie to Gate 5 worst-case.** Which risk IDs worsen if worst-case economics are true?
- **Owner named.** Malte, Daniel, counsel, eng — someone accountable.

---

## What we have done before

**10-T1–T3** — compliance topics:

- [10-T1-PRIVACY.md](10-T1-PRIVACY.md) — privacy risks and counsel items  
- [10-T2-CRAWL-TOS.md](10-T2-CRAWL-TOS.md) — supply legality rows  
- [10-T3-MATCHING-FAIRNESS.md](10-T3-MATCHING-FAIRNESS.md) — automation/discrimination risks  

**Phase 08–09** — ops bus factor, unit economics, worst-case sensitivities.

---

## What we're doing now

**Goal:** Build a risk register with ≥8 rows covering the major risk categories, plus top-3 summary.

Example questions — skip what stays thin after an honest pass.

- ≥8 risks covering privacy, crawl/ToS, discrimination/fairness, supply freshness/parser rot, unit economics/CAC, two-sided liquidity, key-person/ops, feed vendor shock?
- Top 3 by severity + one-line mitigation each?
- Which risk IDs change if Gate 5 **worst-case** economics are true?

You might use this shape ([RISK-REGISTER.md](../RISK-REGISTER.md)):

| ID | Risk | Likelihood | Impact | Mitigation | Owner |
| --- | --- | --- | --- | --- | --- |
| R-01 |  | L/M/H | L/M/H |  |  |

**Start here**

1. Seed from T1–T3 + Phase 08/09.  
2. Aim for ≥8 real rows.  
3. Link on worksheet.

---

## Why it matters

**For the rest of Phase 10:** [T7](10-T7-COMPLIANCE-BRIEF.md) cross-checks nothing critical is missing from the register.

**For Daniel:** Explicit register for Gate 6 — risks he can discuss in 60 minutes, not surprises later.

**For later phases:** Phase 11 handoff index links this register; eng kickoff starts from named risks.
