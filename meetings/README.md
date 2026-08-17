# Meetings

## Calendar (set at kickoff)

| Ritual | Default | Length |
| --- | --- | --- |
| Weekly working session | Same weekday/time each week; **Malte leads** | 60–90 min |
| Gate meeting | When pack is ready (often replaces weekly that week) | 45–60 min |
| T-24 pack | **24 hours before** weekly: all content in repo + agenda + 2–3 decision proposals | Written |

**Real dates live in [SCHEDULE.md](SCHEDULE.md)** (program start/end, all 16 weeks, meeting + T-24 + gate targets).

Quick mirror (keep in sync with SCHEDULE):

| Field | Value |
| --- | --- |
| **Program start** | _TBD_ |
| **Program end** | _TBD_ |
| **Weekly slot** | _TBD_ (weekday + time + timezone) |
| **Figma workspace / link** | _TBD_ |
| **Async channel** | WhatsApp (or update) |
| **Canonical docs** | **this git repo** |

Also mirror start/end into [STATUS.md](../STATUS.md) and [ONBOARDING.md](../ONBOARDING.md).

---

## 1. Kickoff (once)

**Goal:** Same understanding of charter, repo, and how we work. Malte has completed [ONBOARDING.md](../ONBOARDING.md) Day 0–1 reads beforehand when possible.

### Kickoff checklist

**Before**

- [ ] Malte has repo access + can push/commit
- [ ] Malte has read CHARTER, PLAN, RESEARCH-STANDARD, ONBOARDING
- [ ] Figma seat ready to assign (or create file in-session)

**During — agenda**

1. Walk [CHARTER.md](../CHARTER.md) and [PLAN.md](../PLAN.md) (15 min)
2. Repo tour: phases stubs, decisions, meetings, STATUS (10 min)
3. Tools: git habits, Figma, [RESEARCH-STANDARD.md](../RESEARCH-STANDARD.md) (10 min)
4. **Lock program dates:** start, end (= start + 111 days), weekly weekday/time/timezone (10 min)  
5. Agree who fills [SCHEDULE.md](SCHEDULE.md) and sends 16 calendar invites (5 min)  
6. Agree async channel; Figma access (5 min)  
7. Working preferences / open questions (10 min)

**After (same day)**

- [ ] Fill [ONBOARDING.md](../ONBOARDING.md) program-dates table  
- [ ] Fill [SCHEDULE.md](SCHEDULE.md) — all 16 weeks + gate targets  
- [ ] Fill calendar mirror table above  
- [ ] Send/create **16 weekly** calendar invites (+ kickoff if not done)  
- [ ] Write `notes/YYYY-MM-DD-kickoff.md`  
- [ ] Update [STATUS.md](../STATUS.md) (start, end, Week 1 focus)  
- [ ] Set Figma link in SCHEDULE + `docs/phases/06-product/FIGMA.md` when file exists  

---

## 2. Weekly working session (default every week)

**Goal:** Informed discussion of the week’s findings. Daniel arrives having pre-read the repo; the meeting is for **presentation, challenge, and choices** — not for discovering content for the first time.

**Lead:** Malte runs the meeting and may adjust the agenda (adjustments also filed at T-24 when known).

### T-24 (24 hours before) — Malte

1. **Upload all week’s content** to the repo (phase stubs filled/updated, sources, Figma links as relevant).  
2. File the **T-24 pack** using [templates/weekly-t24.md](templates/weekly-t24.md) → `notes/YYYY-MM-DD-weekly-t24.md`  
   - Predefined agenda (see below)  
   - Paths to artifacts  
   - **2–3 decision proposals**, each with options and **advantages / disadvantages** listed  
3. Ping Daniel (async channel) with the note path so he can pre-read.

**Daniel (before the meeting):** Skim T-24 pack + linked artifacts. Come ready to choose among prepared options.

### Live agenda (Malte leads)

Default 60–90 min. Malte may drop/shorten a block if T-24 already said so, or adjust live if discussion requires it (note the change in session notes).

| # | Block | ~Time | What happens |
| --- | --- | --- | --- |
| 1 | **Review of the week** | ~10 min | What was planned vs done; slips and why |
| 2 | **Presentation of results** | ~20 min | Malte presents findings (substance, not reading docs aloud). Informed discussion — Daniel challenges evidence and implications |
| 3 | **Discussion of decisions** | ~25 min | Malte presents **2–3** prepared decisions with options + pros/cons. **Daniel only chooses** among those options (or sends back for a better option set — does not invent the analysis in the room) |
| 4 | **Adjustment to the plan** | ~10 min | Agree changes to week plan / phase focus / STATUS |
| 5 | **Future outlook** | ~10 min | Next 1–2 weeks: focus and deliverables |
| 6 | **Blockers** | ~5 min | What’s stuck; who unblocks |

If a formal **gate** is due the same week, either fold that gate into the decisions block or replace the weekly with a [gate meeting](#3-gate-meeting-when-a-gate-pack-is-ready) — say which in the T-24 pack.

### Decision rule (weekly)

- Malte **proposes** 2–3 decisions with structured options and advantages/disadvantages.  
- Daniel **chooses** (or rejects the set and asks for revised options).  
- Choices that later work depends on → [decisions/DECISION-LOG.md](../decisions/DECISION-LOG.md) same day.  
- Formal program gates (beachhead, GTM, brand, etc.) still use the gate template when locking those milestones.

### After (Malte, same day)

- Session notes: `notes/YYYY-MM-DD-weekly.md` using [templates/weekly-session.md](templates/weekly-session.md)  
- Log chosen decisions  
- Update [STATUS.md](../STATUS.md) and relevant phase READMEs  

### Roles in the room

| Malte | Daniel |
| --- | --- |
| Leads agenda; presents results; frames decisions | Pre-reads; discusses findings; **chooses** among prepared options; clears blockers he owns |

---

## 3. Gate meeting (when a gate pack is ready)


**Goal:** **Lock** a decision so later work can depend on it.

**Before (Malte):**

- Complete phase deliverables (see [PLAN.md](../PLAN.md))
- Write gate brief using [templates/gate.md](templates/gate.md)
- Propose decision text ready to paste into the decision log
- Async: send pack path + “ask” at least 24h ahead when possible

**Agenda (45–60 min):**

| Block | Time | What we do |
| --- | --- | --- |
| Proposal | 10–15 min | Malte presents recommendation + evidence highlights |
| Challenge | 15–25 min | Daniel questions sources, alternatives, risks |
| Decision | 10 min | **Approve / revise (with conditions) / reject** |
| Downstream | 5–10 min | What becomes unblocked; what is explicitly out of scope now |

**After (Malte, same day):**

- Log decision in `decisions/DECISION-LOG.md` with status `accepted` / `accepted-with-conditions` / `rejected`
- If conditions: checklist in the phase README until cleared
- Gate note in `notes/YYYY-MM-DD-gate-N.md`

**Rules:**

- No silent locks — if it isn’t in the decision log, it isn’t locked.
- Rejecting is OK; week plan adjusts; buffer exists for rework.

---

## 4. What we do *not* use meetings for

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
meetings/notes/YYYY-MM-DD-gate-1-beachhead.md
```

Keep notes short; put lasting artifacts in `docs/phases/`.
