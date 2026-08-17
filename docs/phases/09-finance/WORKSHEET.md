# Phase 09 — Monetization & finance worksheet

**For:** Malte  
**How to use:** [WORKSHEET-GUIDE.md](../WORKSHEET-GUIDE.md) · cite facts per [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)  
**Gate:** **Gate 5** — lock finance shape  
**Depends on:** Gate 2 (GTM milestones), ops checkpoint (phase 08 headcount/cost drivers)  
**Brief inputs (assumptions, may be outdated):** [04-monetization.md](../../brief/04-monetization.md)

Tick a task only when **every** sub-question under it has **Answer** + **Proof**.

---

## Learn

### What this phase is

You turn “companies pay for performance” into **math Daniel can plan with**: who pays, what event triggers a charge, what it costs to run, and whether revenue covers that at named milestones.

The **spreadsheet holds the formulas**; [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md) explains *why* the numbers. Do not leave critical math only in prose.

### Terms (plain language)

| Term | Meaning |
| --- | --- |
| **Who pays** | Which side of the marketplace sends money (usually employers; seekers freemium). |
| **Billable event** | The exact action that triggers an invoice (e.g. qualified match shared, interview booked). Not “when someone hires someday.” |
| **Unit economics** | Money in and money out **per unit** (per billable event, per active seeker, or per employer) — not only total company P&L. |
| **CAC** | Customer acquisition cost — what you spend to win one paying employer (or one active seeker), depending on which unit you model. |
| **Contribution** | Revenue minus variable costs for that unit (before fixed overhead). |
| **COGS / variable cost** | Costs that rise with volume (LLM extract, feed fees per listing, payment fees). |
| **Opex** | Running costs that don’t scale 1:1 with each event (infra base, tools, legal buffer). |
| **Fully loaded headcount** | Salary + employer charges + tools for that role (from phase 08). |
| **Milestone projection** | Snapshot at a named GTM milestone: volume → revenue → cost. |
| **Sensitivity / scenario** | Same model with a few drivers changed (best / base / worst) so Gate 5 isn’t a single fantasy number. |
| **Break-even** | Month or volume where contribution covers fixed run cost (state the definition you use). |

### Beginner mistakes

1. **Inventing listing prices** — “~2–3k CHF” in the brief is a hypothesis. Source real portal/competitor prices or write `unknown`.
2. **Vague billable events** — “when we deliver value” is not billable. Name the event, who pays, and when charged.
3. **Revenue without GTM volumes** — funnel must tie to Gate 2 milestones and phase 08 headcount timing.
4. **Skipping spreadsheet tabs** — every tab in [MODEL-OUTLINE.md](MODEL-OUTLINE.md) is required; narrative alone fails Gate 5.
5. **One scenario only** — Gate 5 needs best / base / worst with ≤5 driver changes explained.
6. **Ignoring compliance cost** — put a legal/compliance buffer even if rough (label as assumption).
7. **Seekers as primary revenue too early** — brief preference is employer-primary; if you change that, say so explicitly for Daniel.

---

## Tasks

### 09-T1 — Who pays & billable events

- [ ] **09-T1 done** when Q1–Q5 answered + proved

Copy the filled table into [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md) and the **Pricing** tab.

#### 09-T1-Q1 — Primary payer

Who is the **primary** paying customer in MVP (employer vs seeker vs hybrid)? One sentence why.

**Answer:**  
**Proof:** (path to GTM/beachhead decision or brief + labeled inference)

#### 09-T1-Q2 — Seeker money rules

What is **free forever** for seekers vs what (if anything) is premium later? If premium is out of MVP, write `N/A — post-MVP` and still state free boundaries.

**Answer:**  
**Proof:**

#### 09-T1-Q3 — Billable event catalog (≥2 events)

Fill ≥2 rows (preferred performance events + any subscription/hybrid if you propose them):

| Event name | Who pays | Price (CHF) | When charged | In MVP? Y/N |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

**Answer:** (table above)  
**Proof:** (competitor/comp links or `unknown` + what you’d need)

#### 09-T1-Q4 — Exact MVP charge trigger

Which **one** event is the default MVP invoice trigger? Why not hire-success-only?

**Answer:**  
**Proof:**

#### 09-T1-Q5 — Packaging choice

