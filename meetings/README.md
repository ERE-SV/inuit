# Meetings

**One live meeting per week.** Gates, checkpoints, and weekly review share that slot. No extra review or gate meetings.

## Calendar (set at kickoff)


| Ritual                 | Default                                                                           | Length    |
| ---------------------- | --------------------------------------------------------------------------------- | --------- |
| Weekly working session | Same weekday/time each week; **Malte leads**. Includes gate locks when due.       | **60 min max** |
| T-24 pack              | **24 hours before** weekly: all content in repo + agenda + 2–3 decision proposals | Written   |
| Kickoff                | Once, before Week 1                                                               | **60 min max** |


**Real dates live in [SCHEDULE.md](SCHEDULE.md)** (program start/end, all 16 weeks, meeting + T-24 + gate targets).

Quick mirror (keep in sync with SCHEDULE):


| Field                      | Value                             |
| -------------------------- | --------------------------------- |
| **Program start**          | *TBD*                             |
| **Program end**            | *TBD*                             |
| **Weekly slot**            | *TBD* (weekday + time + timezone) |
| **Figma workspace / link** | *TBD*                             |
| **Async channel**          | WhatsApp (or update)              |
| **Canonical docs**         | **this git repo**                 |


Also mirror start/end into [STATUS.md](../STATUS.md) and [ONBOARDING.md](../ONBOARDING.md).

---



## 1. Kickoff (once)

**Goal:** Same understanding of charter, repo, and how we work. Malte has completed [ONBOARDING.md](../ONBOARDING.md) Day 0–1 reads beforehand when possible.

### Kickoff checklist

**Before**

- [ ] Malte has repo access + can push/commit
- [ ] Malte has read CHARTER, PLAN, RESEARCH-STANDARD, ONBOARDING
- [ ] Figma seat ready to assign (or create file in-session)

**During — agenda (60 min max)**

1. Walk [CHARTER.md](../CHARTER.md) and [PLAN.md](../PLAN.md) (12 min)
2. Repo tour: phases stubs, decisions, meetings, STATUS (8 min)
3. Tools: git habits, Figma, [RESEARCH-STANDARD.md](../RESEARCH-STANDARD.md) (8 min)
4. **Lock program dates:** start, end (= start + 111 days), weekly weekday/time/timezone (10 min)
5. Agree who fills [SCHEDULE.md](SCHEDULE.md) and sends 16 calendar invites (5 min)
6. Agree async channel; Figma access (5 min)
7. Working preferences / open questions (12 min)

**After (same day)**

- [ ] Fill [ONBOARDING.md](../ONBOARDING.md) program-dates table  
- [ ] Fill [SCHEDULE.md](SCHEDULE.md) — all 16 weeks + gate targets  
- [ ] Fill calendar mirror table above  
- [ ] Send/create **16 weekly** calendar invites (+ kickoff if not done)  
- [ ] Write `notes/YYYY-MM-DD-kickoff.md`  
- [ ] Update [STATUS.md](../STATUS.md) (start, end, Week 1 focus)  
- [ ] Set Figma link in SCHEDULE + `docs/phases/06-product/FIGMA.md` when file exists  

---



## 2. Weekly working session (every week, including gate weeks)

**Goal:** Informed discussion of the week’s findings. Daniel arrives having pre-read the repo; the meeting is for **presentation, challenge, and choices** — not for discovering content for the first time.

**Lead:** Malte runs the meeting and may adjust the agenda (adjustments also filed at T-24 when known).

**Hard stop:** 60 minutes. Unfinished items go to async or next week’s T-24 — do not book a follow-up meeting.

### T-24 (24 hours before) — Malte

1. **Upload all week’s content** to the repo (phase stubs filled/updated, sources, Figma links as relevant).
2. File the **T-24 pack** using [templates/weekly-t24.md](templates/weekly-t24.md) → `notes/YYYY-MM-DD-weekly-t24.md`
  - Predefined agenda (see below)  
  - Paths to artifacts  
  - **2–3 decision proposals**, each with options and **advantages / disadvantages** listed
  - If a **gate or checkpoint** is due this week: attach the [gate brief](templates/gate.md) and make that lock **Decision A**
3. Ping Daniel (async channel) with the note path so he can pre-read.

**Daniel (before the meeting):** Skim T-24 pack + linked artifacts. Come ready to choose among prepared options.

### Live agenda (Malte leads) — 60 min max

Malte may drop/shorten a block if T-24 already said so, or adjust live if discussion requires it (note the change in session notes). Times still must sum to **≤ 60**.


