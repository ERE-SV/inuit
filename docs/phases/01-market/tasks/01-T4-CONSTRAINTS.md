# 01-T4 — Product constraints from what you saw

| Field | Value |
| --- | --- |
| **Task ID** | `01-T4` |
| **Phase** | [01-market](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [MARKET-BRIEF.md](../MARKET-BRIEF.md) §4 or `evidence/` |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

This product idea touches sensitive ground: **personal profiles**, **home location for commute**, **automated fit scores**, and **reusing other people’s job listings** to bootstrap supply.

T4 turns what you learned in T1 into **early product constraints** — so we design and message with eyes open, and counsel gets a useful flag list later. This is **not** legal advice.

---

## Our guideline

- **You flag; counsel answers.** Never write “it is legal to scrape” or “we are GDPR compliant.”
- **Tie to real channels.** Scrape/ToS questions should name **channels you opened in T1**, not generic “job boards.”
- **Product language first.** For each topic: what must we explain to users? What do we assume in UI until counsel reviews?
- **Official sources.** nDSG / FDPIC / GDPR orientation pages beat GDPR blogs. See [SOURCES-STARTER.md](../SOURCES-STARTER.md) regulatory section.
- **Open questions are OK.** `unknown` here means “needs counsel” after you opened the official page — not “skipped.”

Useful shape per topic: **constraint (sourced)** → **product implication** → **open legal question**.

---

## What we have done before

**[01-T1](01-T1-MARKET-FUNCTIONS.md)** — you named real channels, walked applicant journeys (what data gets asked), and saw how listings appear on portals vs career pages.

**[01-T2](01-T2-PRODUCT-IMPLICATIONS.md)** — you may have noted product angles that imply processing personal data (commute, notify-both-sides, inferred requirements). T4 makes those implications explicit for privacy and crawl.

If T1 skipped channels you plan to ingest, go back and open them before claiming constraints here.

---

## What we're doing now

**Goal:** Flag product constraints early — matching, commute/home, scores, listing reuse, cross-border data.

Example questions:

**Profiles and matching**

- What must the product be able to explain in plain language about **why** we process profile data for matching?

**Home and commute**

- What should we assume about **consent** and **minimization** for home location until counsel reviews?
- Should employers **never** see raw home address by default? What might they see instead (e.g. commute band)?

**Scores and notifications**

- What transparency do automated **fit scores** and **notify both sides** need?
- Where should a **human** still decide (e.g. before interview)?
- What **trust signal** must the product show so users understand matching is an indicator, not a hire guarantee?

**Scraping and listing reuse**

- For **≥2 channels from your T1 table**: what do terms of service and robots.txt suggest about automated access or reuse?
- What would an **employer opt-out or claim** process look like operationally?

**Cross-border**

- When might CH/EU rules apply (EU applicants, EU employers, EU subprocessors)?

**Starter checklist**

- Work through the regulatory items in [SOURCES-STARTER.md](../SOURCES-STARTER.md). Anything else you discovered?

**Start here**

1. Pick two T1 channels that matter for bootstrap ingest.  
2. Open official privacy pages + those channels’ terms / robots.txt.  
3. Write constraints in product language — implication + open question.  
4. Link from the worksheet.

---

## Why it matters

**For the rest of Phase 01:** [T5](01-T5-SOURCES-PASS.md) should log the official URLs you used here.

**For Daniel:** A prioritized list for counsel (crawl vs home vs scores) and messaging guardrails (“don’t promise crawl-fed supply as first-party”).

**For later phases:** Phase 07 (dictionary, commute, matching), Phase 10 (compliance brief), and Phase 11 (build constraints) all reuse these flags — better to surface them now than in week 14.
