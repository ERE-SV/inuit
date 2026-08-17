# MVP screen inventory

Seeded from product brief. **Keep / rename / split / cut** with rationale in Notes. Every row must exist as a Figma frame before Gate 4 (MVP).

| Screen ID | Frame name (Figma) | Purpose | Primary actions | Key data | States | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| MVP-000 | Marketing / landing | Explain product; CTA signup | Sign up seeker; Sign up company | Value prop | — | Optional if waitlist-only MVP |
| MVP-010 | Auth — sign up | Create account | Email/password or SSO; choose role | Role: seeker / company | Error, loading | |
| MVP-011 | Auth — sign in | Return user | Sign in; reset password | — | Error | |
| MVP-020 | Seeker onboarding — welcome | Set expectations | Continue | Steps overview | — | |
| MVP-021 | Seeker — profile basics | Name, location hub, work auth | Save / continue | Name, city, work permit | Validation | Home address later / sensitive |
| MVP-022 | Seeker — education | Degrees, grades, institutions | Add / edit / continue | Education entries | Empty | |
| MVP-023 | Seeker — experience | Roles, years, skills | Add / edit / continue | Experience, skills | Empty | |
| MVP-024 | Seeker — certificates & languages | Creds + language levels | Add / continue | Certs, languages | Empty | |
| MVP-025 | Seeker — search preferences | Constraints for matching | Save preferences | Role, commute, salary floor, size, culture, work model | — | Core matching inputs |
| MVP-026 | Seeker — privacy / consent | Commute & visibility consent | Accept / customize | Consent flags | — | Required before commute match |
| MVP-030 | Seeker — home / match list | Top-X jobs | Open match; refresh | Ranked jobs + score teaser | Empty, loading | |
| MVP-031 | Seeker — match detail | Why it fits | Interested / pass; see rationale | Criteria hit/miss; job facts; inferred labels | — | Explainability |
| MVP-032 | Seeker — pipeline / status | Own opportunities overview | Open thread/status | Status per match | Empty | Not employer ATS |
| MVP-033 | Seeker — notifications | Fit alerts | Open match | Notification list | Empty | |
| MVP-040 | Company onboarding | Claim / create org | Continue | Company basics | — | |
| MVP-041 | Company — profile | Culture, locations, size, work model | Save | Company fields | — | |
| MVP-042 | Company — job requirement | Structured must/nice | Publish / save draft | Requirements | Validation | Not only marketing copy |
| MVP-043 | Company — candidate list | Top-X seekers for a job | Open candidate; invite | Ranked candidates + score | Empty, loading | |
| MVP-044 | Company — candidate detail | Rationale + profile summary | Request interview / pass | Hit/miss; limited PII | — | |
| MVP-045 | Company — inbound forward | Review forwarded match (bootstrap) | Claim interest / dismiss | Candidate summary; listing source | — | GTM bootstrap motion |
| MVP-050 | Shared — interview interest | Both sides confirm interest | Propose times / handoff | Contact path | Pending states | Calendar may be external |
| MVP-060 | Settings — account | Profile visibility, notifs | Save | Settings | — | |
| MVP-061 | Settings — data / export | Privacy rights basics | Export / delete request | — | Confirm | Lightweight MVP OK |

## Flows to prototype (link frames)

1. Seeker signup → profile → preferences → first matches  
2. Company signup → job requirements → candidate Top-X  
3. Strong fit → notify both → interview interest  
4. Empty matches → (MVP: message only; what-if can be V2)

## Change log

| Date | Change | Rationale |
| --- | --- | --- |
| 2026-08-17 | Seeded from brief | Starting IA for Malte |
