# Financial model outline

Build a spreadsheet (Google Sheets or Excel). Put the file or link in this folder and reference it from [FINANCIAL-MODEL.md](FINANCIAL-MODEL.md).

## Recommended tabs

| Tab | Purpose | Required columns / rows |
| --- | --- | --- |
| **Assumptions** | Single place for drivers | Unit prices, conversion rates, CAC, headcount FTEs, infra monthly, feed costs, LLM cost/1k, launch month; each row: value, unit, source/note, scenario (base) |
| **Pricing** | Billable events | Event name, who pays, price, when charged, competitor comp link |
| **Costs_monthly** | Run costs | Category, monthly CHF, start month, notes (infra, tools, data, LLM, legal buffer, other) |
| **Headcount** | From ops model | Role, FTE, start month, fully loaded monthly cost, trigger |
| **Funnel** | Volume bridge | Month → seekers active, employers active, matches, billable events |
| **P&L_monthly** | 18–36 months | Revenue, COGS/variable, opex, headcount, contribution, cash |
| **Milestones** | Exec view | Milestone name, month, revenue, cost, key volume — mirrors [MILESTONE-PROJECTIONS.md](MILESTONE-PROJECTIONS.md) |
| **Scenarios** | Best / base / worst | Toggle or copy sheet; change 3–5 drivers max |

## Minimum drivers to include (base case)

- Billable event definition + price  
- Matches → billable conversion  
- Seeker and employer growth (tied to GTM milestones)  
- Ingestion/sales FTEs and start timing (from phase 08)  
- Monthly infra + data/feed + LLM extract  
- Compliance / legal buffer (even if rough)

## Narrative doc

[FINANCIAL-MODEL.md](FINANCIAL-MODEL.md) explains *why* the numbers; the sheet holds *math*. Do not leave critical formulas only in prose.

## Gate 5 pack

- Spreadsheet link/export in `docs/phases/09-finance/`  
- Narrative + milestone table  
- Best/base/worst summary
