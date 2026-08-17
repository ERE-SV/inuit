# Phase 08 — Supply & operations — Worksheet

**Status:** not-started  
**Unlocks:** **Ops checkpoint** (Weeks 10–11) — assumptions accepted as **inputs to the financial model** (Phase 09), not a forever org chart  
**Primary path:** this file  
**Depends on:** Beachhead, GTM, data acquisition approach (Phase 07)  

## Learn (read before working)

### What this phase is

You explain how **job listings get into the product** and how many people (and tools) it takes to keep that supply fresh and sell/support the beachhead. Output feeds finance: cost drivers, headcount timing, and what one person can run alone. Optional dumps: [OPS-MODEL.md](OPS-MODEL.md), [HEADCOUNT-PLAN.md](HEADCOUNT-PLAN.md).

### Ingestion, feeds, and crawl (student level)

Think of listings as inventory in a shop. You need a way to stock the shelves before every employer builds a profile on you.

| Approach | Plain meaning | Pros | Cons |
| --- | --- | --- | --- |
| **Feed / API** | A provider sends structured job data under a contract or partner API | Fresher, more stable fields, clearer rights | Cost, quotas, negotiation; fields may be incomplete |
| **Crawl** | Your software visits career pages (allowlist), downloads HTML, extracts text | Fills gaps; works before partnerships | Breaks when sites redesign; ToS/robots/legal risk; needs babysitting |
| **First-party** | Employer enters or pushes jobs on your platform | Highest trust and consent | Needs sales/onboarding; slow for bootstrap |
| **Inferred fields** | LLM/rules turn free text into skills/years/etc. | Unlocks matching early | Lower confidence; must label; QA cost |

**Ingestion** = the whole pipeline: discover sources → fetch on a schedule → extract/normalize → QA → publish with lineage (where it came from).  
**Ops** for ingestion ≠ “one script forever” — someone watches breakage, quotas, and quality.

### Key terms

| Term | Meaning in plain language | Why it matters here |
| --- | --- | --- |
| **Freshness** | How recently a listing was checked/updated | Stale jobs destroy seeker trust |
| **Allowlist** | Explicit list of sites/employers you may crawl | Compliance-by-design; not “crawl the whole internet” |
| **Parser / adapter** | Code that understands one site or feed format | Each new source = maintenance cost |
| **Lineage** | Source URL, fetch time, parser version | Debugging + trust labels in UI |
| **Headcount plan** | Who you hire, when, for which milestone | Finance opex; hiring triggers |
| **Sales motion** | How company acquisition works (forward-loop vs cold listing sales) | Sales headcount must match GTM |
| **Cost driver** | Something that makes spend go up with volume | Phase 09 model inputs |

### Common beginner mistakes

- Assuming crawl is “free” (ignore legal + engineer time)  
- Planning a 10-person ops team before MVP liquidity  
- Sales headcount that ignores GTM forward-motion (prove candidates first)  
- No hiring trigger (“we’ll know when it’s painful” with no metric)  
- Forgetting support load when both sides get notifications  
- Cost drivers as vague “tech” instead of vendors, seats, API calls, salaries  

## How to prove answers

- Ops choices → paths in OPS-MODEL / HEADCOUNT-PLAN / evidence  
- Legal posture = summary + “flag for counsel,” not invented permissions  
- Headcount timing tied to GTM milestones / Gate 2  
- Label inferences; cite vendor pricing pages when claiming CHF costs  
- Follow [RESEARCH-STANDARD.md](../../../RESEARCH-STANDARD.md)  

## Tasks

### [ ] 08-T1 — Learn supply approaches for this product

**Done when:** You can explain feed vs crawl vs first-party in your own words and pick an MVP mix.  
**Unlocks / feeds:** Ops model table; finance cost drivers  

#### Sub-questions

- [ ] **08-T1-Q1.** Explain **ingestion**, **feed/API**, and **crawl** in ≤3 sentences each, using this product as the example.
  - **Answer:**  
  - **Proof:** (path: brief `05-tech-feasibility.md`)  

- [ ] **08-T1-Q2.** For MVP beachhead: what is the **primary** listing supply approach, and what is **secondary**? Why?
  - **Answer:**  
  - **Proof:** (inference from GTM + Phase 07 acquisition)  

- [ ] **08-T1-Q3.** When do **first-party** employer profiles become the main path (link to GTM stage / product Phase 2)?
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T1-Q4.** What does “label inferred requirements” mean for ops (QA, support tickets, employer complaints)?
  - **Answer:**  
  - **Proof:**  

### [ ] 08-T2 — Ops model: sources, legal posture, freshness

**Done when:** [OPS-MODEL.md](OPS-MODEL.md) has a filled supply table + freshness/quality hypotheses.  
**Unlocks / feeds:** Ops checkpoint; Phase 09  

#### Sub-questions

