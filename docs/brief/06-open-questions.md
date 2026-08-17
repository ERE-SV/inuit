# Open questions

Decision backlog. Move items into numbered docs when resolved; leave a one-line “Resolved: …” note here or delete the item.

---

## Strategy & niche

- [ ] **Exact beachhead niche** — IT/consultants, bankers, other? (criteria in [03-gtm-niche.md](03-gtm-niche.md))
- [ ] **Geography** — Zurich-only first? How far into CH/DACH later?
- [ ] **First-wave seeker acquisition** — channels, partnerships, university hooks
- [ ] **Company acquisition motion** — outbound after forwards vs inbound claim flow

---

## Product & matching

- [ ] **Matching algorithm detail** — weights, thresholds, Top-X size (fixed vs adaptive)
- [ ] **Subjective factors** (culture, weekend willingness, etc.) — structured tags vs inference vs out of automation
- [ ] **Commute modeling depth** — tram-line aware vs minute isochrones; data vendors
- [ ] **Soft preference UX** — what must be explicit vs inferred
- [ ] **Uncertainty communication** — “estimated” / “self-reported” / “market benchmark” without overload
- [ ] **Profile visibility** — consent per employer, visibility tiers, docs on request
- [ ] **Career-gap** — min N per cohort; role taxonomy (custom vs ESCO/O*NET); live vs archived jobs
- [ ] **What-if / relaxation** — which constraints may loosen; how many scenarios; naming alternate cities
- [ ] **Cover letter / free text** — employer setting “required yes/no” for pilot segment
- [ ] **ATS handoff** — PDF/CSV/API export enough for beachhead?

---

## Privacy & compliance

- [ ] **CH/EU data-handling approach** — DPIA triggers, retention, subprocessors, regions
- [ ] **Crawl / ToS legality** per source; robots.txt policy; employer opt-out SLA
- [ ] **Enrichment licenses** (salary, culture aggregators) — who is liable for bad matches
- [ ] **Discrimination / fairness** — which criteria must never be automated
- [ ] **Voice capture** (if pursued) — recording consent, vendor regions, retention of audio vs transcript

---

## Monetization

- [ ] **Precise billable events** — match shared, interview booked, hire, other?
- [ ] **Price points** vs ~2–3k CHF listing baseline (validate real listing prices)
- [ ] **Seeker freemium boundaries** — what is free forever vs premium
- [ ] **Employer packaging** — pure performance vs hybrid subscription
- [ ] **Data products timing** — when insights/benchmarking are ethical and useful enough to sell

---

## Technical feasibility

- [ ] **Scalable crawling + matching** — unit cost, freshness SLAs, dedupe across sources
- [ ] **1–3 feed/API providers** for CH — contract, cost, field coverage, redundancy
- [ ] **Crawl remainder surface** — max allowlist size; legal sign-off process
- [ ] **Cloud region** — CH/EU preference
- [ ] **Push feed vs polling** for Phase-3 API
- [ ] **Build vs buy** for ingestion pieces

---

## Validation work (next research steps)

1. One-sentence positioning for a chosen niche (not “all jobs”).  
2. 10–15 interviews: ~5 HR leads, ~5 active seekers — quantify time, cost, tools.  
3. Competitor matrix: pricing + features of 3–5 alternatives.  
4. Paper prototype / journeys (seeker + company) including status overview.  
5. Business-model sketch with 2 variants and break-even assumptions.  
6. Feed/API due diligence: shortlist, sandbox, field mapping, cost calculator.  
7. Legal/risk review for feeds and residual crawl (CH) before broad rollout.  
8. Architecture spike (1–2 weeks): ingest → normalize → store → metrics + runbook draft.
