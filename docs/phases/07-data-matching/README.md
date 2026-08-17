# Phase 07 — Data profiles, acquisition & matching

- **Status:** not-started
- **Block:** B–C (v0 in Week 7; depth Weeks 10–11)
- **Gate:** **Gate 4** (with phase 06)
- **Owner:** Malte

## Deliverables

| File | Required |
| --- | --- |
| [DATA-DICTIONARY.md](DATA-DICTIONARY.md) | Yes *(seeded from brief)* |
| [DATA-ACQUISITION.md](DATA-ACQUISITION.md) | Yes *(seeded methods)* |
| [MATCHING-SPEC.md](MATCHING-SPEC.md) | Yes |
| [SEARCH-DIMENSIONS.md](SEARCH-DIMENSIONS.md) | Yes *(seeded)* |

## Definition of done

- [ ] **Human search profile:** all fields (type, required, example, privacy notes)
- [ ] **Company / job requirement profile:** all fields
- [ ] **Search dimensions:** what seekers filter for; what companies filter for
- [ ] **Acquisition:** for each field — user input / feed-API / crawl / enrichment / inferred + confidence + legal note
- [ ] **Matching:** hard filters, soft scores, Top-X, thresholds, explainability, zero-match behavior
- [ ] Edge cases: asymmetric prefs (e.g. commute), missing data, fairness constraints
- [ ] Implementable by an engineer without a strategy workshop

> This checklist is **canonical DoD**.

## Relationship to Figma

Refine seeded dictionary in **Week 7** before polishing all screens. Keep dictionary ↔ inventories in sync before Gate 4. Week tasks: [PLAN-WEEKS.md](../../../PLAN-WEEKS.md).
