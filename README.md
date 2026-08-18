# Job Portal — Company definition (source of truth)

This repository is the **handoff package and living source of truth** for turning the job-marketplace idea into a buildable company plan.

It is **not** the engineering codebase yet. When this program is complete, an engineer should be able to start from this repo (especially `docs/phases/11-handoff/`) plus Figma links without reconstructing context from chat.

## Start here

| If you are… | Read |
| --- | --- |
| Malte (first day) | [ONBOARDING.md](ONBOARDING.md) → [WORKSHEET-GUIDE.md](docs/phases/WORKSHEET-GUIDE.md) |
| New to the project | [CHARTER.md](CHARTER.md) → [docs/brief/](docs/brief/) |
| Checking progress | [STATUS.md](STATUS.md) · [meetings/SCHEDULE.md](meetings/SCHEDULE.md) |
| Running the 16-week program | [PLAN.md](PLAN.md) + [PLAN-WEEKS.md](PLAN-WEEKS.md) + [meetings/README.md](meetings/README.md) |
| Writing research | [RESEARCH-STANDARD.md](RESEARCH-STANDARD.md) |
| Looking for a locked decision | [decisions/DECISION-LOG.md](decisions/DECISION-LOG.md) |
| Taking engineering handoff | [docs/phases/11-handoff/](docs/phases/11-handoff/) |

## Repo map

```text
README.md                  You are here
ONBOARDING.md              Malte first-week guide
CHARTER.md                 Mandate, scope, roles, success criteria
PLAN.md                    16-week plan, gates, linked stubs
PLAN-WEEKS.md              Week-by-week task checklist (14 work + 2 buffer)
STATUS.md                  Current week, gates, blockers
RESEARCH-STANDARD.md       Evidence & citation bar

docs/
  brief/                   Pre-hire ideation (starting assumptions)
  phases/01–11/            Each phase: WORKSHEET.md (primary guided tasks)
  archive/                 Frozen original German brainstorm

decisions/                 Decision log + templates
meetings/                  Cadence, SCHEDULE, templates, minutes, transcripts
.cursor/rules/             Cursor rules for work in this repo
```

## Program snapshot

- **Duration:** **16 weeks total** (14 weeks planned work + **2-week buffer**)
- **Malte's scope:** Strategy through brand principles, full Figma (MVP/V2/V3), data & matching specs, ops & finance — **no coded frontend**
- **Research style:** Desk research, **fact-based and sourced** (not interview-led)
- **Governance:** One **60 min** weekly session (**Malte leads**, T-24 pack). Formal **gates** lock in that same slot (Malte proposes → Daniel chooses/approves). No extra review meetings.
- **Method:** Decision-first spiral — lock beachhead early; UI only after brand principles

## Phase index

| # | Phase folder | Gate? |
| --- | --- | --- |
| 01 | [Market](docs/phases/01-market/) · [task briefs](docs/phases/01-market/tasks/README.md) | — |
| 02 | [Competitive](docs/phases/02-competitive/) | — |
| 03 | [Beachhead](docs/phases/03-beachhead/) | **Gate 1** |
| 04 | [Go-to-market](docs/phases/04-gtm/) | **Gate 2** |
| 05 | [Brand](docs/phases/05-brand/) | **Gate 3** |
| 06 | [Product / Figma](docs/phases/06-product/) | Scope checkpoint + **Gate 4** (with 07) |
| 07 | [Data & matching](docs/phases/07-data-matching/) | **Gate 4** |
| 08 | [Ops](docs/phases/08-ops/) | Checkpoint |
| 09 | [Finance](docs/phases/09-finance/) | **Gate 5** |
| 10 | [Risk](docs/phases/10-risk/) | **Gate 6** (with handoff) |
| 11 | [Handoff](docs/phases/11-handoff/) | **Gate 6** |

Status and definition of done live in each phase `README.md`.
