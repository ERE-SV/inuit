# Phase 11 — Engineering handoff — Worksheet

**Status:** not-started  
**Unlocks:** **Gate 6** — Daniel accepts handoff (“engineers can start from this folder + Figma”)  
**Primary path:** this file  
**Depends on:** Gates 1–5 + Phase 10 risk pack  
**Owner:** Malte prepares / Daniel accepts  

## Learn (read before working)

### What this phase is

Engineers should **not** dig through chat. You assemble a **single entry pack**: what we are building, for whom, what MVP means, what is decided, what is still open (with owners), and which budget/ops/privacy constraints limit the build.

You deliver the **blueprint index**. Coded product build is a later program unless Daniel expands scope. Optional dumps: [SYSTEM-CONTEXT.md](SYSTEM-CONTEXT.md), [BUILD-CONSTRAINTS.md](BUILD-CONSTRAINTS.md), [OPEN-QUESTIONS-FOR-ENG.md](OPEN-QUESTIONS-FOR-ENG.md), [HANDOFF-CHECKLIST.md](HANDOFF-CHECKLIST.md).

### Engineer-ready pack (student level)

| Piece | Job |
| --- | --- |
| **System context** | Short what/why/for whom — beachhead, versions, matching & supply paragraphs |
| **Figma + inventories** | Screens engineers implement; frames match inventory IDs |
| **Data / matching specs** | Fields, acquisition, match rules |
| **Build constraints** | Money, headcount, beachhead-only, privacy → shape eng choices |
| **Open questions** | Unresolved items tagged **eng** vs **business**, blocking or not |
| **Checklist + sign-off** | Binary: pack complete; Daniel accepts |

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Handoff** | Package so a new engineer starts without re-asking strategy | Gate 6 bar |
| **MVP build scope** | Exactly what to implement first | Ambiguity fails Gate 6 |
| **Build constraint** | Limit from finance/ops/risk | Prevents “build everything” |
| **Open question (E-ID)** | Unresolved implementation/strategy item | Must have an owner |
| **Decision log** | Authoritative Gates 1–6 | Not chat |
| **Gate 6** | Daniel’s accept that the pack is engineer-ready | You prepare; you do not self-approve |

### Common beginner mistakes

- Linking empty stubs as if gated  
- Ambiguous MVP vs V2  
- Open questions without eng/business owner  
- Skipping SYSTEM-CONTEXT (“read the whole repo”)  
- Self-approving Gate 6  
- Forgetting privacy/run-cost in BUILD-CONSTRAINTS  
- Orphan Figma (no link / inventories don’t match frames)  

## How to prove answers

- Artifact present → path + Gate/decision ID where locked  
- Figma → URL in `../06-product/FIGMA.md` + matching inventory Screen IDs  
- Constraints → paths to Phase 08/09/10  
- Open questions → filled OPEN-QUESTIONS-FOR-ENG.md  
- Follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md) only if you add new factual claims  

## Tasks

### [ ] 11-T1 — Handoff index (gated artifacts)

**Done when:** Every major gated artifact is linked and OK (or blocker named with owner).  
**Unlocks / feeds:** README index; HANDOFF-CHECKLIST  

#### Sub-questions

- [ ] **11-T1-Q1.** Fill status for each:

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

  - **Answer:** (table)  
  - **Proof:** (paths + decision IDs)  

- [ ] **11-T1-Q2.** If any row is not OK: what is blocked and who must finish it before Gate 6?
  - **Answer:**  
  - **Proof:**  

### [ ] 11-T2 — System context

**Done when:** [SYSTEM-CONTEXT.md](SYSTEM-CONTEXT.md) has what/beachhead/versions/matching/supply filled.  
**Unlocks / feeds:** Gate 6 walkthrough  

#### Sub-questions

- [ ] **11-T2-Q1.** ≤5 sentences: product loop, primary value, explicit non-goals.
  - **Answer:**  
  - **Proof:** (product concept / charter)  

- [ ] **11-T2-Q2.** Beachhead niche × geography + Gate 1 decision ID.
  - **Answer:**  
  - **Proof:**  

- [ ] **11-T2-Q3.** One line each: MVP / V2 / V3 (what ships).
  - **Answer:**  
  - **Proof:** (VERSION-MAP / product concept)  

- [ ] **11-T2-Q4.** Matching in one paragraph (hard filters, soft scores, Top-X, human confirm).
  - **Answer:**  
  - **Proof:** (`../07-data-matching/MATCHING-SPEC.md`)  

- [ ] **11-T2-Q5.** Supply in one paragraph (MVP feeds/API vs crawl + Phase 2/3 direction).
  - **Answer:**  
  - **Proof:** (data acquisition / ops)  

### [ ] 11-T3 — MVP build scope clarity

**Done when:** Must-build vs must-not-build is unambiguous; Figma linked; residual ambiguity captured as E-ID.  
**Unlocks / feeds:** Gate 6  

#### Sub-questions

- [ ] **11-T3-Q1.** Bullets: what engineers **must** build for MVP; what they must **not** build yet (V2/V3/non-goals).
  - **Answer:**  
  - **Proof:** (scope checkpoint + VERSION-MAP + inventories)  

