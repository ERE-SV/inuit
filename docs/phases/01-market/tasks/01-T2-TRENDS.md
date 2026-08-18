# 01-T2 — Product “so what” on the T1 trend inventory

| Field | Value |
| --- | --- |
| **Task ID** | `01-T2` |
| **Phase** | [01-market](../README.md) |
| **Answers live in** | [WORKSHEET.md](../WORKSHEET.md) (`01-T2-Q1` … `Q5`) |
| **Week** | 2 — **after** [01-T1-Q20](01-T1-MARKET-FUNCTIONS.md) |
| **Formal gate** | None — feeds Gate 1 later |
| **Optional dump** | [MARKET-BRIEF.md](../MARKET-BRIEF.md) §2 |

This file is the **assignment definition**. Do not write answers here.

T2 is **not** a second market study. T1 already collected how the market functions and a trend inventory. T2 only answers: **so what for this product?**

---

## 1. Definition

You take the trend bullets from [01-T1-Q20](01-T1-MARKET-FUNCTIONS.md) (plus T1 facts on apply volume, salary, structure if they sit in Q11/Q14–Q18) and write a **product “so what”** for each load-bearing claim.

A “so what” is one sentence: what this fact means for a **two-sided matchmaking** product (structured requirements, less noise, seeker floors, commute/preferences, trust) — not “HR is changing” and not “so we should raise funding.”

**Done when:** at least **four** trends have source (T1 path or new URL) **and** a product so-what; Q2 states evidence strength; Q5 says what we would do if the most load-bearing trend is wrong.

You are still **not** picking a niche.

---

## 2. Why this task exists

T1 can be true and still useless for product (“employment rose 0.4%”). T2 is the filter: which facts change matching, profiles, or messaging?

If this is thin:

- Phase 02 white space becomes “we use AI.”
- Phase 03 “pain” scores are vibes.
- Phase 05 claims noise or salary transparency that T1 never supported.

---

## 3. Who reads this, and what happens in Week 2

| Who | What they do |
| --- | --- |
| **Malte** | Start from T1-Q20. Add at most **two** new trends if T1 missed something load-bearing. Fill the so-what table. |
| **Daniel** | Reads the **table**, not a memo. Chooses which claims may be used in later messaging vs must stay internal. |
| **Later phases** | Positioning and beachhead *pain* rows cite this table by path. |

---

## 4. Guiding context

### Reuse first

Point **Proof** at T1 answers or MARKET-BRIEF §1.8. Do not re-download the same BFS table and rewrite Q1 as a new stats dump. [01-T1-Q6](01-T1-MARKET-FUNCTIONS.md) / Q11 already hold official volume and growth.

### What “so what” must name

Tie the fact to **this** product ([docs/brief/01-vision.md](../../../brief/01-vision.md)): bidirectional match, fewer unqualified applies, reusable profiles, commute, salary floors, notify-both-sides. If you cannot name a product implication, the trend is decorative — drop it or leave it on T1 only.

### Brief claims = hypotheses (do not paste as facts)

| Claim in the brief | What T2 should do |
| --- | --- |
| 40–50 applications / 3–6 months | Reuse T1-Q14; so-what + **strength** (strong / weak / unknown). |
| AI cover-letter noise | Reuse T1-Q15 / apply log; do not upgrade “I saw a cover-letter field” into a market trend. |
| Unqualified inbound | Employer-side vs seeker-side separately. |
| Structured requirements beat keyword search | Q3 so-what for *bidirectional* match. |
| Salary ranges / floors on profiles | Q4 — sourced CH transparency or `unknown`. |

### Strength labels (required on Q2, useful on all rows)

`strong` (Tier A/B, CH, recent) · `weak` (anecdote, foreign, dated) · `unknown` (searched, nothing usable)

---

## 5. Scope

**In**

- ≥4 rows: T1 trend → so what for matchmaking / less-noise hiring.
- Apply-volume / AI / structure / salary as the default four *themes* — you may swap one if T1 evidence is stronger elsewhere.
- One “if this is wrong” on the **most** load-bearing row (Q5).

**Out**

- Re-doing T1 (new channel maps, new fill-volume study).
- Beachhead pick.
- Legal analysis ([01-T4](01-T4-CONSTRAINTS.md)).
- Invented “talent shortage %.”

---

## 6. Required output

Trend table in [MARKET-BRIEF.md](../MARKET-BRIEF.md) §2 or `evidence/trends.md`:

| # | Trend (one line) | T1 proof path or new URL + accessed + tier | Strength | So what for this product | If wrong (one row only) |
| --- | --- | --- | --- | --- | --- |
| 1 |  | `01-T1-Q20` / … | strong / weak / unknown |  |  |

Minimum **four** rows with so-what. Q5 fills the last column on exactly one row.

---

## 7. Method

1. Copy T1-Q20 bullets into the table.
2. Drop decorative rows. Keep or add until you have four that change the product.
3. Write one so-what each. If you need a new source, log it in [SOURCES.md](../SOURCES.md) — that is the only new research.
4. Q2: set strength using T1-Q14–Q16, not vibes.
5. Q5 last: pick the row that would most change MVP scope or messaging if reversed.

---

## 8. Sub-questions — what “complete” means

**Q1.** Which T1-Q20 (and at most two adds) will you carry? List them with T1 paths. No new BFS essay.

**Q2.** Apply volume / unqualified / AI cover letters — **so what** + **strength**. Seeker vs employer if you can tell them apart.

**Q3.** Skills-based / structured requirements — sourced change + so what for **bidirectional** matching (not a better search box).

**Q4.** CH salary transparency / benchmarks — so what for **company ranges** and **seeker floors**. `unknown` beats a guessed median.

**Q5.** The one trend that would most change this product if wrong: fact → so what → **inference** if reversed.

---

## 9. What Daniel can usefully choose

- Which so-whats are **load-bearing** for the product story vs decorative.
- Whether “AI cover-letter noise” may appear in later messaging (`strong`) or stays internal (`weak` / `unknown`).
- Whether Q5’s trend should become a Phase 03 scorecard criterion.

No lock. Options with pros/cons.

---

## 10. Quality bar

| Result | Looks like |
| --- | --- |
| **Pass** | ≥4 rows; each has T1 path or URL + so what; Q2 has a strength label; Q5 has if-wrong; no second market study. |
| **Incomplete** | T1 list copied with empty so-what; Q1 is a new BFS dump; strength missing. |
| **Fail** | Brief 40–50 / 2–3k pasted as fact; “AI matching is the future”; beachhead chosen. |

---

## 11. Common mistakes

- Rewriting T1-Q6 as T2-Q1.
- So-what that only says “this matters.”
- Upgrading the apply log into a national apply-volume statistic.
- Inventing salary bands (that is still sourced-or-unknown).

---

## 12. What this feeds

| Next | How it uses T2 |
| --- | --- |
| Phase 02 white space | Only claim gaps T2 marked `strong` or clearly labeled inference. |
| Phase 03 scorecard | Pain / non-CV criteria cite this table. |
| Phase 05 | Messaging caution: no unsourced pain. |

---

## 13. Start here

1. [01-T1-Q20](01-T1-MARKET-FUNCTIONS.md) (and Q14–Q16, Q18 if needed).
2. Fill MARKET-BRIEF §2; then worksheet `01-T2-Q1` … `Q5`.
3. New URLs only → [SOURCES.md](../SOURCES.md).
