# 07-T3 — Acquisition per field

| Field | Value |
| --- | --- |
| **Task ID** | `07-T3` |
| **Phase** | [07-data-matching](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [DATA-ACQUISITION.md](../DATA-ACQUISITION.md) · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Every kept field needs a method, confidence idea, legal note, and fallback — so Phase 08 ops and Gate 4 eng know how data actually arrives.

---

## Our guideline

- **One method per kept field.** User, feed/API, crawl, enrichment, inferred, or computed — update the acquisition table.
- **Label inferred data.** Bootstrap job requirements from text need UI label + confidence rule (see MVP screens such as MVP-031 / MVP-045).
- **No invented salary or culture.** Enrichment allowed, unknown, or first-party only — say which; never fabricate numbers.
- **Field-level only.** This task assigns a method **per dictionary field**. Primary supply mix narrative (feed vs crawl vs first-party) is **[08-T1](../../08-ops/tasks/08-T1-SUPPLY-APPROACHES.md)** — summarize here only where it affects a field's method.
- **Fallback for hard filters.** If a critical field is missing: skip listing, partial match, or block? Decide per field.

| Method | Meaning | Typical use here |
| --- | --- | --- |
| **User input** | Person or company types it | Seeker profile; first-party job requirements |
| **Feed / API** | Licensed or official listing data | Bootstrap title, location, description |
| **Crawl** | Fetch pages on an allowlist (fragile; legal care) | Gap-filler — not primary scale plan |
| **Enrichment** | Third-party or public datasets | Salary bands, transit — contracts + caution |
| **Inferred** | Model extracts structure from text | P1 requirements from listings |
| **Computed** | Calculated from other fields | Commute minutes from home + workplace |

---

## What we have done before

Build on dictionary and dimensions from T1–T2:

- [07-T1 — Dictionary](07-T1-DICTIONARY.md) — kept fields with types and privacy notes
- [07-T2 — Search dimensions](07-T2-SEARCH-DIMENSIONS.md) — dimensions that may need computed or enriched data
- [DATA-ACQUISITION.md](../DATA-ACQUISITION.md) — seeded acquisition table
- [Phase 06 — product](../../06-product/README.md) — [MVP-SCREEN-INVENTORY.md](../../06-product/MVP-SCREEN-INVENTORY.md) for inferred-field UI (MVP-031, MVP-045)
- [06-T1 — Journeys](../../06-product/tasks/06-T1-VERSIONS-JOURNEYS.md) — bootstrap forward / ingest path

---

## What we're doing now

**Goal:** Assign acquisition method, confidence, legal note, and fallback for every kept field; define feed-vs-crawl and salary/culture policy.

Example questions:

- Default map: which field groups are **user**, **feed/crawl**, **inferred**, **enrichment**, **computed**? Update the acquisition table.
- For **inferred** job requirements in bootstrap: what UI label and confidence rule will you use? (See product screens such as MVP-031 / MVP-045.)
- For **salary** and **culture** gaps: enrichment allowed, unknown, or first-party only? No invented numbers.
- Crawl vs feed: what is primary for MVP listing supply? What is allowlist-only gap-filler?
- Fallback if a hard-filter field is missing: skip listing, partial match, or block? Per critical field.

**Start here**

1. Dictionary kept fields + DATA-ACQUISITION seed.  
2. Assign methods; define inferred labels and salary/culture policy.  
3. Primary supply + fallbacks for hard filters.  
4. Link from the worksheet.  

---

## Why it matters

**For the rest of Phase 07:** [T4](07-T4-MATCHING-RULES.md) fail behavior depends on missing-field fallbacks. [T5](07-T5-PRIVACY-FAIRNESS.md) commute/home acquisition ties to computed fields.

**For Daniel:** Acquisition table for **Gate 4** — eng and ops can see how data arrives without a workshop.

**For later phases:** Phase 08 [T1](../../08-ops/tasks/08-T1-SUPPLY-APPROACHES.md) synthesizes this table into ops mix — do not reassign field methods there.
