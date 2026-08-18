# 01-T4 — Regulatory and product constraints checklist

| Field | Value |
| --- | --- |
| **Task ID** | `01-T4` |
| **Phase** | [01-market](../README.md) |
| **Answers live in** | [WORKSHEET.md](../WORKSHEET.md) (`01-T4-Q1` … `Q6`) |
| **Week** | 2 |
| **Formal gate** | None — flags feed Phase 07, Phase 10, and counsel |
| **Optional dump** | [MARKET-BRIEF.md](../MARKET-BRIEF.md) §4 |

This file is the **assignment definition**. Do not write answers here.

---

## 1. Definition

You turn the starter **regulatory product checklist** into a set of **product constraints**: for each topic, what the product must be able to explain or refuse, what to assume until counsel reviews, and what is an **open legal question** (not an answer).

Topics (required):

1. Processing candidate profiles for **matching** (purpose limitation).
2. **Home address / commute** calculation (consent, minimization, employers do not see raw home address).
3. Automated **“fit” scores** and notifications (transparency / human-in-the-loop).
4. **Scraping or reusing** third-party listings (ToS / robots.txt / opt-out) for at least two sources.
5. **Cross-border CH/EU** data — when this product would touch EU rules.
6. Any **extra** constraint you discover, plus the starter checklist marked complete.

**Done when:** every starter item has a note in the form **constraint → product implication → open legal question**, with official or primary pages as proof — not blog legal advice.

This is **not** a legal opinion and **not** a compliance program. It is a flag list so matching, crawl, and commute are not designed as if law were optional.

---

## 2. Why this task exists

The product idea needs things that are legally sharp: rich profiles, commute from home, auto-match scores, and a bootstrap that **ingests other people’s listings** ([docs/brief/03-gtm-niche.md](../../../brief/03-gtm-niche.md), [docs/brief/05-tech-feasibility.md](../../../brief/05-tech-feasibility.md)).

If T4 is skipped or written as “we will be GDPR compliant”:

- Phase 07 will specify commute and scores with no constraints.
- Phase 10 will rediscover the same questions.
- Engineering handoff will look implementable and still be blocked.

You **flag**. Counsel (later) **answers**. Daniel should see what cannot be casually promised in GTM or UI copy.

---

## 3. Who reads this, and what happens in Week 2

| Who | What they do |
| --- | --- |
| **Malte** | Read official nDSG / FDPIC / GDPR pages; observe ToS/robots on ≥2 listing sources; write constraints in plain language. |
| **Daniel** | Sees which product bets (commute, crawl, auto-score) are “design under assumption” vs “needs review before build.” May prioritize which flags to take to counsel first — not a legal sign-off. |
| **Phase 07 / 10 / 11** | Dictionary, matching spec, compliance brief, open questions for eng reuse these flags by path. |

Do not ask Daniel to “approve crawling jobs.ch.”

---

## 4. Guiding context

### Product constraints, not legal advice

Write as: “Until counsel reviews, the product should assume X, and must be able to explain Y to a user.”  
Do not write: “It is legal to scrape Z.”

Every item has three lines:

| Line | Meaning |
| --- | --- |
| **Constraint** | What the rule or ToS appears to require or forbid (sourced). |
| **Product implication** | What UI, data, or ops should do or avoid. |
| **Open legal question** | What only counsel can answer. |

### Why these five topics (they match the product)

| Topic | Why it is on the starter list |
| --- | --- |
| Profile matching | The whole product is processing personal data for a new purpose — matching — not “just hosting a CV.” |
| Home / commute | Seeker hard constraint; company has no “commute” field. Home is sensitive; employers should not see the raw address. |
| Fit scores + notify both sides | Automated suggestion that can feel like a decision; transparency and human review matter. |
| Scrape / reuse listings | Bootstrap GTM depends on ingesting existing ads. ToS ≠ “we looked at the homepage.” |
| CH / EU | Seekers, employers, or vendors may sit in the EU; GDPR may apply even if the company is CH. |

### Official pages first

Prefer FDPIC (EDÖB), Swiss nDSG materials, official GDPR / Commission pages. Tier C “GDPR guides” are not enough for a constraint you will design against.

---

## 5. Scope

**In**

- Plain-language purpose limitation for matching profiles.
- Working assumptions for commute (consent, minimization, no raw home address to employers).
- Transparency / human-in-the-loop flags for scores and notifications.
- ToS / robots / opt-out notes for **at least two** concrete sources (e.g. a major portal + a career-page example).
- When CH/EU cross-border likely triggers extra rules.
- Extra constraints you found (discrimination/fairness, retention, enrichment vendors — only if you actually opened a source).