Pure performance, subscription-with-caps, or hybrid? State the choice and one rejected alternative.

**Answer:**  
**Proof:**

---

### 09-T2 — Price points vs comps

- [ ] **09-T2 done** when Q1–Q3 answered + proved

#### 09-T2-Q1 — Listing baseline (sourced)

What do beachhead employers typically pay today for a classic listing / agency / LinkedIn-style channel? Fill ≥3 sourced comps or mark rows `unknown`.

| Comp | Product | Price / unit | URL | Accessed |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

**Answer:** (table)  
**Proof:** (same URLs + dates; Tier A/B only for gate-critical numbers)

#### 09-T2-Q2 — Our price vs baseline

For your MVP billable event, what is the **target price**, and how does it compare to the baseline (e.g. “~X× cheaper” or “not comparable — different unit”)?

**Answer:**  
**Proof:**

#### 09-T2-Q3 — Value story in one line

Complete: “Employers pay us for ___ , not for ___ .”

**Answer:**  
**Proof:** (inference OK if labeled and tied to Q1–Q2)

---

### 09-T3 — Spreadsheet build (MODEL-OUTLINE tabs)

- [ ] **09-T3 done** when Q1–Q8 answered + proved

Create Google Sheets or Excel. Put link or `model.xlsx` in this folder. Reference from [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md).

**Required tabs** (exact names): `Assumptions` · `Pricing` · `Costs_monthly` · `Headcount` · `Funnel` · `P&L_monthly` · `Milestones` · `Scenarios`

#### 09-T3-Q1 — File location

Where is the spreadsheet (path or URL)?

**Answer:**  
**Proof:** (link/path that Daniel can open)

#### 09-T3-Q2 — Assumptions tab

Does **Assumptions** include: unit prices, conversion rates, CAC, headcount FTEs, infra monthly, feed costs, LLM cost/1k, launch month — each with value, unit, source/note, scenario=base?

**Answer:** (yes / list missing rows)  
**Proof:** (screenshot section or cell range note)

#### 09-T3-Q3 — Pricing tab

Does **Pricing** list every billable event from 09-T1 with who pays, price, when charged, competitor comp link?

**Answer:**  
**Proof:**

#### 09-T3-Q4 — Costs_monthly tab

List categories with monthly CHF + start month (infra, tools, data/feeds, LLM, legal buffer, other).

**Answer:** (summary table or “see sheet — ranges”)  
**Proof:**

#### 09-T3-Q5 — Headcount tab

Are FTEs, start months, and fully loaded costs **copied from phase 08** (not reinvented)? Note any deliberate change.

**Answer:**  
**Proof:** (path to `../08-ops/HEADCOUNT-PLAN.md` or ops model)

#### 09-T3-Q6 — Funnel tab

Month → seekers active, employers active, matches, billable events — tied to GTM milestones?

**Answer:**  
**Proof:** (path to Gate 2 GTM plan)

#### 09-T3-Q7 — P&L_monthly tab

Is there an **18–36 month** P&L with revenue, variable, opex, headcount, contribution, cash (or runway note)?

**Answer:** (horizon in months)  
**Proof:**

#### 09-T3-Q8 — Minimum drivers check

Confirm all minimum drivers from [MODEL-OUTLINE.md](MODEL-OUTLINE.md) are present (billable definition+price, matches→billable conversion, seeker/employer growth, ingestion/sales FTEs, infra+data+LLM, compliance buffer).

**Answer:** (checklist)  
**Proof:**

---

### 09-T4 — Unit economics

- [ ] **09-T4 done** when Q1–Q4 answered + proved

#### 09-T4-Q1 — Unit definition

What is your primary unit for unit economics (per billable event / per paying employer / other)? Why?

**Answer:**  
**Proof:**

#### 09-T4-Q2 — Revenue per unit

Base-case revenue per unit (CHF) and how it is calculated.

**Answer:**  
**Proof:** (sheet cell / formula description)

#### 09-T4-Q3 — Variable cost per unit

What variable costs sit on that unit (extract, feed share, payment fee, etc.)? Sum in CHF.

**Answer:**  
**Proof:**

#### 09-T4-Q4 — Contribution & break-even

Contribution per unit; break-even volume or month under your stated definition.