| #   | Block                       | Time    | What happens                                                                                                                                                                                       |
| --- | --------------------------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **Review of the week**      | 5 min   | What was planned vs done; slips and why                                                                                                                                                            |
| 2   | **Presentation of results** | 15 min  | Malte presents findings (substance, not reading docs aloud). On gate weeks: recommendation + evidence highlights. Daniel challenges evidence and implications                                      |
| 3   | **Discussion of decisions** | 25 min  | Malte presents **2–3** prepared decisions with options + pros/cons. **Daniel only chooses** among those options (or sends back for a better option set). On gate weeks, Decision A is the gate lock |
| 4   | **Plan + outlook**          | 10 min  | Agree changes to week plan / STATUS; next 1–2 weeks’ focus and deliverables                                                                                                                        |
| 5   | **Blockers**                | 5 min   | What’s stuck; who unblocks                                                                                                                                                                         |


### Gate weeks (same slot, same agenda)

When a formal **gate** or **checkpoint** is due (see [SCHEDULE.md](SCHEDULE.md)):

- There is **no extra meeting** and the weekly is **not replaced**.
- T-24 includes the [gate brief](templates/gate.md).
- Block 2 is the proposal; block 3 Decision A is **Approve / revise (with conditions) / reject**.
- If two locks land the same week (e.g. Gate 4 + ops checkpoint), they are Decision A and B in the same 25 min. Keep weekly option-sets to what fits.
- Downstream impact (what is unblocked / now out of scope) is covered in block 4.

### Decision rule (weekly)

- Malte **proposes** 2–3 decisions on a topic with structured options and advantages/disadvantages, if a decision is needed.  
- Daniel **chooses** (or rejects the set and asks for revised options).  
- Choices that later work depends on → [decisions/DECISION-LOG.md](../decisions/DECISION-LOG.md) same day.  
- Formal program gates (beachhead, GTM, brand, etc.) still use the gate template as the T-24 brief when locking those milestones.


### After (Malte, same day)

Required — same day, before pinging Daniel:

1. **Minutes:** `notes/YYYY-MM-DD-weekly.md` using [templates/weekly-session.md](templates/weekly-session.md)
2. **Decision log:** chosen decisions (including any gate outcome) in [decisions/DECISION-LOG.md](../decisions/DECISION-LOG.md)
3. **STATUS:** Malte updates [STATUS.md](../STATUS.md) — week number, current block, phase focus, next gate, open blockers, this week’s deliverables, and any gate row that changed
4. Phase READMEs if status changed
5. Ping Daniel with paths to minutes + STATUS for review


### Roles in the room


| Malte                                                                                          | Daniel                                                                                     |
| ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Leads agenda; presents results; frames decisions; **same day:** minutes, decision log, STATUS | Pre-reads; discusses findings; **chooses** among prepared options; clears blockers he owns |


---



## 3. Gate lock (written pack — decided in the weekly)

**Goal:** **Lock** a decision so later work can depend on it. The lock happens in that week’s 60-minute session, not in a separate meeting.

**Before (Malte, in the T-24 pack):**

- Complete phase deliverables (see [PLAN.md](../PLAN.md))
- Write gate brief using [templates/gate.md](templates/gate.md) → `notes/YYYY-MM-DD-gate-N-brief.md`
- Propose decision text ready to paste into the decision log
- Attach the brief path in the T-24 pack at least 24h ahead

**In the weekly (blocks 2–4):** proposal → challenge → **Approve / revise (with conditions) / reject** → what this unblocks.

**After (Malte, same day):**

- Log decision in `decisions/DECISION-LOG.md` with status `accepted` / `accepted-with-conditions` / `rejected`
- If conditions: checklist in the phase README until cleared
- Record the outcome in the weekly session notes (no separate gate-meeting note)
- Update [STATUS.md](../STATUS.md) (gates table + next gate + blockers)

**Rules:**

- No silent locks — if it isn’t in the decision log, it isn’t locked.
- Rejecting is OK; week plan adjusts; buffer exists for rework.
- Do not schedule a follow-up review meeting. If the pack is rejected, revise in the repo and bring it back at the next weekly.

---



## 4. What we do *not* use meetings for

- A second live session in the same week (gate, review, or “quick follow-up”)
- Reading entire documents aloud (Daniel pre-reads the T-24 pack)
- Discovering the week’s work for the first time in the room (must be in repo at T-24)
- Daniel inventing option analysis from scratch (Malte prepares options + pros/cons)
- Re-opening a locked gate without a new decision entry
- Engineering implementation detail beyond what handoff needs

---



## Notes folder convention

```text
meetings/notes/YYYY-MM-DD-kickoff.md
meetings/notes/YYYY-MM-DD-weekly-t24.md    # due 24h before
meetings/notes/YYYY-MM-DD-weekly.md        # after the session
meetings/notes/YYYY-MM-DD-gate-N-brief.md  # T-24 attachment on gate weeks (not a meeting)
```

Keep notes short; put lasting artifacts in `docs/phases/`.
