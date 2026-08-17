# Research & citation standard

All factual claims in phase deliverables must be **checkable**. Unsupported numbers do not pass a gate.

## What counts as evidence


| Tier                        | Examples                                                                    | How to treat                                |
| --------------------------- | --------------------------------------------------------------------------- | ------------------------------------------- |
| **A — Primary / official**  | BFS/stat offices, company pricing pages, product docs, laws, annual reports | Prefer; quote/paraphrase with link          |
| **B — Reputable secondary** | Established press, industry associations, major research firms              | OK with link + date; note if paywalled      |
| **C — Weak / opaque**       | Random blogs, unsourced LinkedIn posts, “everyone knows”                    | Do not use for gate-critical claims         |
| **Inference**               | Your conclusion from A/B facts                                              | Label explicitly as **inference**, not fact |


Interviews are optional in this program. If used, log date, role (not personal data beyond what’s needed), and treat as **anecdote** unless multiple independent sources agree.

## Required citation format

In deliverables, use inline or footnote style consistently (necessary for agents):

```text
Claim. (Source Title — https://example.com — accessed YYYY-MM-DD)
```

Or a `SOURCES.md` / appendix table:


| Claim ID | Claim summary                 | URL       | Accessed   | Tier |
| -------- | ----------------------------- | --------- | ---------- | ---- |
| S-01     | jobs.ch listing price range … | https://… | 2026-08-17 | A    |




## Rules

1. **No invented statistics.** If you cannot source it, write `unknown` and say what you’d need to learn it.
2. **Competitor pricing:** only if visible/sourced; otherwise `unknown` — never guess.
3. **Access date required** — pages change.
4. **Separate fact vs recommendation** — recommendations are fine; they must sit on cited facts or labeled assumptions.
5. **Assumptions** belong in the phase doc *and* eventually `docs/phases/10-risk/ASSUMPTIONS.md`.
6. **Stale data:** if a source is >24 months old, flag it (`dated`) and prefer a newer source when possible.
7. Leave sources in the artifact (and `SOURCES.md` where used).



## “Strong desk research” bar (this program)

Enough that Daniel can click through and verify the load-bearing claims for a gate (beachhead liquidity, competitor pricing shape, regulatory constraints, cost comps). Depth beats volume: **fewer claims, all sourced**, rather than a long unsourced narrative.

## Gate implication

A gate pack can be rejected solely for weak evidence — even if the recommendation “sounds right.”