**Answer:**  
**Proof:**

---

### 09-T5 — Milestone projections (≥3)

- [ ] **09-T5 done** when Q1–Q3 answered + proved

Fill [MILESTONE-PROJECTIONS.md](MILESTONE-PROJECTIONS.md) **and** the **Milestones** tab. Use **named** GTM milestones (not “month 6” alone).

#### 09-T5-Q1 — Milestone table (≥3 rows)

| Milestone name | Timing | Key volumes | Revenue | Cost | Notes |
| --- | --- | --- | --- | --- | --- |
| 1 |  |  |  |  |  |
| 2 |  |  |  |  |  |
| 3 |  |  |  |  |  |

**Answer:** (table)  
**Proof:** (sheet ranges + path to MILESTONE-PROJECTIONS.md)

#### 09-T5-Q2 — Volume bridge

For milestone 2, show the bridge: seekers → matches → billable events → revenue (numbers).

**Answer:**  
**Proof:**

#### 09-T5-Q3 — Cost at milestone 2

Split cost at milestone 2: headcount vs infra/data/LLM vs other.

**Answer:**  
**Proof:**

---

### 09-T6 — Sensitivities (best / base / worst)

- [ ] **09-T6 done** when Q1–Q3 answered + proved

Use the **Scenarios** tab. Change **at most 3–5 drivers**.

#### 09-T6-Q1 — Driver list

Which 3–5 drivers differ across scenarios (e.g. price, conversion, CAC, feed cost, hire delay)?

**Answer:**  
**Proof:**

#### 09-T6-Q2 — Scenario outcomes

| Scenario | Driver changes (short) | Outcome at milestone 2 (revenue / cash / break-even) |
| --- | --- | --- |
| Best |  |  |
| Base |  |  |
| Worst |  |  |

**Answer:** (table — also in FINANCIAL-MODEL.md)  
**Proof:**

#### 09-T6-Q3 — What would kill the model

Which single driver, if worst-case, makes Gate 5 “reject / rethink”? State the threshold.

**Answer:**  
**Proof:** (inference labeled OK)

---

### 09-T7 — Narrative & Gate 5 ask

- [ ] **09-T7 done** when Q1–Q3 answered + proved

#### 09-T7-Q1 — Narrative complete

Is [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md) filled (who pays, costs, sensitivities, spreadsheet link) — not left as stub headings?

**Answer:**  
**Proof:** (path)

#### 09-T7-Q2 — Gate 5 ask

Write the ask: Approve finance shape / Conditions / Reject criteria (draft for Daniel).

**Answer:**  
**Proof:** (will be copied into Gate pack below)

#### 09-T7-Q3 — Decision-log readiness

Draft one-line decision text for `decisions/DECISION-LOG.md` after Daniel decides (leave date blank).

**Answer:**  
**Proof:** N/A — draft only until Daniel locks

---

## Gate pack (Gate 5)

Complete before that week’s T-24 pack. Daniel locks in the 60-minute weekly session; you do not self-approve.

| Item | Status | Path / link |
| --- | --- | --- |
| Spreadsheet (all MODEL-OUTLINE tabs) | [ ] |  |
| [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md) narrative | [ ] |  |
| [MILESTONE-PROJECTIONS.md](MILESTONE-PROJECTIONS.md) ≥3 milestones | [ ] |  |
| Best / base / worst summary | [ ] |  |
| Gate brief ([meetings/templates/gate.md](../../../meetings/templates/gate.md)) | [ ] |  |
| Decision to log after meeting | [ ] | `decisions/DECISION-LOG.md` |

**Ask for Daniel:** Approve finance shape for planning?  
**Conditions (if any):**  
**Reject if:**

---

## Handoff

When Gate 5 is logged:

1. Point phase 10 at cost/compliance buffer numbers that affect risk appetite.  
2. Point phase 11 [BUILD-CONSTRAINTS.md](../11-handoff/BUILD-CONSTRAINTS.md) at run-cost envelope + headcount timing.  
3. Do **not** invent new revenue lines after Gate 5 without a new decision-log entry.  
4. Update [STATUS.md](../../../STATUS.md) gates table.

**Next phase:** [10-risk/WORKSHEET.md](../10-risk/WORKSHEET.md)
