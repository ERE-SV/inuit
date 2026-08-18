# 01-T1 — Swiss hiring channels map

| Field | Value |
| --- | --- |
| **Task ID** | `01-T1` |
| **Phase** | [01-market](../README.md) |
| **Answers live in** | [WORKSHEET.md](../WORKSHEET.md) (`01-T1-Q1` … `Q5`) |
| **Week** | 1 (all sub-questions) |
| **Formal gate** | None — feeds Gate 1 later |
| **Optional dump** | [MARKET-BRIEF.md](../MARKET-BRIEF.md) §1 or `evidence/channels-map.md` |

This file is the **assignment definition**. Do not write answers here.

---

## 1. Definition

You produce a **sourced map of where Swiss hiring actually happens today** — the main places seekers find jobs and employers find candidates, including commercial portals, professional networks, company career pages, and public employment (`arbeit.swiss` / RAV), plus relevant DACH channels that Swiss users already use.

For each channel you record:

1. The **seeker’s job** of that channel — one sentence: what the person *hires the channel to do*.
2. The **employer’s job** of that channel — one sentence: what the company *hires the channel to do*.
3. **Public employer pricing**, or `unknown` if not shown. Never invent CHF figures.
4. When a seeker or employer would use **career pages** or **RAV / arbeit.swiss** *instead of* a big portal.
5. How **posting on several channels at once** creates cost or noise for employers (facts + labeled **inference**).

This is **observation of the current market**. You are not recommending a beachhead, a crawl plan, a brand, or a price.

**Done when:** the channels table covers seekers *and* employers for the main CH (+ relevant DACH) paths, every factual cell has proof, and all five worksheet sub-questions are answered.

---

## 2. Why this task exists

The brief assumes classic portals are the status quo: expensive listings, noisy inbound, and employers posting in several places at once. That is a **hypothesis**. T1 is where you check whether the map of channels, the jobs those channels do, and the multi-channel cost/noise story are real enough to carry into competitive teardown and beachhead scoring.

If this map is thin:

- Phase 02 cannot tell **direct** vs **adjacent** competitors (a portal is not the same job as RAV, an agency, or a career site).
- Phase 03 cannot judge **where volume already lives** when scoring niche × geography.
- Later “we are cheaper / less noisy than boards” claims have no observed baseline.

T1 does **not** lock a niche. It locks a shared picture of the field.

---

## 3. Who reads this, and what happens in Week 1

| Who | What they do |
| --- | --- |
| **Malte** | Opens the starter list, fills the table, answers Q1–Q5 with proof, logs URLs in [SOURCES.md](../SOURCES.md). |
| **Daniel (Week 1 weekly)** | Reads the **table + Q5**, not an essay. Reacts: missing channel? which two extras to carry into Phase 02? does multi-channel pain look real enough to keep as a design premise? |
| **Later phases** | Phase 02 consumes channel names as competitor seeds. Phase 03 consumes “where people already look” as a liquidity/geography input. |

There is **no gate this week**. The T-24 pack still needs 2–3 *small* decision options (see §8). Do not ask Daniel to pick a beachhead here.

---

## 4. Guiding context

### What a “channel” is

A **channel** is a place jobs are posted or found — portal, network, career site, public employment, agency. The important question is not “is it famous?” but **what job each side hires it to do**.

Write those jobs as jobs-to-be-done, not as marketing copy.

| Weak | Strong |
| --- | --- |
| “jobs.ch is the biggest Swiss job portal.” | “Seekers use it to browse a large CH inventory and apply with a stored profile; employers buy listings (and extras) to generate inbound applications.” |
| “Everyone uses LinkedIn.” | “Seekers use it as a professional network plus Easy Apply; employers use it for organic posts and/or paid Recruiter / job slots (public pricing: `unknown` if not on the page).” |

### Product thesis this map sits under

The idea is a **two-sided matchmaking marketplace**, not another listing board ([docs/brief/01-vision.md](../../../brief/01-vision.md)). T1 describes the **listing-and-apply world that idea would replace or sit beside**. Keep that contrast in mind when you write “so what” in Q5 — but do not pitch the product in the table. The table is about *them*, not us.

