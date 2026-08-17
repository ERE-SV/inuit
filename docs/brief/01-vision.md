# Vision & problem

## Core idea

A **two-sided job marketplace** that replaces traditional applications with **profile-based matchmaking**.

| Side | What they create | What they get |
| --- | --- | --- |
| **Job seekers** (“humans”) | Rich personal profiles (education, grades, skills, experience) plus detailed search preferences (role, location/commute, salary, company culture/age, etc.) | Fewer, better opportunities; less admin; notifications when there is a real fit |
| **Companies** | Detailed company profiles (culture, salary ranges, values) plus precise job requirements | Far fewer unqualified applications; pre-qualified candidates; faster path to interview |

**Loop:** The platform automatically matches both sides and **notifies both when there is a fit** so they can **book an interview**.

**Goal:** Eliminate noise (unqualified applications + endless applying) and make hiring faster and more efficient.

### Market structure

Both sides operate **multi-opportunity**:

- Seekers evaluate many roles at once — not one application, one employer.
- Companies fill multiple vacancies in parallel — not one listing, one candidate.

The market only works with enough **liquidity** (relevant matches) and **trust** (fair, explainable process).

---

## Problems with the current system

Framed against jobs.ch and similar portals.

### For companies / HR

- **Unqualified application flood** → heavy filtering work.
- **Expensive listing** — roughly estimated **2–3k CHF per position** (order-of-magnitude; validate).
- Multi-channel posting (jobs.ch, LinkedIn, career site, etc.) → high total cost, duplicate work, inconsistent messaging.
- Selection is labor-intensive and carries reputation risk (Kununu, Glassdoor).
- Subjective factors often outweigh clean objective screening — yet portals don’t structure those factors well.
- Operational load (routing to hiring managers, interview coordination, stage tracking, rejections, offer/decline, listing upkeep) crowds out real candidate care.

### For job seekers

- Especially graduates: often **40–50 applications** and **3–6 months** to land a role (validate with interviews).
- High admin overhead across many parallel applications.
- Hard to find employers that match combined preferences (e.g. Zurich + short tram commute + company size + salary floor) — classic portals barely support this.
- Weak overview of all open applications and progress.
- **Motivational letters** are largely **AI-generated noise** — low signal for both sides.

### Market / meta

- Classic job boards charge high prices while still delivering noisy inbound.
- HR teams grow around volume screening that is incomplete, unstructured, and only partly rational.
- Two information spaces stay disconnected:
  - Seekers invest in CVs, certificates, cover letters.
  - Companies invest in employer branding, career sites, long job posts.
  - **Gap:** these are rarely matched automatically and structurally; HR does the reconciliation by hand.

### Asymmetric preferences

Seeker and employer preferences do not always share the same dimensions.

*Example:* A seeker cares about max commute time. The company has no “commute” field — the system still needs workplace location + transit data + seeker home (with consent) to evaluate the constraint.

Sensitive employer data (culture, salary bands, team detail) is often unpublished — matching needs **controlled enrichment** from third-party or inferred sources, with transparency and legal care.

---

## Desired outcome

| Stakeholder | Outcome |
| --- | --- |
| Seekers | One reusable structured profile; platform handles as much apply-admin as possible; matches that respect hard preferences |
| Companies | Fewer, better candidates (Top-X above thresholds); less screen time; faster interviews |
| Platform | Trusted match indicator (not a hire guarantee); later career intelligence and retention beyond a single job search |