- [ ] **08-T2-Q1.** Fill the supply table: Feed/API | Crawl (allowlist) | First-party — role in MVP, legal posture **summary**, freshness assumption.
  - **Answer:**  
  - **Proof:** (path: `OPS-MODEL.md`)  

- [ ] **08-T2-Q2.** Freshness SLA hypothesis: how often must hot listings be re-checked? What is “too stale” for the beachhead?
  - **Answer:**  
  - **Proof:** (inference labeled)  

- [ ] **08-T2-Q3.** Quality checks: name ≥3 metrics you would watch (extract rate, field completeness, duplicate rate, etc.).
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T2-Q4.** Opt-out / claim: what happens operationally if an employer wants listings removed or corrected?
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T2-Q5.** Risks if parsers break after a career-site relaunch — who is on-call in MVP (role, not person’s name)?
  - **Answer:**  
  - **Proof:**  

### [ ] 08-T3 — Headcount: crawlers/ingestion vs sales vs support

**Done when:** [HEADCOUNT-PLAN.md](HEADCOUNT-PLAN.md) states counts, timing, skills, and what one person covers alone.  
**Unlocks / feeds:** Finance opex; hiring plan  

#### Sub-questions

- [ ] **08-T3-Q1.** **Ingestion / crawler maintenance:** how many people for MVP? Skills required? What can **one** person cover alone?
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T3-Q2.** **Sales:** how many for MVP? How does the role map to GTM (forward qualified candidates vs selling listing slots)?
  - **Answer:**  
  - **Proof:** (path: `../04-gtm/…`)  

- [ ] **08-T3-Q3.** **Support** (seeker + company): needed at MVP? Part-time founder-led vs hire #1?
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T3-Q4.** Any **other** role required for MVP ops (e.g. part-time data QA)? Justify or write `none`.
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T3-Q5.** Compare: is early headcount heavier on **ingestion engineering** or **sales**? Why for *this* bootstrap GTM?
  - **Answer:**  
  - **Proof:**  

### [ ] 08-T4 — When to hire (triggers)

**Done when:** Hiring triggers are measurable (volume, breakage, response time), not vibes.  
**Unlocks / feeds:** Milestone projections in finance  

#### Sub-questions

- [ ] **08-T4-Q1.** When do you hire ingestion person **#2**? Give a trigger (e.g. sources > N, weekly breakages > N, or hours/week > N).
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T4-Q2.** When do you hire sales person **#1** or **#2**? Tie to GTM milestones (e.g. forwards/week, onboarded employers).
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T4-Q3.** What does **one founder + one hire** run vs what waits until revenue or funding?
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T4-Q4.** Fill the hiring-trigger table in HEADCOUNT-PLAN (Trigger → Hire).
  - **Answer:**  
  - **Proof:**  

### [ ] 08-T5 — Cost drivers for finance

**Done when:** OPS-MODEL lists concrete cost drivers Phase 09 can model (tools, vendors, time).  
**Unlocks / feeds:** Phase 09 financial model  

#### Sub-questions

- [ ] **08-T5-Q1.** List cost drivers for **listing supply** (feed fees, proxy/captcha, LLM extract, maps/transit APIs, cloud). Mark known CHF vs `unknown`.
  - **Answer:**  
  - **Proof:** (URLs for any priced items — accessed YYYY-MM-DD)  

- [ ] **08-T5-Q2.** List cost drivers for **people** (roles × rough timing). No fake salaries — use ranges only if sourced, else `unknown` + placeholder for finance.
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T5-Q3.** List cost drivers for **support/compliance ops** (tools, counsel buffer flag).
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T5-Q4.** Which cost drivers **scale with** active seekers, active jobs, or employers onboarded? (Unit drivers for the model.)
  - **Answer:**  
  - **Proof:**  

- [ ] **08-T5-Q5.** One-paragraph **ops checkpoint summary** for Daniel: supply approach, headcount shape, top 5 cost drivers.
  - **Answer:**  
  - **Proof:** (path: `OPS-MODEL.md` or `evidence/ops-checkpoint.md`)  

## Gate / checkpoint pack — Ops checkpoint

Daniel accepts as **finance inputs** (not eternal org design):

- [ ] Listing supply approach (feeds/APIs vs crawl) + legal posture summary  
- [ ] Freshness / quality assumptions  
- [ ] Headcount: ingestion — how many, when, skills  
- [ ] Headcount: sales — how many, when, motion link to GTM  
- [ ] Support / other roles if needed for MVP  
- [ ] What one person can run vs when to hire #2  
- [ ] Cost drivers listed for Phase 09  

## Handoff to next phase

Phase 09 (finance) will consume:

- Supply cost drivers and unit drivers (per seeker / job / employer)  
- Headcount timing by milestone  
- Freshness assumptions that affect retention/churn hypotheses  

Phase 10 (risk) will consume:

- Crawl/ToS legal posture flags  
- Single-person bus factor on ingestion  
