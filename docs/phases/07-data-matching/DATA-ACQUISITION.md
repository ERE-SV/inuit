# Data acquisition

Seeded methods — replace with evidence and legal notes by Gate 4.

| Field | Side | Method (user / feed / crawl / enrich / inferred) | Confidence | Legal / ToS note | Fallback if missing |
| --- | --- | --- | --- | --- | --- |
| seeker profile fields | seeker | user | high | consent + purpose | block match if required missing |
| seeker home_location | seeker | user | high | explicit consent; minimize retention | disable commute filter |
| seeker search constraints | seeker | user | high | | |
| job description_raw / title / location | job | feed or crawl | med–high | ToS / license per source | skip listing |
| job required_skills / years / languages | job | inferred (LLM) from text P1; user P2 | low–med P1 | label “derived from listing” | partial match / lower rank |
| company culture / salary bands | company | user P2; enrich P1 | low–med | license; no invented salaries | unknown |
| commute_minutes | computed | maps/transit API | med | no raw home to employer | exclude commute criterion |
| match score | computed | algorithm | — | explainability; not a hire decision | | 
