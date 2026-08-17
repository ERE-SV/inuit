# Program schedule (real calendar)

**Source of truth for dates.** Week numbers in [PLAN.md](../PLAN.md) / [PLAN-WEEKS.md](../PLAN-WEEKS.md) map here.  
Fill at kickoff from [ONBOARDING.md](../ONBOARDING.md) · mirror into [STATUS.md](../STATUS.md).

## Locked inputs (required before Week 1)

| Field | Value |
| --- | --- |
| **Program start (Week 1 day 1)** | _TBD_ — ISO date `YYYY-MM-DD` |
| **Program end (last day of Week 16)** | _TBD_ — = start + 111 days (16×7 − 1) |
| **Weekly meeting weekday** | _TBD_ — e.g. Thursday |
| **Weekly meeting time** | _TBD_ — e.g. 16:00–17:00 (**60 min max**) |
| **Timezone** | _TBD_ — e.g. Europe/Zurich |
| **T-24 deadline** | 24 hours before each weekly meeting (same clock time) |
| **Figma link** | _TBD_ |
| **Async channel** | WhatsApp (or update) |

### How to compute

1. Choose **Program start** = first calendar day of Week 1 (recommend a Monday).  
2. **Program end** = start + 111 days (end of Week 16).  
3. For each week `n` (1–16):  
   - Week range = `[start + 7×(n−1), start + 7×(n−1) + 6]`  
   - Weekly meeting = the chosen weekday that falls inside that range  
   - T-24 = meeting datetime − 24 hours  
4. Paste dates into the table below and send calendar invites for all **16 weekly sessions** (60 min). Gate locks happen **in** that week’s weekly — no extra invites.

---

## 16-week calendar

Fill the date columns at kickoff. Gate weeks: the lock is **Decision A in that week’s weekly session** (same 60 min slot). Note the gate in T-24; do not book a second meeting.

| Week | Block | Week dates (Mon–Sun or start–end) | Weekly meeting | T-24 due | Planned milestone |
| --- | --- | --- | --- | --- | --- |
| 1 | A | _TBD_ | _TBD_ | _TBD_ | Market start |
| 2 | A | _TBD_ | _TBD_ | _TBD_ | Market + competitive |
| 3 | A | _TBD_ | _TBD_ | _TBD_ | Competitive + beachhead |
| 4 | A | _TBD_ | _TBD_ | _TBD_ | **Gate 1 — Beachhead** |
| 5 | B | _TBD_ | _TBD_ | _TBD_ | **Gate 2 — GTM** |
| 6 | B | _TBD_ | _TBD_ | _TBD_ | **Gate 3 — Brand** |
| 7 | B | _TBD_ | _TBD_ | _TBD_ | **Scope checkpoint** + MVP start |
| 8 | C | _TBD_ | _TBD_ | _TBD_ | MVP Figma |
| 9 | C | _TBD_ | _TBD_ | _TBD_ | MVP finish + V2 start |
| 10 | C | _TBD_ | _TBD_ | _TBD_ | V2 + acquisition + matching |
| 11 | C | _TBD_ | _TBD_ | _TBD_ | **Gate 4** + ops checkpoint |
| 12 | D | _TBD_ | _TBD_ | _TBD_ | V3 Figma finish |
| 13 | D | _TBD_ | _TBD_ | _TBD_ | **Gate 5 — Finance** |
| 14 | D | _TBD_ | _TBD_ | _TBD_ | **Gate 6 — Handoff** |
| 15 | E | _TBD_ | _TBD_ | _TBD_ | Buffer |
| 16 | E | _TBD_ | _TBD_ | _TBD_ | Buffer / close |

---

## Meeting invites checklist (after dates locked)

- [ ] 16× weekly working session on calendar (Malte + Daniel), **60 min each**  
- [ ] Gate weeks: mark the weekly invite title as “Weekly + Gate N” — **no extra holds**  
- [ ] Reminder: T-24 is Malte’s deadline every week (not a second meeting)  
- [ ] Kickoff meeting scheduled (before Week 1 start)  
- [ ] [STATUS.md](../STATUS.md) shows start, end, Week 1 focus  
- [ ] [PLAN.md](../PLAN.md) gantt note points here for real dates  

---

## Gate date targets (fill after schedule locked)

| Gate | Target week | Target meeting date | Status |
| --- | --- | --- | --- |
| 1 Beachhead | 4 | _TBD_ | not-started |
| 2 GTM | 5 | _TBD_ | not-started |
| 3 Brand | 6 | _TBD_ | not-started |
| Scope checkpoint | 7 | _TBD_ | not-started |
| 4 UI + data/matching | 11 | _TBD_ | not-started |
| Ops checkpoint | 11 | _TBD_ | not-started |
| 5 Finance | 13 | _TBD_ | not-started |
| 6 Handoff accept | 14 | _TBD_ | not-started |
