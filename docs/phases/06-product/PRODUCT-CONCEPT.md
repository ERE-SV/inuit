# Product concept

- **Status:** seeded starter — refine Week 7  
- **Phase:** 06-product  
- **Depends on:** Gate 3 brand principles  
- **Screens:** start from [MVP-SCREEN-INVENTORY.md](MVP-SCREEN-INVENTORY.md)

## Journeys

### Seeker (happy path)

1. Sign up → build profile + search preferences (+ privacy consent)  
2. See Top-X matches with rationale  
3. Express interest → notify company side → interview path  
4. Track status in personal pipeline  

### Company / HR (happy path)

1. Sign up / claim company → company profile  
2. Create structured job requirements (or receive bootstrap forward)  
3. See Top-X pre-qualified candidates with rationale  
4. Invite / interview interest → external calendar/ATS as needed  

## Feature lists (each feature in exactly one version)

### MVP — liquidity + core match loop

| Feature | Notes |
| --- | --- |
| Seeker profile + search preferences | Seeded fields in data dictionary |
| Company profile + structured job requirements | |
| Bidirectional match Top-X + rationale | Indicator, not hire guarantee |
| Notifications on strong fit | |
| Interview interest / handoff (lightweight) | Not full ATS |
| Bootstrap: forward candidates against ingested listings | Label inferred requirements |
| Privacy consents for sensitive matching | Commute/home |
| Seeker pipeline overview | Own status only |
| Basic settings / data rights request | Lightweight |

### V2 — retention + employer depth

| Feature | Notes |
| --- | --- |
| Zero-match / what-if constraint relaxation | From brief |
| Richer employer first-party profiles | Phase-2 data model |
| Claim listing / correct inferred fields | Trust |
| Career-gap / radar (basic) | Cohort disclaimer |
| Stronger notification preferences | |
| Export to ATS (CSV/PDF) | Beachhead handoff |

### V3 — scale + intelligence

| Feature | Notes |
| --- | --- |
| Company push API for jobs | Brief phase 3 |
| Market intelligence for employers | Volume vs criteria |
| Advanced culture/soft matching (if gated safe) | |
| Voice/conversational profile capture (optional) | After forms proven |
| Deeper premium seeker insights | Monetization-dependent |

## Non-goals (near term)

- Full ATS replacement (approvals, internal stage tracking)  
- Hire guarantee from scores  
- Cover-letter generation factory  
- Nationwide all-roles coverage before beachhead liquidity  

## Scope checkpoint ask

- [ ] Lock MVP/V2/V3 feature lists  
- [ ] Conditions:  
