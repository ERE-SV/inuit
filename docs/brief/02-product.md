# Product

## Scope boundaries

**What this is not (employer side):** a full ATS replacement. No internal approvals, interview scheduling as a product core, or full stage tracking inside the company stack — that stays in existing ATS / HRIS / calendar / email.

**Employer core:** HR sees **far fewer** applications, but only **pre-qualified** candidates (Top-X, match thresholds).

**Seeker core (intentionally broader):**

- One profile + search criteria; platform handles matching, Top-X roles, profile reuse, overview, notifications.
- Interviewing, offers, and domain judgment stay with the employer.
- A seeker-side pipeline view (own applications / status) is in the vision; it is not an employer ATS.

---

## Profiles

### Job seekers

- Education, grades, skills, experience, certificates, languages.
- Search preferences / constraints: role, location & commute, salary floor, company size/culture/age, work model, etc.
- Optional soft preferences where they can be modeled safely.

### Companies & jobs

- Company profile: culture, values, salary ranges, size, locations, work model.
- Per-role **structured requirement profile** (must-haves / nice-to-haves) — not only marketing copy.
- Storytelling optional; filters are first-class.

### Naming

“Search profile” fits both sides: companies search for people; seekers search for opportunities.

---

## Bidirectional matching

| Direction | Question |
| --- | --- |
| Seeker → job | Does this role satisfy the seeker’s constraints? (job facts + enrichment) |
| Company → seeker | Does this person meet the role requirements? (direct profile compare) |

Where categories pair (language level, remote share, etc.), true **overlap** can be scored. High compatibility is an **indicator**, not a hiring promise.

**Output:**

- Top-X jobs for seekers; Top-X candidates for employers.
- Short rationale: which criteria hit / missed.
- Both sides notified on strong fit → path to **book an interview**.

### Hard vs soft factors

- **Objective:** degrees, certificates, years, languages, commute, salary bands — good first automation layer.
- **Subjective** (culture fit, weekend willingness, team vibe): high value for niche differentiation, but harder to encode without gaming or bias. Treat as open design work — see [06-open-questions.md](06-open-questions.md).

---

## Product phases

| Phase | Data basis | Implication |
| --- | --- | --- |
| **Phase 1 — Bootstrap** | Ingest existing Swiss listings (platforms + selective career pages); infer structured requirements from text | Lower confidence; show source/“derived from listing” in UI; deliver value by forwarding relevant candidates to companies |
| **Phase 2 — Onboarded employers** | First-party company & job profiles on the platform | Higher precision; Phase-1 data as backfill / validation |
| **Phase 3 — Direct supply** | Companies push listings via **API** (career-site → platform) | Less scrape fragility; sticky B2B integration |

Phase 1 is the go-to-market wedge (see [03-gtm-niche.md](03-gtm-niche.md)), not the long-term data model.

---

## Adjacent product ideas (post-MVP value)

### Career-gap / “career radar”

From aggregated job requirements, show seekers which qualifications are typically missing for a **target role** (must-have vs frequent; with sample size).

- Supports retention after placement — users return to prepare the *next* move.
- Communicate carefully: “based on N roles on our platform,” not absolute market truth.
- Cohort norms only (min sample, anonymization); disclaimer; not a regulated career-advice substitute.

### Zero-match diagnosis & what-if

When constraints yield zero or weak matches, suggest **minimal** relaxations (salary floor, radius, remote, cert) with expected gain (“loosening A unlocks Z more roles”).

- Relocation / pay tradeoffs must stay optional, neutral, user-owned.
- Treat distant labor markets (e.g. Chur vs Zurich) as different markets in UX — not “just expand 15 km.”

### Market intelligence (company-facing, later)

Advise how changing salary or criteria affects applicant volume; salary benchmarking; anonymized insights for research / partners.

### Profile capture UX

Rich structured data is required; giant forms kill completion.

- Guided wizards first.
- Optional later: conversational / **voice** capture (outbound AI calls) with opt-in, transcript confirmation in UI, CH/EU compliance — after a form-based core is validated. Details in [05-tech-feasibility.md](05-tech-feasibility.md).

---

## Explicit non-goals (near term)

- Replacing ATS workflows end-to-end.
- Guaranteeing hires from match scores.
- Covering every Swiss role/geography at once (niche beachhead first).
- Motivational-letter factories (signal, not more AI noise).
