# 07-T5 — Privacy (commute/home) & fairness

| Field | Value |
| --- | --- |
| **Task ID** | `07-T5` |
| **Phase** | [07-data-matching](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [MATCHING-SPEC.md](../MATCHING-SPEC.md) · [DATA-DICTIONARY.md](../DATA-DICTIONARY.md) privacy notes · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Commute/home handling and fairness constraints must be written so product + counsel can review. These are **product constraints to flag**, not legal advice. Feeds Gate 4 and Phase 10.

---

## Our guideline

- **Never send raw home address to employers.** Collect, consent, compute server-side; company sees derived result (e.g. commute band), not home.
- **Document the decline path.** If the seeker declines commute consent, what matching still runs?
- **Fairness = product flags.** Prohibited or restricted automated criteria for the beachhead — flag for legal review, don’t skip.
- **Culture tags need guardrails.** Reduce gaming/bias on soft culture tags in MVP (avoid / low weight / human confirm).
- **Sync with product screens.** Consent and explainability Screen IDs from Phase 06 must match flows you write here.
- **Not legal advice.** Write constraints the product will obey; counsel validates in Phase 10.

| Term | Why it matters |
| --- | --- |
| **Fairness / prohibited criteria** | Rules you will not automate or will constrain — legal + brand trust |

---

## What we have done before

Build on matching spec, dictionary privacy, product consent screens, and brand trust:

- [07-T4 — Matching rules](07-T4-MATCHING-RULES.md) — hard/soft rules, explainability, zero-match (may need updates after privacy decisions)
- [07-T1 — Dictionary](07-T1-DICTIONARY.md) — privacy columns on home_location and related fields
- [07-T3 — Acquisition](07-T3-ACQUISITION.md) — computed commute from home + workplace
- [Phase 06 — product](../../06-product/README.md) — consent screen IDs ([06-T3 MVP inventory](../../06-product/tasks/06-T3-MVP-INVENTORY.md))
- [Phase 05 — brand](../../05-brand/README.md) — **Gate 3** tone/fairness boundaries (trust signal, do/don’t on claims)
- [decisions/DECISION-LOG.md](../../../../decisions/DECISION-LOG.md) — **Gate 1** beachhead (which protected-characteristic risks matter in niche)

---

## What we're doing now

**Goal:** Document home/commute collect-consent-compute-display flow, decline path, fairness constraints, and culture-tag guardrails for Gate 4.

Example questions:

- How is **home_location** collected, consented, stored, and used? Do employers ever see the raw address?
- If the seeker **declines** commute consent, what matching still runs?
- Server-side commute: who computes minutes, and what does the company see instead of home?
- **Fairness:** which criteria are prohibited or restricted for automated filtering in your beachhead (e.g. protected characteristics)? Flag for legal review.
- How do you reduce **gaming** or bias on soft culture tags in MVP (avoid / low weight / human confirm)?

**Start here**

1. Dictionary privacy columns + Phase 06 consent screen IDs.  
2. Write home/commute flow (collect → consent → compute → what company sees).  
3. Decline path + fairness / culture-tag constraints.  
4. Link from the worksheet.  

---

## Why it matters

**For Daniel:** Commute/home + fairness notes in the **Gate 4** pack — product constraints he can review before lock.

**For later phases:** Phase 06 consent and explainability screens must match flows documented here. Phase 10 turns flags into a compliance brief.

**For the program:** Skipping fairness or raw-address leakage is a common beginner mistake — document constraints now so Gate 4 is trustworthy, not just implementable.
