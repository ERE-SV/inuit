# Phase 06 — Product concept & Figma — Worksheet

**Status:** not-started  
**Unlocks:** **Scope checkpoint** (end Week 7) → MVP/V2/V3 feature lists locked; feeds **Gate 4** (with Phase 07, Week 11); V3 finishes Week 12  
**Primary path:** this file  
**Depends on:** Gate 3 brand principles  

## Learn (read before working)

### What this phase is

You turn the vision into a **versioned product**: what ships first (MVP), what waits (V2/V3), which screens exist, and how journeys work — then design those screens in Figma under the locked brand. Start from seeded [PRODUCT-CONCEPT.md](PRODUCT-CONCEPT.md) and [MVP-SCREEN-INVENTORY.md](MVP-SCREEN-INVENTORY.md). You **decide keep / cut / add / rename / split** — you do not invent a second product from scratch.

### MVP vs V2 vs V3 (plain language)

| Version | Job | Rule of thumb |
| --- | --- | --- |
| **MVP** | Prove the **core match loop** with beachhead liquidity: profiles → Top-X → notify → interview interest (+ bootstrap forward) | If you cut it, matching does not work end-to-end |
| **V2** | Retention + trust depth: what-if, career-gap, claim/correct inferred listings, richer employer profiles, light ATS handoff | Improves quality/retention after the loop works |
| **V3** | Scale + intelligence: company push API, market intel, optional soft matching / voice capture | Needs MVP+V2 learning; often monetization-linked |

Every feature belongs in **exactly one** version. “Nice for later” is not a dumping ground — put it in V2 or V3 with a reason, or cut it.

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Journey** | Step-by-step path a seeker or company user takes to get value | Screens must cover the path, not orphan pages |
| **Non-goal** | Something you deliberately will *not* build soon | Stops ATS-sized scope creep |
| **Screen inventory** | Table of frames: purpose, actions, data, states | Engineer + Daniel can audit Figma completeness |
| **Scope checkpoint** | Daniel locks MVP/V2/V3 feature lists (Week 7) | Expanding later needs a new decision-log entry |
| **Annotation standard** | Each Figma frame states purpose, actions, data, states, nav | Gate 4: implementable without a workshop |
| **Bootstrap forward** | Sending pre-qualified candidates against *ingested* listings before employers fully onboard | Core GTM + MVP feature from the brief |
| **Indicator vs guarantee** | Match score suggests fit; it does not promise a hire | Must appear in product copy and empty/error states |

### Common beginner mistakes

- Stuffing V2/V3 ideas into MVP “just in case”  
- Designing a full employer ATS (approvals, stage tracking) — explicit non-goal  
- Ignoring seeded inventory rows (silent deletes without change log)  
- Figma screens with no empty/loading/error states  
- Feature lists that disagree with VERSION-MAP / inventories  
- Starting Figma before Gate 3 brand principles  
- Scope checkpoint skipped — building screens for unlocked features  

## How to prove answers

- Decisions → path to updated concept / inventory / VERSION-MAP  
- Figma → URL in [FIGMA.md](FIGMA.md) + frame name matching inventory Screen ID  
- Label product opinions as **inference** when not from brief/gates  
- Follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md) for any market claims  

## Tasks

### [ ] 06-T1 — Learn versions, journeys, non-goals

**Done when:** You can explain MVP/V2/V3 and document seeker + company journeys + non-goals in PRODUCT-CONCEPT.  
**Unlocks / feeds:** Scope checkpoint; inventory keep/cut  

#### Sub-questions

- [ ] **06-T1-Q1.** In your own words: what is the **one job** of MVP vs V2 vs V3 for this marketplace?
  - **Answer:**  
  - **Proof:** (path: `PRODUCT-CONCEPT.md` + this answer)  

- [ ] **06-T1-Q2.** Rewrite the **seeker happy path** as numbered steps (signup → … → interview interest). Flag any step that is V2+.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T1-Q3.** Rewrite the **company / HR happy path**, including the **bootstrap forward** path (ingested listing → forwarded candidate).
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T1-Q4.** List **non-goals** for near term. For each, one sentence: what would go wrong if you built it in MVP anyway?
  - **Answer:**  
  - **Proof:** (path: brief `02-product.md` + your list)  

- [ ] **06-T1-Q5.** Where must UI say the match is an **indicator**, not a hire guarantee?
  - **Answer:**  
  - **Proof:**  

### [ ] 06-T2 — Feature lists: keep / cut / move (scope checkpoint prep)

**Done when:** Every seeded feature is in exactly one of MVP / V2 / V3 / cut, with rationale; VERSION-MAP matches.  
**Unlocks / feeds:** Scope checkpoint with Daniel  

#### Sub-questions

- [ ] **06-T2-Q1.** Open [PRODUCT-CONCEPT.md](PRODUCT-CONCEPT.md). For each **MVP** seeded feature: **keep**, **cut**, or **move** to V2/V3? One-line rationale each.
  - **Answer:**  
  - **Proof:** (path: updated `PRODUCT-CONCEPT.md`)  

