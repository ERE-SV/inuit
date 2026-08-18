# 01-T4 — Regulatory product constraints (from T1 channels)

| Field | Value |
| --- | --- |
| **Task ID** | `01-T4` |
| **Phase** | [01-market](../README.md) |
| **Answers live in** | [WORKSHEET.md](../WORKSHEET.md) (`01-T4-Q1` … `Q6`) |
| **Week** | 2 — after T1 channels exist |
| **Formal gate** | None — flags feed Phase 07, 10, and counsel |
| **Optional dump** | [MARKET-BRIEF.md](../MARKET-BRIEF.md) §4 |

This file is the **assignment definition**. Do not write answers here.

T4 is **not** a legal opinion. It turns T1’s real channels and journeys into **product constraints** so matching, commute, scores, and crawl are not designed as if law were optional.

---

## 1. Definition

For each required topic you write three lines: **constraint** (sourced) → **product implication** → **open legal question** (counsel later).

Required topics:

1. Processing profiles for **matching** (purpose limitation).
2. **Home / commute** (consent, minimization; employers do not see raw home address).
3. Automated **fit scores** and dual notifications.
4. **Scrape / reuse** of third-party listings — **≥2 sources from your T1 channels table**.
5. **CH / EU** cross-border — when this product would touch EU rules.
6. Starter checklist complete + any extra you actually found.

**Done when:** the constraints table is full, scrape rows name T1 channels, no sentence says “it is legal to…”

---

## 2. Why this task exists

The idea needs rich profiles, commute from home, auto-scores, and bootstrap **ingest of other people’s ads** ([docs/brief/03-gtm-niche.md](../../../brief/03-gtm-niche.md)). T1 already named those channels and the apply/commute pain. T4 is the flag list so Phase 07/10 do not rediscover this.

You **flag**. Counsel **answers**. Daniel sees what GTM/UI must not promise.

---

## 3. Who reads this, and what happens in Week 2

| Who | What they do |
| --- | --- |
| **Malte** | Official nDSG / FDPIC / GDPR; ToS + robots on **two T1 channels**; plain-language constraints. |
| **Daniel** | Prioritize counsel (crawl vs home vs scores). Not a sign-off. |
| **Phase 07 / 10 / 11** | Reuse flags by path. |

Do not ask Daniel to approve crawling jobs.ch.

---

## 4. Guiding context

### Tie to T1

| T1 fact | T4 use |
| --- | --- |
| Channels table (Q1–Q5) | Q4 scrape sources **must be two named rows** from that table |
| Applicant journey / apply log (home, docs uploaded) | Q1–Q2: what you already typed is personal data |
| Notify-both-sides product idea | Q3: notifications are also processing |
| Disruptors / aggregators (Q21) | Same ToS class of problem — do not assume “they do it so we can” |

### Constraint / implication / open question

| Line | Meaning | Example shape (not legal advice) |
| --- | --- | --- |
| **Constraint** | What the page/ToS appears to require | “Purpose must be specified…” + URL |
| **Product implication** | What we assume in UI/data until counsel | “Explain matching purpose in plain language before profile create.” |
| **Open legal question** | Only counsel | “Does inferred commute from home require a separate consent?” |

**Fail:** “We will be GDPR compliant.” **Fail:** “Public listings can always be reused.”

### Official pages first

FDPIC (EDÖB), nDSG materials, official GDPR/Commission. Tier C “GDPR blogs” are not enough to design against.

`unknown` here means **open legal question** after you opened the official page — not “skipped.”

---

## 5. Scope

**In**

- Plain-language purpose limitation for matching.
- Commute assumptions: consent, minimization, no raw home address to employers.
- Score + notify transparency / human-in-the-loop **flags**.
- ToS / robots / opt-out on **≥2 T1 channels** (e.g. a major portal + a career page or second portal).
- Concrete CH/EU triggers (EU applicants, EU company users, EU subprocessors).
- Extras only if you opened a source (fairness, retention, enrichment vendors).

**Out**

- DPIA, DPAs, “we are compliant.”
- Crawl architecture.
- Invented legality (“fair use”).
- Resolving Phase 10 kill criteria.

---

## 6. Required output

[MARKET-BRIEF.md](../MARKET-BRIEF.md) §4 or `evidence/constraints.md`:

| Topic | Constraint (sourced) | Product implication | Open legal question | Proof (URL + accessed) |
| --- | --- | --- | --- | --- |
| Matching / purpose limitation |  |  |  |  |
| Home / commute |  |  |  |  |
| Fit scores / notify both |  |  |  |  |
| Scrape / reuse — T1 channel A |  |  |  |  |
| Scrape / reuse — T1 channel B |  |  |  |  |
| CH / EU cross-border |  |  |  |  |
| Extra (or “none found”) |  |  |  |  |

Tick [SOURCES-STARTER.md](../SOURCES-STARTER.md) **or** paste status in Q6 — one place of truth.

---

## 7. Method

1. Official privacy pages → [SOURCES.md](../SOURCES.md).
2. Q1 in user-facing language (“we use your profile to…”).
3. Q2: assume employers **never** see raw home address until counsel says otherwise.
4. Q3: what must be explainable; who still decides to interview (human).
5. Q4: robots.txt **and** terms that mention automated access, for two **T1** channels. Quote/paraphrase; flag for counsel.
6. Q5: trigger list + “needs review before build.”
7. Q6: close starter checklist.

---

## 8. Sub-questions — what “complete” means

**Q1.** What must the product explain for matching? Official page + date.

**Q2.** Home/commute: consent, minimization, no raw address to employers — **assumptions until counsel**.

**Q3.** Scores + notifications: transparency / human-in-the-loop **flags**, not a model design.

**Q4.** ≥2 **named T1 channels**. ToS / robots / opt-out. Not a legality conclusion.

**Q5.** When EU rules likely apply; what is blocked until review.

**Q6.** Starter checklist done; extras or “none found.”

---

## 9. What Daniel can usefully choose

- Counsel order: crawl/reuse vs home vs automated scoring.
- Whether Week 2 language already avoids “we scrape the market.”
- Which T1 channels are **off-limits to ingest** until review (assumption, not a verdict).

No legal approval.

---

## 10. Quality bar

| Result | Looks like |
| --- | --- |
| **Pass** | Three lines per topic; official/primary proof; Q4 names two T1 channels; no “it is legal.” |
| **Incomplete** | “Comply with GDPR”; one scrape source; commute skipped; Q4 uses a site not in T1. |
| **Fail** | Legal conclusions; invented ToS; “public data is free.” |

---

## 11. Common mistakes

- Law-school essay with no product implication.
- Forgetting dual notifications are processing.
- robots.txt without the terms clause on automated access.
- Mixing T1 (what the channel *is*) with T4 (whether reuse is restricted).

---

## 12. What this feeds

| Next | How it uses T4 |
| --- | --- |
| Phase 07 | Dictionary, commute, score copy, acquisition methods. |
| Phase 10 / 11 | Compliance, risks, open questions for eng. |
| Phase 02 / 04 | Do not market a crawl-fed product as first-party supply. |

---

## 13. Start here

1. T1 channels table — pick two ingest candidates.
2. [SOURCES-STARTER.md](../SOURCES-STARTER.md) checklist + official nDSG/FDPIC/GDPR.
3. Fill the constraints table; then `01-T4-Q1` … `Q6`.
