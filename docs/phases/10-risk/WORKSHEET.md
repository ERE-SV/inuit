# Phase 10 — Risk, compliance & assumptions — Worksheet

**Status:** not-started  
**Unlocks:** **Gate 6 inputs** (bundled with Phase 11 handoff)  
**Depends on:** Gate 5 recommended (finance informs risk appetite)  
**Owner:** Malte  
**Brief inputs:** [05-tech-feasibility.md](../../brief/05-tech-feasibility.md) · [06-open-questions.md](../../brief/06-open-questions.md)  
**Primary path:** this file  

## How this file works

This is **progress tracking**, not an exam. Tick **Ready** when you can talk about that area in the weekly. Put notes wherever you like and paste the path under **Your notes**.

Read [task files](tasks/README.md) for context and example questions. Each brief has the same thread: **why it exists → guideline → what came before → what we're doing now → why it matters.**

You are **not** a lawyer. Flag constraints and counsel questions; do not invent legal certainty. See [WORKSHEET-GUIDE.md](../WORKSHEET-GUIDE.md) and [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md).

## Learn (read before working)

### What this phase is

Write down the scary parts so engineers and Daniel are not surprised: privacy, crawl/ToS, discrimination in matching, load-bearing assumptions, and when to kill or pivot.

Optional dumps: [RISK-REGISTER.md](RISK-REGISTER.md), [COMPLIANCE-BRIEF.md](COMPLIANCE-BRIEF.md), [ASSUMPTIONS.md](ASSUMPTIONS.md), [KILL-CRITERIA.md](KILL-CRITERIA.md).

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Risk register** | Likelihood, impact, mitigation, owner | Nothing critical should live only in chat |
| **Assumption** | Treated as true without full proof — say how you'd test | Load-bearing unknowns need names |
| **Kill / pivot criteria** | Pre-agreed triggers; Daniel decides | Hope is not a plan |
| **Allowlist + opt-out** | Only approved sources; employers can demand removal | Compliance-by-design for crawl supply |

### What to avoid

- “We'll fix compliance later”  
- Treating inferred fields as facts  
- Empty risk rows  
- Inventing Swiss law quotes  
- Hiding risks in chat  
- Self-approving Gate 6 (you prepare inputs; Daniel accepts with handoff)  

## Progress

| Task | Focus | Task file | Your notes | Ready |
| --- | --- | --- | --- | --- |
| **10-T1** | Privacy | [10-T1-PRIVACY.md](tasks/10-T1-PRIVACY.md) |  | [ ] |
| **10-T2** | Crawl / ToS | [10-T2-CRAWL-TOS.md](tasks/10-T2-CRAWL-TOS.md) |  | [ ] |
| **10-T3** | Matching fairness | [10-T3-MATCHING-FAIRNESS.md](tasks/10-T3-MATCHING-FAIRNESS.md) |  | [ ] |
| **10-T4** | Risk register | [10-T4-RISK-REGISTER.md](tasks/10-T4-RISK-REGISTER.md) |  | [ ] |
| **10-T5** | Assumptions | [10-T5-ASSUMPTIONS.md](tasks/10-T5-ASSUMPTIONS.md) |  | [ ] |
| **10-T6** | Kill / pivot | [10-T6-KILL-CRITERIA.md](tasks/10-T6-KILL-CRITERIA.md) |  | [ ] |
| **10-T7** | Compliance brief | [10-T7-COMPLIANCE-BRIEF.md](tasks/10-T7-COMPLIANCE-BRIEF.md) |  | [ ] |

## Gate pack (Gate 6 inputs)

Bundle with [../11-handoff/WORKSHEET.md](../11-handoff/WORKSHEET.md). This phase alone does not approve legal risk. **Malte does not self-approve Gate 6.**

- [ ] RISK-REGISTER (≥8 rows suggested)  
- [ ] COMPLIANCE-BRIEF complete enough to discuss  
- [ ] ASSUMPTIONS (≥8 rows suggested)  
- [ ] KILL-CRITERIA (≥4 triggers suggested)  
- [ ] Counsel open-item list ready for handoff  

**Daniel reviews at Gate 6:** risks are explicit; nothing critical only verbal.

## Handoff

Phase 11 will consume:

- Eng-relevant open questions → [OPEN-QUESTIONS-FOR-ENG.md](../11-handoff/OPEN-QUESTIONS-FOR-ENG.md)  
- Privacy/crawl constraints → [BUILD-CONSTRAINTS.md](../11-handoff/BUILD-CONSTRAINTS.md)  
- This folder linked from the handoff index  

Update [STATUS.md](../../../STATUS.md).

**Next:** [../11-handoff/WORKSHEET.md](../11-handoff/WORKSHEET.md)
