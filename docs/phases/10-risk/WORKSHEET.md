# Phase 10 — Risk, compliance & assumptions — Worksheet

**Status:** not-started  
**Unlocks:** **Gate 6 inputs** (bundled with Phase 11 handoff)  
**Primary path:** this file  
**Depends on:** Gate 5 recommended (finance informs risk appetite)  
**Brief inputs:** [05-tech-feasibility.md](../../brief/05-tech-feasibility.md) · [06-open-questions.md](../../brief/06-open-questions.md)

## Learn (read before working)

### What this phase is

Strategy can look fine on slides and still be **illegal, unfair, or unbuildable**. You write down the scary parts so engineers and Daniel are not surprised: privacy, crawl/ToS, discrimination in matching, load-bearing assumptions, and when to kill or pivot.

You are **not** a lawyer. Produce a clear brief + open items for counsel — not fake legal certainty. Optional dumps: [RISK-REGISTER.md](RISK-REGISTER.md), [COMPLIANCE-BRIEF.md](COMPLIANCE-BRIEF.md), [ASSUMPTIONS.md](ASSUMPTIONS.md), [KILL-CRITERIA.md](KILL-CRITERIA.md).

### Privacy, crawl, discrimination (student level)

| Topic | Plain meaning | Product implication |
| --- | --- | --- |
| **Privacy (nDSG / GDPR-aligned)** | Rules on collecting/using/storing personal data | Purpose limitation + minimization; consent for sensitive uses (home for commute; recording if voice) |
| **Server-side matching** | Compute fits on our servers | Employers need not see raw home address |
| **Crawl / scrape** | Auto-fetch job pages | Restricted by **ToS** and **robots.txt**; prefer licensed feeds/APIs |
| **Allowlist + opt-out** | Only approved sources; employers can demand removal | Compliance-by-design; need an SLA |
| **Inferred fields** | LLM/rules guess requirements/salary/culture | Must **label**; correction/claim flows; never treat as ground truth |
| **Automated matching** | Software ranks/filters people | Some criteria must **never** be automated discriminators; score ≠ hire guarantee |
| **Lineage / retention** | Know source URL, fetch time, parser version | Different rules for raw crawl vs derived structured fields |

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Risk register** | Risks with likelihood, impact, mitigation, owner | Nothing critical only in someone’s head |
| **Assumption** | Treated as true without full proof yet | Must say how we’d test later |
| **Kill / pivot criteria** | Pre-agreed triggers to stop or change course | Daniel decides; hope is not a plan |
| **DPIA** | Formal high-risk processing review | Flag for counsel — don’t fake the answer |
| **Fairness** | Match logic that systematically disadvantages groups | First-class design, not an afterthought |

### Common beginner mistakes

- “We’ll fix compliance later”  
- Treating inferred fields as facts  
- Empty risk rows (“legal risk” with no likelihood/impact/owner)  
- Assumptions without test methods  
- No kill criteria  
- Inventing Swiss law quotes (cite or `unknown — counsel`)  
- Hiding risks in chat  

## How to prove answers

- Product/data claims → paths to dictionary, matching spec, ops, Figma  
- Law/ToS → official URL + access date, or open counsel item  
- Risks/assumptions/kills → filled evidence files linked from Proof  
- Label inferences; never invent statistics  
- Follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)  

## Tasks

### [ ] 10-T1 — Privacy (product implications)

**Done when:** Data types, commute/consent, visibility/retention, inferred-field UX, and ≥3 counsel questions are written.  
**Unlocks / feeds:** COMPLIANCE-BRIEF; Phase 11 BUILD-CONSTRAINTS  

#### Sub-questions

- [ ] **10-T1-Q1.** List personal data types MVP needs. Mark each: required / optional / deferred.
  - **Answer:**  
  - **Proof:** (path to data dictionary / product concept)  

- [ ] **10-T1-Q2.** How does commute matching work **without** employers seeing raw home address? What consent is required?
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T1-Q3.** What can employers see by default? Retention idea for **raw crawl** vs **derived** fields (OK: `TBD with counsel` + question).
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T1-Q4.** How are inferred fields labeled? Correction / claim / opt-out in one sentence each.
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T1-Q5.** ≥3 open privacy questions only counsel/DPO should answer.
  - **Answer:**  
  - **Proof:** N/A — questions list  

### [ ] 10-T2 — Crawl / ToS / listing reuse

**Done when:** Supply posture, ≥3-source risk table, opt-out SLA, and “expand allowlist” gate are clear.  
**Unlocks / feeds:** COMPLIANCE-BRIEF; risk register  

#### Sub-questions

- [ ] **10-T2-Q1.** MVP beachhead primary supply: feeds/APIs, selective crawl, or mix? One paragraph.
  - **Answer:**  
  - **Proof:** (path to `../07-data-matching/` or `../08-ops/`)  

- [ ] **10-T2-Q2.** Source table ≥3 rows:

  | Source / class | Method (API / feed / crawl) | ToS/robots note | Risk (L/M/H) | Mitigation |
  | --- | --- | --- | --- | --- |
  |  |  |  |  |  |

  - **Answer:** (table)  
  - **Proof:** (URLs or `unknown — legal review`)  

- [ ] **10-T2-Q3.** Employer opt-out/claim: target response time + process owner?
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T2-Q4.** What must be true before expanding beyond the allowlist?
  - **Answer:**  
  - **Proof:**  