**Out**

- A DPIA, vendor DPA, or “we are compliant” statement.
- A crawl implementation plan or parser list.
- Invented legality (“fair use,” “public data is free”).
- Resolving Phase 10 kill criteria (you only feed them).

---

## 6. Required output

A **checklist table** (in the worksheet, MARKET-BRIEF §4, or `evidence/constraints.md`):

| Topic | Constraint (sourced) | Product implication | Open legal question | Proof (URL + accessed) |
| --- | --- | --- | --- | --- |
| Matching / purpose limitation |  |  |  |  |
| Home / commute |  |  |  |  |
| Automated fit scores / notify |  |  |  |  |
| Scrape / reuse (source A) |  |  |  |  |
| Scrape / reuse (source B) |  |  |  |  |
| CH / EU cross-border |  |  |  |  |
| Extra (if any) |  |  |  |  |

Also tick the list in [SOURCES-STARTER.md](../SOURCES-STARTER.md) **or** paste status in Q6 — one place of truth, pointed to from the other.

---

## 7. Method

1. Official privacy pages first; log in [SOURCES.md](../SOURCES.md).
2. Write Q1 in language a user could read (“we use your profile to…”).
3. Q2: assume **employers never see raw home address** until counsel says otherwise. Document consent + minimization as product requirements.
4. Q3: scores and dual notifications — what would need to be explainable; where a human (employer) still decides to interview.
5. Q4: open robots.txt and ToS/terms for ≥2 sources you might ingest. Quote or paraphrase the relevant clause; **flag for counsel**.
6. Q5: concrete triggers (EU applicants, EU company users, EU subprocessors, targeting EU). “Needs legal review before build” list.
7. Q6: close the starter checklist; add extras.

---

## 8. Sub-questions — what “complete” means

### 01-T4-Q1 — Purpose limitation / matching

What must the product explain to a user in plain language? Proof: official nDSG / FDPIC or GDPR page + access date.

### 01-T4-Q2 — Home / commute

Consent, minimization, and “employers don’t see raw home address” as **assumptions until counsel**. Not a full location-architecture.

### 01-T4-Q3 — Automated scores and notifications

Transparency and human-in-the-loop **expectations to flag**. You are not designing the model.

### 01-T4-Q4 — Scrape / reuse

≥2 named sources. What ToS / robots / opt-out you found. Explicit: not a legality conclusion.

### 01-T4-Q5 — CH / EU

When this product would likely touch EU rules; what is “needs legal review before build.”

### 01-T4-Q6 — Checklist complete + extras

Starter items ticked or pasted; extras listed or “none found.”

---

## 9. What Daniel can usefully react to

- Which flags are **blocking for bootstrap GTM** (crawl/reuse) vs design-time assumptions (commute, scores).
- Order for later counsel: crawl ToS vs privacy of home vs automated scoring.
- Whether Week 2 messaging should already avoid “we scrape the market” language.

No legal approval in the weekly.

---

## 10. Quality bar

| Result | Looks like |
| --- | --- |
| **Pass** | All six Qs; each required topic has constraint + implication + open question; official/primary proof; ≥2 named scrape sources; no “it is legal.” |
| **Incomplete** | Generic “comply with GDPR”; only one scrape source; commute skipped because “hard.” |
| **Fail** | Legal conclusions; invented ToS; “public listings can always be reused.” |

---

## 11. Common mistakes

- Treating this as a law-school essay.
- Forgetting that **notifications to both sides** are also processing.
- Checking robots.txt but not the terms that mention automated access.
- Mixing T4 (constraints) with T1 (channel jobs) — T1 sees the channel; T4 sees whether reuse is restricted.
- Closing Q6 without opening the starter checklist.

---

## 12. What this feeds

| Next | How it uses T4 |
| --- | --- |
| Phase 07 | Dictionary, commute fields, score explanations, acquisition methods. |
| Phase 10 | Compliance brief, risk register, kill criteria. |
| Phase 11 | Open questions for eng — do not leave “is crawl legal?” undiscovered until handoff. |
| Phase 02 / 04 | Honesty in positioning: do not claim a crawl-fed product as if it were first-party supply. |

---

## 13. Start here

1. Starter checklist in [SOURCES-STARTER.md](../SOURCES-STARTER.md).
2. Official nDSG / FDPIC / GDPR pages (Tier A).
3. ToS + robots for two channels you already opened in [01-T1](01-T1-CHANNELS-MAP.md).
4. Fill the constraints table; then `01-T4-Q1` … `Q6`.