- [ ] **11-T3-Q2.** Confirm FIGMA.md link works; MVP (+ V2 as gated) inventories match frame names.
  - **Answer:**  
  - **Proof:** (`../06-product/FIGMA.md` + inventories)  

- [ ] **11-T3-Q3.** One sentence an engineer might still find ambiguous — resolve it or add E-ID.
  - **Answer:**  
  - **Proof:**  

### [ ] 11-T4 — Build constraints

**Done when:** [BUILD-CONSTRAINTS.md](BUILD-CONSTRAINTS.md) has ≥4 rows + ≥2 hard “out of bounds” eng choices.  
**Unlocks / feeds:** Gate 6  

#### Sub-questions

- [ ] **11-T4-Q1.** Constraints table ≥4 rows:

  | Constraint | Source | Implication for build |
  | --- | --- | --- |
  | Budget / run-cost envelope | Phase 09 |  |
  | Headcount for ingestion | Phase 08 |  |
  | Beachhead-only scope | Gate 1 |  |
  | Privacy (home/commute) | Phase 10 |  |

  - **Answer:** (table)  
  - **Proof:** (paths to 08/09/10)  

- [ ] **11-T4-Q2.** ≥2 implementation choices that are **out of bounds** (e.g. wrong cloud region, raw home on employer UI, unbounded crawl).
  - **Answer:**  
  - **Proof:**  

### [ ] 11-T5 — Open questions for engineering

**Done when:** [OPEN-QUESTIONS-FOR-ENG.md](OPEN-QUESTIONS-FOR-ENG.md) has ≥6 rows with owners; blocking set identified; business leftovers deferred or decided.  
**Unlocks / feeds:** Gate 6  

**Required columns:** ID · Question · Blocking MVP? · Owner (eng / business) · Notes  

#### Sub-questions

- [ ] **11-T5-Q1.** ≥6 E-IDs covering leftovers (privacy/crawl, matching thresholds, feeds, region, ATS handoff, etc. as relevant).
  - **Answer:** (count)  
  - **Proof:** (path)  

- [ ] **11-T5-Q2.** Which E-IDs **block MVP**? What if unresolved at kickoff?
  - **Answer:**  
  - **Proof:**  

- [ ] **11-T5-Q3.** Business-owned leftovers: decided or explicitly deferred in the decision log?
  - **Answer:**  
  - **Proof:**  

### [ ] 11-T6 — Checklist & decision log

**Done when:** HANDOFF-CHECKLIST artifacts/clarity boxes done (or gaps owned); Gates 1–5 IDs listed; Malte prepared-by row filled.  
**Unlocks / feeds:** Gate 6 meeting  

#### Sub-questions

- [ ] **11-T6-Q1.** All HANDOFF-CHECKLIST “Artifacts present” + “Clarity” boxes ticked, or gaps listed with owners.
  - **Answer:**  
  - **Proof:** (path to HANDOFF-CHECKLIST.md)  

- [ ] **11-T6-Q2.** Decision log has Gates 1–5; Gate 6 draft line ready. Paste decision IDs.
  - **Answer:**  
  - **Proof:** (`/decisions/DECISION-LOG.md`)  

- [ ] **11-T6-Q3.** Fill Malte row on HANDOFF-CHECKLIST (name + date + ready for Daniel).
  - **Answer:**  
  - **Proof:**  

### [ ] 11-T7 — Gate 6 meeting pack

**Done when:** Gate brief written; 5-minute walkthrough order set.  
**Unlocks / feeds:** Daniel accept  

#### Sub-questions

- [ ] **11-T7-Q1.** Prepare gate brief from [meetings/templates/gate.md](../../../meetings/templates/gate.md) — ask = accept handoff.
  - **Answer:** (path)  
  - **Proof:**  

- [ ] **11-T7-Q2.** List walkthrough order (e.g. SYSTEM-CONTEXT → Figma MVP → matching → constraints → open E-IDs → checklist).
  - **Answer:**  
  - **Proof:** N/A — process  

## Gate pack (Gate 6)

- [ ] SYSTEM-CONTEXT filled  
- [ ] BUILD-CONSTRAINTS filled  
- [ ] OPEN-QUESTIONS-FOR-ENG ≥6 rows  
- [ ] HANDOFF-CHECKLIST prepared  
- [ ] README handoff index complete  
- [ ] Figma + inventories linked  
- [ ] Risk pack linked (`../10-risk/`)  
- [ ] Finance constraints linked (`../09-finance/`)  
- [ ] Decision log Gates 1–6 ready  
- [ ] Gate brief ready  

**Ask for Daniel:** Accept handoff — engineers can start from this folder + Figma?  
**Conditions:**  
**Reject if:**  

| Role | Name | Date | Result |
| --- | --- | --- | --- |
| Prepared by (Malte) |  |  |  |
| Accepted by (Daniel) |  |  | Approve / conditions / reject |

**Daniel only** accepts Gate 6 in the decision log.

## Handoff (program close)

After Gate 6 is **accepted** and logged:

1. Set this phase README status per convention (`gated` / `done`)  
2. Update [STATUS.md](../../../STATUS.md) — all gates accepted or deferred with owner + date  
3. Weeks 15–16: rework/evidence/polish only; no new niche/scope without decision-log entry  
4. Engineers use **this folder + Figma** as entry — not chat  

**Out of scope unless Daniel expands:** coded frontend/backend build.
