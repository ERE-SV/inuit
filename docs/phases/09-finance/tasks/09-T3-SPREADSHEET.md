# 09-T3 — Spreadsheet build

| Field | Value |
| --- | --- |
| **Task ID** | `09-T3` |
| **Phase** | [09-finance](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | Google Sheet / Excel in this folder or linked; reference from [FINANCIAL-MODEL.md](../FINANCIAL-MODEL.md) |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

The **spreadsheet holds the formulas**; narrative explains *why*. Critical math only in prose fails Gate 5. T3 is where T1–T2 decisions become auditable numbers. Full tab detail: [MODEL-OUTLINE.md](../MODEL-OUTLINE.md).

---

## Our guideline

- **Sheet is source of truth for math.** FINANCIAL-MODEL explains; cells calculate.
- **Pull from Phase 08.** Headcount and cost drivers belong in Assumptions, Costs_monthly, and Headcount tabs — note deliberate changes.
- **Minimum drivers present.** Billable definition+price; conversion; growth; FTEs; infra+data+LLM; compliance buffer.
- **Unknown is OK.** Use `unknown` + placeholder until sourced — never invent CHF.
- **Daniel must be able to open it.** Path or URL on the worksheet.

---

## What we have done before

**09-T1–T2** — monetization shape and comps:

- [09-T1-WHO-PAYS.md](09-T1-WHO-PAYS.md) — billable events for Pricing tab  
- [09-T2-PRICE-COMPS.md](09-T2-PRICE-COMPS.md) — price inputs  

**Phase 08 ops checkpoint** — headcount timing and cost drivers for Assumptions / Headcount / Costs_monthly.

Suggested tab shape: [MODEL-OUTLINE.md](../MODEL-OUTLINE.md).

---

## What we're doing now

**Goal:** Build the financial spreadsheet with MODEL-OUTLINE-shaped tabs and minimum drivers in base case.

Example questions — skip what stays thin after an honest pass.

- Where does the spreadsheet live (path or URL Daniel can open)?
- Does **Assumptions** hold drivers (prices, conversion, CAC, FTEs, infra, feeds, LLM, launch) with value / unit / source / scenario?
- Does **Pricing** list billable events from T1 with who pays, price, when charged, comps?
- **Costs_monthly**: categories with monthly CHF + start month?
- **Headcount**: FTEs and fully loaded costs from Phase 08 (note deliberate changes)?
- **Funnel**: month → volumes tied to GTM milestones?
- **P&L_monthly**: 18–36 month horizon with revenue, variable, opex, headcount, contribution, cash/runway note?
- Are minimum drivers from MODEL-OUTLINE present?

Suggested tab names (inspiration for what the sheet should contain):

| Tab | Purpose |
| --- | --- |
| **Assumptions** | Drivers: value, unit, source/note, scenario=base |
| **Pricing** | Billable events |
| **Costs_monthly** | Run costs by category |
| **Headcount** | From ops model |
| **Funnel** | Volume bridge |
| **P&L_monthly** | 18–36 months |
| **Milestones** | Exec view (≥3 named GTM milestones) |
| **Scenarios** | Best / base / worst (≤5 driver changes) |

**Start here**

1. Skim [MODEL-OUTLINE.md](../MODEL-OUTLINE.md).  
2. Create the sheet; pull headcount from Phase 08.  
3. Link path/URL on the worksheet.

---

## Why it matters

**For the rest of Phase 09:** [T4–T6](09-T4-UNIT-ECONOMICS.md) pull numbers from this sheet; [T7](09-T7-NARRATIVE-GATE5.md) links it in the Gate 5 pack.

**For Daniel:** Openable sheet he can audit in the 60-minute Gate 5 session.

**For later phases:** Phase 11 BUILD-CONSTRAINTS cites run-cost envelope from this model.