- [ ] **06-T2-Q2.** Same for **V2** and **V3** seeded features. Add any **new** feature only if you can name which journey step it serves and which version — else cut.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T2-Q3.** Update [VERSION-MAP.md](VERSION-MAP.md) so it matches your lists. Note any conflict you resolved.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T2-Q4.** What is the **smallest** set of features that still completes: seeker match list → company Top-X → mutual interview interest?
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T2-Q5.** Prepare the **scope checkpoint ask** (approve / conditions / reject notes) for Daniel.
  - **Answer:**  
  - **Proof:** (path: `PRODUCT-CONCEPT.md` Scope checkpoint section)  

### [ ] 06-T3 — MVP screen inventory: keep / cut / add / rename / split

**Done when:** Every MVP inventory row has a decision; change log updated; flows still cover the core loop.  
**Unlocks / feeds:** MVP Figma frames; Gate 4 pack  

#### Sub-questions

- [ ] **06-T3-Q1.** Walk [MVP-SCREEN-INVENTORY.md](MVP-SCREEN-INVENTORY.md) row by row (MVP-000 … MVP-061). Mark each: **keep / cut / rename / split / add**. Summarize cuts and adds here.
  - **Answer:**  
  - **Proof:** (path: inventory + change log dated)  

- [ ] **06-T3-Q2.** Which screens are required for Flow 1 (seeker signup → first matches)? List Screen IDs.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T3-Q3.** Which screens are required for Flow 2 (company → Top-X) and Flow 3 (strong fit → interview interest)?
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T3-Q4.** Empty-match behavior: MVP message-only vs V2 what-if — confirm version placement and which screen shows it.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T3-Q5.** Privacy / commute consent: which Screen ID owns it, and what happens if the user declines?
  - **Answer:**  
  - **Proof:**  

### [ ] 06-T4 — Figma annotation standard + MVP structure

**Done when:** FIGMA.md has the file link; MVP pages follow the annotation standard; brand principles applied.  
**Unlocks / feeds:** Weeks 8–9 MVP depth; Gate 4  

#### Sub-questions

- [ ] **06-T4-Q1.** Set the canonical Figma URL in [FIGMA.md](FIGMA.md). Confirm Gate 3 decision ID is noted.
  - **Answer:**  
  - **Proof:** (Figma URL + decision ID)  

- [ ] **06-T4-Q2.** State the **annotation standard** you will use on every frame (purpose, primary actions, data fields, states, nav). Paste a filled example for one screen (e.g. MVP-030).
  - **Answer:**  
  - **Proof:** (Figma frame name + screenshot path optional)  

- [ ] **06-T4-Q3.** Which brand visual principles (color/type/density) did you apply on the first MVP frames? List 3 concrete choices.
  - **Answer:**  
  - **Proof:** (path: `../05-brand/…` + Figma)  

- [ ] **06-T4-Q4.** After scope checkpoint: start core MVP flows in Figma. Which flows are framed vs still outline-only?
  - **Answer:**  
  - **Proof:**  

### [ ] 06-T5 — V2 / V3 inventories + Gate 4 readiness

**Done when:** V2 inventory+Figma complete for Gate 4; V3 planned/finished per week plan; inventories match frames.  
**Unlocks / feeds:** Gate 4 (with Phase 07); eng handoff later  

#### Sub-questions

- [ ] **06-T5-Q1.** Fill [V2-SCREEN-INVENTORY.md](V2-SCREEN-INVENTORY.md) from locked V2 features. Keep/cut/add as needed.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T5-Q2.** Confirm every V2 inventory row has a Figma frame (or note deferred with Daniel’s OK).
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T5-Q3.** Fill [V3-SCREEN-INVENTORY.md](V3-SCREEN-INVENTORY.md) and complete V3 Figma by Week 12. List any open gaps.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T5-Q4.** Can an engineer implement UI structure from Figma + inventories without a strategy workshop? List remaining ambiguities.
  - **Answer:**  
  - **Proof:**  

- [ ] **06-T5-Q5.** Sync check: dictionary fields you expect on MVP screens — any screen showing a field Phase 07 cut? Resolve.
  - **Answer:**  
  - **Proof:** (path: `../07-data-matching/DATA-DICTIONARY.md`)  

## Gate / checkpoint pack

### Scope checkpoint (Week 7)

- [ ] MVP / V2 / V3 feature lists — each feature in exactly one version  
- [ ] Seeker + company journeys documented  
- [ ] Non-goals explicit  
- [ ] MVP Figma structure started under brand principles  
- [ ] Decision-log draft for Daniel to lock  

### Gate 4 (with Phase 07; Week 11) — product side

- [ ] MVP Figma complete: screens, key states, annotations  
- [ ] V2 Figma complete to same standard  
- [ ] Inventories match Figma frame names  
- [ ] Phase 07 matching/dictionary ready in the same pack  

**Daniel only** locks gates in the decision log.

## Handoff to next phase

Phase 07 will consume:

- Locked feature lists (which matching behaviors are MVP vs later)  
- Screen IDs that display which profile fields  
- Explainability / consent screens that matching rules must support  

Phase 08 will consume:

- Bootstrap ingest + forward as an MVP ops load  
- Non-goals that keep ATS/support scope bounded  