### [ ] 10-T3 — Matching, automation & discrimination

**Done when:** Score copy, never-automate list, human confirm, and subjective-factor policy are set.  
**Unlocks / feeds:** COMPLIANCE-BRIEF; matching constraints for eng  

#### Sub-questions

- [ ] **10-T3-Q1.** How will product copy prevent “match score = hire guarantee”?
  - **Answer:**  
  - **Proof:** (matching spec / brand / Figma)  

- [ ] **10-T3-Q2.** Criteria that must **not** be automated filters/scores in MVP (or “none identified — counsel confirm”). Why each?
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T3-Q3.** Before employer contact / interview path, what must a human confirm (seeker and/or company)?
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T3-Q4.** Culture / soft prefs in MVP: structured tags, low-weight inference, or out of automation?
  - **Answer:**  
  - **Proof:**  

### [ ] 10-T4 — Risk register (≥8 rows)

**Done when:** [RISK-REGISTER.md](RISK-REGISTER.md) has ≥8 rows covering required themes; top 3 called out; finance-linked risks noted.  
**Unlocks / feeds:** Gate 6  

**Required columns:** ID · Risk · Likelihood (L/M/H) · Impact (L/M/H) · Mitigation · Owner  

**Must cover at least once:** privacy · crawl/ToS · discrimination/fairness · supply freshness/parser rot · unit economics/CAC · two-sided liquidity · key-person/ops · feed vendor shock  

#### Sub-questions

- [ ] **10-T4-Q1.** Confirm ≥8 rows in RISK-REGISTER.md (IDs `R-01` …).
  - **Answer:** (count)  
  - **Proof:** (path)  

- [ ] **10-T4-Q2.** Top 3 by severity (likelihood × impact) + one-line mitigation each.
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T4-Q3.** Which risk IDs change if Gate 5 **worst-case** economics are true?
  - **Answer:**  
  - **Proof:** (path to Phase 09 scenarios)  

### [ ] 10-T5 — Assumptions register (≥8 rows)

**Done when:** [ASSUMPTIONS.md](ASSUMPTIONS.md) has ≥8 rows with test methods; three load-bearing assumptions highlighted.  
**Unlocks / feeds:** Gate 6  

**Required columns:** ID · Assumption · Why it matters · How we’d test later · Related phase  

#### Sub-questions

- [ ] **10-T5-Q1.** Confirm ≥8 assumptions spanning GTM, matching quality, supply legality/cost, pricing willingness, ops capacity.
  - **Answer:**  
  - **Proof:** (path)  

- [ ] **10-T5-Q2.** Three assumptions that, if false, break the company definition — testing method each.
  - **Answer:**  
  - **Proof:**  

### [ ] 10-T6 — Kill / pivot criteria

**Done when:** [KILL-CRITERIA.md](KILL-CRITERIA.md) has ≥4 measurable triggers including liquidity, unit economics, legal block on supply + one more.  
**Unlocks / feeds:** Gate 6  

#### Sub-questions

- [ ] **10-T6-Q1.** Fill ≥4 rows (who decides = Daniel):

  | Trigger (measurable) | What we do (kill / pivot / narrow) | Who decides |
  | --- | --- | --- |
  |  |  | Daniel |

  - **Answer:** (table)  
  - **Proof:** (path)  

- [ ] **10-T6-Q2.** For each trigger: metric/evidence that would show it fired within ~90 days of launch planning.
  - **Answer:**  
  - **Proof:**  

- [ ] **10-T6-Q3.** One painful outcome that is **not** automatic kill (keeps the bar clear).
  - **Answer:**  
  - **Proof:** (inference)  

### [ ] 10-T7 — Compliance brief completeness

**Done when:** COMPLIANCE-BRIEF sections are non-empty; no critical risk only in chat.  
**Unlocks / feeds:** Phase 11 handoff  

#### Sub-questions

- [ ] **10-T7-Q1.** Confirm COMPLIANCE-BRIEF has: Privacy · Crawl/ToS · Automated matching/discrimination · Retention · Open items for counsel.
  - **Answer:**  
  - **Proof:** (path)  

- [ ] **10-T7-Q2.** Every critical risk appears in RISK-REGISTER, ASSUMPTIONS, or KILL-CRITERIA (name leftovers if any).
  - **Answer:**  
  - **Proof:**  

## Gate pack (Gate 6 inputs)

Bundle with [../11-handoff/WORKSHEET.md](../11-handoff/WORKSHEET.md). This phase alone does not “approve” legal risk.

- [ ] RISK-REGISTER ≥8 rows  
- [ ] COMPLIANCE-BRIEF complete  
- [ ] ASSUMPTIONS ≥8 rows  
- [ ] KILL-CRITERIA ≥4 triggers  
- [ ] Counsel open-item list ready for handoff  

**Daniel reviews at Gate 6:** risks are explicit; nothing critical only verbal.

## Handoff to next phase

Phase 11 will consume:

- Eng-relevant open questions → [OPEN-QUESTIONS-FOR-ENG.md](../11-handoff/OPEN-QUESTIONS-FOR-ENG.md)  
- Privacy/crawl constraints → [BUILD-CONSTRAINTS.md](../11-handoff/BUILD-CONSTRAINTS.md)  
- This folder linked from the handoff index  

Update [STATUS.md](../../../STATUS.md).

**Next:** [../11-handoff/WORKSHEET.md](../11-handoff/WORKSHEET.md)
