# Technical feasibility

## Roles & data objects

| Role | Platform job | Objects |
| --- | --- | --- |
| **Company** | Publish roles as structured requirement profiles (not only marketing text) | Search/requirement profile(s) per role or talent pipeline |
| **Seeker** | One-time rich profile + search criteria for matching | Candidate profile + search profile |

**Matching:** seeker search profile ↔ job requirements; employer search profile ↔ candidate profile. Constraint satisfaction + overlap where categories pair.

---

## Ingestion strategy (reconciled)

**Bootstrap (GTM):** Crawl / ingest from main Swiss job platforms and selective career pages so the product works before employers onboard.

**Preferred at scale:** Official **APIs or licensed feeds** from a small number of major listing providers (~3 as working hypothesis — validate contracts, cost, fields, freshness). Engineering focus: normalize, dedupe, quota management — not N fragile HTML parsers.

**Career-site crawl:** Optional gap-filler on an allowlist; not the primary scale strategy. Check ToS, robots.txt, employer relationship, and opt-out before expansion.

### Ingestion subsystem (sketch)

1. **Registry & discovery** — employer registry, career URLs, ATS templates (Workday, Greenhouse, custom HTML)  
2. **Scheduling** — hot/warm/cold priority, change detection (ETags, hash), SLAs per tier  
3. **Fetch** — polite rate limits, backoff, captcha → escalation  
4. **Extract & normalize** — versioned adapters, schema mapping; LLM with confidence + human-in-the-loop  
5. **Lineage** — canonical URL, fetch time, parser version, raw hash; retention rules  
6. **QA** — extract rate, field completeness, drift monitoring, relaunch regression  
7. **Compliance-by-design** — allowlists, opt-out, robots.txt, staging → review → publish  
8. **Observability** — success, latency, queue, error classes, cost; runbooks  
9. **Ownership** — clear “ingestion” vs domain owners; on-call for parser breaks  

### Phase implications

| Phase | Source | Confidence |
| --- | --- | --- |
| Phase 1 | Feeds/APIs + selective crawl; LLM extraction from free text | Lower — label as inferred |
| Phase 2 | First-party employer data | Higher — Phase-1 as backfill |
| Phase 3 | Company push API | Highest freshness & consent |

---

## Enrichment sources (where employers omit fields)

| Topic | Possible sources | Caution |
| --- | --- | --- |
| Workplace / location | Employer fields, geocoding, commercial register | Multi-site accuracy |
| Commute / transit | Maps APIs, CH open transit data | Cost per request; privacy of home location |
| Salary / benchmarks | Aggregators, BFS / industry studies | Contracts; never invent individual salaries |
| Culture / employer brand | Review sites via allowed interfaces | Aggregate vs anecdote |
| Job requirements | Listing feeds (P1), first-party profiles (P2) | Free-text extraction uncertainty |

**Pareto:** map the most common seeker constraints → fields → legal sources → fallback when missing.

---

## Matching algorithm (feasibility notes)

**Near-term (feasible):** hard filters + weighted soft scores on structured fields; explainable Top-X; thresholds per niche.

**Harder (open):** culture and other subjective factors — need either:

- Structured self-description on both sides (e.g. values tags, work-style scales), or  
- Careful inference from text with low weight and transparency, or  
- Human confirmation before contact  

Bias, gaming, and fairness reviews are first-class — not afterthoughts.

**Commute:** isochrones / transit minutes likely better than “same city” alone; depth TBD (line-aware vs minutes).

---

## Privacy, consent, data handling (CH / EU)

Must be designed in from day one (nDSG / GDPR-aligned):

- Purpose limitation and data minimization  
- Consent for sensitive uses (home address for commute matching; recording if voice used)  
- Server-side matching — employers need not see raw home address  
- Visibility tiers for seeker profiles; certificates on request  
- Source labels for inferred employer attributes; correction / claim / opt-out flows  
- Retention of raw crawl vs derived structured fields  
- No prohibited automated discrimination criteria  

Legal review before broad crawl or third-party enrichment.

---

## Voice / conversational capture (later option)

Idea: AI agents call seekers (voice API), dialogue fills schema, user confirms in UI.

| Requirement | Note |
| --- | --- |
| Transparency | Disclose bot; purpose; retention |
| Confirmation | UI review before matching write |
| Accessibility | Voice optional; text/UI always available |
| Compliance | Recording consent; no voice biometrics; EU/CH regions |
| Safety | Bound question scope; no health/bank data over insecure channels |

Validate **after** form-based onboarding MVP (completion rate, data quality, cost/minute).

---

## Feasibility risks (technical)

| Risk | Mitigation |
| --- | --- |
| Parser rot on career-site relaunches | Monitoring, canaries, fast ownership |
| Feed vendor price/limit shocks | Multi-source strategy, exit plan |
| Inferred attributes treated as ground truth | UI labeling; prefer first-party after onboard |
| Employers feel “surveilled” by crawl | Opt-out/claim; clear value prop |
| Match score misread as hire guarantee | Copy, explainability, human confirm before contact |
| Scalable crawl + matching cost | Niche beachhead; API-first where possible; measure unit cost early |

---

## Suggested technical spikes (when building starts)

1. End-to-end ingestion (one feed **or** small crawl allowlist) → normalize → store → quality metrics  
2. Schema for seeker + job requirement profiles + explainable match stub  
3. Privacy threat model for commute + enrichment fields  
4. Cost model: fetch / LLM extract / routing API per active seeker  

See also next steps in the archived German brainstorm and [06-open-questions.md](06-open-questions.md).
