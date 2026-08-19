# 07-T1 — Search profiles & dictionary keep/cut/add

| Field | Value |
| --- | --- |
| **Task ID** | `07-T1` |
| **Phase** | [07-data-matching](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [DATA-DICTIONARY.md](../DATA-DICTIONARY.md) · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Both sides have a **search profile**. Seeded dictionary tables need keep / cut / add decisions (with types and privacy notes) so Week 7 screens and Gate 4 matching share one field set.

---

## Our guideline

- **Both sides, one dictionary.** Seeker profile + search fields; company profile + job requirement fields — same conceptual model.
- **Decide in the dictionary.** Mark keep/cut/add in [DATA-DICTIONARY.md](../DATA-DICTIONARY.md) tables — not as Q&A on this page.
- **Align with MVP screens.** Fields no MVP screen collects or shows are a common pitfall; cross-check Phase 06 inventories as you go.
- **Required before match.** For seeker and job: which fields must exist before matching runs? What happens if missing?
- **Types and privacy now.** Kept rows need type, required flag, example, and privacy notes in the dictionary.

| Term | Plain meaning |
| --- | --- |
| **Search profile** | Structured preferences + constraints used to find the other side |
| **Profile fields** | Facts about the person or company/job |

---

## What we have done before

This is the **first task in Phase 07**. You start from seeded data stubs and product/beachhead context:

- [DATA-DICTIONARY.md](../DATA-DICTIONARY.md) — seeded seeker, company, and job field tables
- [decisions/DECISION-LOG.md](../../../../decisions/DECISION-LOG.md) — **Gate 1** beachhead (niche × geography drives which fields matter)
- [Phase 06 — product](../../06-product/README.md) — [MVP-SCREEN-INVENTORY.md](../../06-product/MVP-SCREEN-INVENTORY.md) screen expectations (align as T6 product work progresses)
- [Phase 05 — brand](../../05-brand/README.md) — fairness and tone constraints that affect field labeling (Gate 3)
- [PRODUCT-CONCEPT.md](../../06-product/PRODUCT-CONCEPT.md) — which profile data the product concept assumes

---

## What we're doing now

**Goal:** Keep/cut/add dictionary fields with types and privacy notes, and define required-before-match behavior for seeker and job.

Example questions (inspiration — mark decisions in the dictionary, not as Q&A here):

- In your own words: what is a **search profile**, and why do **both** seekers and companies have one?
- For **Seeker — profile fields** in [DATA-DICTIONARY.md](../DATA-DICTIONARY.md): which rows **keep / cut / add**? Summarize cuts and any new fields somewhere durable.
- Same for **Seeker — search / constraint fields**.
- Same for **Company — profile** and **Job — requirement** tables. For kept job fields: **must**, **nice**, or **n/a**?
- Which kept fields are **required** before matching can run for (a) seeker, (b) job? What happens if missing?

You might work row-by-row in the dictionary tables — preferred over a worksheet form.

**Start here**

1. Read DATA-DICTIONARY seeded tables + Phase 06 screen expectations.  
2. Keep/cut/add with types and privacy notes in the dictionary.  
3. Note required-before-match fields and missing-field behavior.  
4. Link from the worksheet.  

---

## Why it matters

**For the rest of Phase 07:** [T2](07-T2-SEARCH-DIMENSIONS.md) dimensions map to kept fields. [T3](07-T3-ACQUISITION.md) assigns methods per kept field. [T4](07-T4-MATCHING-RULES.md) hard/soft rules reference this set.

**For Daniel:** Decided field set for Week 7 product alignment and **Gate 4** — required vs optional clarity for matching fail behavior.

**For later phases:** Phase 06 inventories and Figma must stay synced with final field names; Phase 08 ops needs to know which fields are first-party vs ingested.