### Brief claims to treat as hypotheses (do not paste as facts)

| Claim in the brief | What T1 should do |
| --- | --- |
| Listings cost on the order of **2–3k CHF per position** | Record **only** what pricing pages show. If not public, write `unknown`. Validation continues in Phase 02 (`02-T3`). |
| Employers post on **several channels** (portal + LinkedIn + career site) → cost and duplicate work | Q5: facts you can see (product pages, “post to multiple boards,” agency upsells) + **inference** labeled. |
| Career pages and public employment are part of the real map | Q4 is required. Do not map only commercial portals. |

### CH vs DACH

Start in **Switzerland**. Add a DACH channel only when Swiss seekers or employers already use it (LinkedIn, XING, Indeed’s DACH surface). Say so in the row. Do not turn this into a Germany market study.

---

## 5. Scope

**In**

- Direct observation of live sites (pricing pages, employer products, seeker apply flow as a *visitor*).
- Commercial portals, professional networks, **company career pages** (pattern, not 50 employers), **arbeit.swiss / RAV**.
- Public pricing or explicit `unknown`.
- A short multi-channel cost/noise note (Q5).

**Out**

- Picking a beachhead or recommending “we should start with X.”
- Full competitor feature matrix (Phase 02).
- Invented prices, traffic ranks, or “talent shortage” numbers.
- Legal conclusion that crawling a site is allowed (flag ToS in [01-T4](01-T4-CONSTRAINTS.md); here you only *see* the channel).
- Interview-led “HR told me…” as the primary evidence (desk-first; [RESEARCH-STANDARD.md](../../../../RESEARCH-STANDARD.md)).

---

## 6. Required output

### Channels table (canonical evidence)

Put the table in [MARKET-BRIEF.md](../MARKET-BRIEF.md) §1 **or** `evidence/channels-map.md`. Point the worksheet **Proof** lines at that path.

Minimum columns:

| Channel | Type | Geography | Seeker job (1 sentence) | Employer job (1 sentence) | Public employer pricing | Source (URL + accessed) |
| --- | --- | --- | --- | --- | --- | --- |
|  | portal / network / public / career site / other | CH / DACH / global-used-in-CH |  |  | figure + URL, or `unknown` |  |

Optional extra columns if useful: “when used instead of a big portal,” “group / owner (e.g. JobCloud).”

### Minimum rows

**Required (worksheet):**

- jobs.ch
- Indeed CH
- LinkedIn
- **Two more** commercial or network channels you actually opened
- Company career pages — **one pattern row** (you may sample 5–10 employers; the row describes the *pattern*, not each firm)
- Public employment — arbeit.swiss / RAV

**Strongly recommended from [SOURCES-STARTER.md](../SOURCES-STARTER.md):** JobCloud / group brands (so you know what sits under jobs.ch), XING, one regional board (e.g. ostjob). If you skip one, say so in Q1 with a reason.

You should be able to count **at least 7 rows** (3 named portals + 2 extras + career-page pattern + public employment). More is fine; depth beats a 20-row directory with empty jobs.

### Worksheet answers

Short. The table does the heavy lifting. Q1 is a visit list. Q2–Q4 can point at table rows. Q5 is 3–5 bullets, not a memo.

---

## 7. Method

1. Open [SOURCES-STARTER.md](../SOURCES-STARTER.md) first. Log every URL you actually use in [SOURCES.md](../SOURCES.md) the same day (URL + access date + tier).
2. Visit as a **seeker** (search, apply CTA, profile) and as an **employer** (post-a-job / products / pricing). Write one sentence per side from what you *saw*, not from memory.
3. Pricing: screenshot or quote the page if a number is public; otherwise `unknown`. The brief’s 2–3k CHF figure is **not** a source.
4. Career pages: sample 5–10 employers in the brief’s candidate niches (IT/consulting, banking, healthcare, trades). One pattern row is enough: when would someone use the career site instead of a portal?
5. Public employment: open arbeit.swiss / RAV-related pages and write when a seeker or employer would use them instead of jobs.ch.
6. Q5: each bullet = observable fact → **inference** (what that means for cost or noise). No inference-only bullets.

