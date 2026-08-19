# 06-T3 — MVP screen inventory

| Field | Value |
| --- | --- |
| **Task ID** | `06-T3` |
| **Phase** | [06-product](../README.md) |
| **Track progress on** | [WORKSHEET.md](../WORKSHEET.md) |
| **Put your work** | [MVP-SCREEN-INVENTORY.md](../MVP-SCREEN-INVENTORY.md) (change log) · notes of your choice |

This file is **context and inspiration**. Do not fill it in.

---

## Why this exists

Seeded inventory rows are the starting map for MVP Figma. Decide keep / cut / rename / split / add so flows still cover the core loop — do not silently delete rows without a change log.

---

## Our guideline

- **Row-by-row decisions.** Walk MVP-000 … MVP-061 (or current seed range): keep / cut / rename / split / add.
- **Log every change.** Update the inventory change log with a date — silent deletes break Gate 4 sync.
- **Close the core flows.** Flow 1 (seeker signup → first matches), Flow 2 (company → Top-X), Flow 3 (strong fit → interview interest) must still complete.
- **Place consent and empty states.** Privacy / commute consent and empty-match behavior need explicit Screen IDs and version placement (MVP vs V2).
- **An inventory is a contract.** Purpose, actions, data, states per screen — engineer + Daniel use it to audit Figma.

Work directly in the inventory table + change log — preferred over a separate form.

---

## What we have done before

Build on locked feature scope from T2:

- [06-T2 — Feature lists](06-T2-FEATURE-LISTS.md) — locked (or draft-for-checkpoint) MVP feature set
- [06-T1 — Versions, journeys](06-T1-VERSIONS-JOURNEYS.md) — seeker/company paths, bootstrap forward, non-goals
- [MVP-SCREEN-INVENTORY.md](../MVP-SCREEN-INVENTORY.md) — seeded screen rows and change log
- [VERSION-MAP.md](../VERSION-MAP.md) — feature-to-version map from T2

---

## What we're doing now

**Goal:** Decide keep/cut/rename/split/add for every MVP inventory row and confirm Flows 1–3 still close, including consent and empty-match placement.

Example questions:

- Walk [MVP-SCREEN-INVENTORY.md](../MVP-SCREEN-INVENTORY.md) row by row (MVP-000 … MVP-061). Mark each: **keep / cut / rename / split / add**. Summarize cuts and adds somewhere you can find later.
- Which screens are required for Flow 1 (seeker signup → first matches)? List Screen IDs.
- Which screens are required for Flow 2 (company → Top-X) and Flow 3 (strong fit → interview interest)?
- Empty-match behavior: MVP message-only vs V2 what-if — confirm version placement and which screen shows it.
- Privacy / commute consent: which Screen ID owns it, and what happens if the user declines?

**Start here**

1. Open MVP inventory + locked feature lists from 06-T2.  
2. Decide row by row; update the change log with a date.  
3. Check Flows 1–3 still close.  
4. Link from the worksheet.  

---

## Why it matters

**For the rest of Phase 06:** [T4](06-T4-FIGMA.md) frames must match inventory Screen IDs. Week 10 dictionary ↔ Figma sync checkpoint with Phase 07.

**For Daniel:** Inventory decisions for MVP Figma and the scope checkpoint — auditable, not ad hoc frames.

**For later phases:** Phase 07 consent / empty-match / explainability rules must align with Screen IDs you place here.