Proof rule: factual claim → URL + access date, or path under this phase / `evidence/`. Prefer Tier A/B.

---

## 8. Sub-questions — what “complete” means

### 01-T1-Q1 — What did you open?

A list: **name + URL** for every starter (and extra) channel you opened. Not a paragraph. If you skipped a starter row, one line why.

### 01-T1-Q2 — Seeker job vs employer job

For jobs.ch, Indeed CH, LinkedIn, and your two extras: two sentences per channel (seeker / employer). Must match the table. “Biggest / most popular” is not a job.

### 01-T1-Q3 — Public pricing

One cell per portal in Q2: **number + what it buys + URL + access date**, or `unknown`. No ranges copied from the brief. No “around 2–3k.”

### 01-T1-Q4 — Career pages and RAV

Two short notes:

- **Career pages:** when a seeker goes direct (known employer, referral, employer brand) vs when an employer invests in a career site instead of or as well as a paid listing.
- **arbeit.swiss / RAV:** when a registered job-seeker or an employer obligated/encouraged to use the public channel would use it *instead of* a commercial portal.

### 01-T1-Q5 — Multi-channel cost or noise

3–5 bullets. Each bullet names a **fact** (what a product page, packing, or cross-post feature shows) and an **inference** (cost, duplicate screening, inconsistent ads). This is the load-bearing “so what” for the brief’s noise/cost story.

---

## 9. What Daniel can usefully choose in Week 1

Not a beachhead. Useful T-24 options look like:

- **Which two extras** (beyond the three named portals) to treat as first-class in the Phase 02 matrix (e.g. XING vs a regional board vs JobCloud sister brands).
- **How to treat RAV / arbeit.swiss** in later work: design-against (seekers already live there) vs note-and-park for a Zurich professional beachhead.
- **Whether the multi-channel pain premise stays** as a design input, or is still too weakly evidenced (then Phase 02 must work harder on it).

Each option needs pros/cons. You recommend; Daniel chooses.

---

## 10. Quality bar

| Result | Looks like |
| --- | --- |
| **Pass** | Required rows filled; seeker + employer job are distinct, observational sentences; every pricing cell is sourced or `unknown`; Q4 covers career pages *and* public employment; Q5 has 3–5 fact+inference bullets; [SOURCES.md](../SOURCES.md) lists the URLs with access dates. |
| **Incomplete** | Table started but RAV or career pages missing; extras not opened; Q5 is opinion only; pricing left blank instead of `unknown`. |
| **Fail** | Invented CHF numbers; essay with no table; “everyone uses LinkedIn”; jumping to “our beachhead should be…”. |

Daniel should be able to click every load-bearing URL. Depth beats volume.

---

## 11. Common mistakes

- Mapping only the three famous portals and skipping RAV / career pages.
- Writing channel *descriptions* (“leading Swiss board”) instead of jobs-to-be-done.
- Treating the brief’s 2–3k CHF as a sourced price.
- Turning Q5 into a product pitch (“therefore we should build matching”).
- Confusing this table with the Phase 02 competitor matrix (no feature-by-feature teardown here).
- One visit to the homepage, no employer-products / pricing page.

---

## 12. What this feeds

| Next | How it uses T1 |
| --- | --- |
| [02-T1](../../02-competitive/WORKSHEET.md) | Channel names become competitor seeds; “direct vs adjacent” starts from the jobs you wrote (portal vs RAV vs career site vs network). |
| [03-T2](../../03-beachhead/WORKSHEET.md) | Where volume already lives (city portals, RAV, LinkedIn) informs liquidity/geography — not a lock. |
| Week 1 T-24 | Table + Q5 + 2–3 small options above. |

---

## 13. Start here

1. Read this brief, then the worksheet Learn section.
2. Open [SOURCES-STARTER.md](../SOURCES-STARTER.md) and visit the channel table.
3. Create the channels table (MARKET-BRIEF §1 or `evidence/channels-map.md`).
4. Fill worksheet `01-T1-Q1` … `Q5` with short answers + Proof paths.
5. Log sources in [SOURCES.md](../SOURCES.md).
