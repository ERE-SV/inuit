# Data dictionary

- **Status:** seeded from `docs/brief/` — refine in Week 7; finalize by Gate 4  
- **Phase:** 07-data-matching  

Mark each row: **keep** / **cut** / **add**. Acquisition detail lives in [DATA-ACQUISITION.md](DATA-ACQUISITION.md).

## Seeker — profile fields

| Field | Type | Required | Example | Privacy notes | Seed status |
| --- | --- | --- | --- | --- | --- |
| full_name | string | yes | Anna Meier | Visible per tier | keep? |
| headline | string | no | Backend engineer | | keep? |
| city | string | yes | Zürich | | keep? |
| home_location | geo | no | Precise lat/long or address | **Sensitive** — consent; prefer server-side commute | keep? |
| work_authorization_ch | enum | yes | yes/no/unknown | | keep? |
| education[] | list | yes | BSc CS, ETH, grade | Grades optional by niche | keep? |
| experience[] | list | yes | Employer, title, years | | keep? |
| skills[] | list | yes | Python, Kubernetes | | keep? |
| certificates[] | list | no | AWS SAP… | On request visibility possible | keep? |
| languages[] | list | yes | DE C2, EN C1 | | keep? |
| portfolio_links[] | url list | no | | | keep? |

## Seeker — search / constraint fields

| Field | Type | Required | Example | Notes | Seed status |
| --- | --- | --- | --- | --- | --- |
| target_roles[] | list | yes | Software Engineer | | keep? |
| salary_floor_chf | number | yes | 90000 | | keep? |
| max_commute_minutes | number | no | 30 | Needs home + workplace | keep? |
| preferred_locations[] | list | yes | Zürich city | | keep? |
| company_size_range | enum/range | no | 50–200 | | keep? |
| company_age_or_stage | enum | no | startup/scale/enterprise | | keep? |
| culture_tags[] | list | no | flat, remote-friendly | Subjective — careful | keep? |
| work_model | enum | yes | onsite/hybrid/remote | | keep? |
| remote_share_max | number | no | 60% | | keep? |
| must_have_benefits[] | list | no | | Soft | keep? |

## Company — profile fields

| Field | Type | Required | Example | Notes | Seed status |
| --- | --- | --- | --- | --- | --- |
| legal_name | string | yes | | | keep? |
| display_name | string | yes | | | keep? |
| size_employees | number/range | yes | 120 | | keep? |
| locations[] | list | yes | Zürich, Bern | Multi-site care | keep? |
| work_model_default | enum | yes | hybrid | | keep? |
| culture_tags[] | list | no | | Self-described | keep? |
| values_text | text | no | | Optional storytelling | keep? |
| salary_bands_public | range | no | | Often missing → enrich | keep? |

## Job — requirement profile fields

| Field | Type | Required | Must/Nice | Example | Notes | Seed status |
| --- | --- | --- | --- | --- | --- | --- |
| title | string | yes | — | Senior Engineer | | keep? |
| workplace_location | geo | yes | — | | Commute calc | keep? |
| salary_range_chf | range | no | — | | Often inferred P1 | keep? |
| work_model | enum | yes | — | | | keep? |
| years_experience_min | number | no | must | 3 | | keep? |
| required_skills[] | list | yes | must/nice | | | keep? |
| required_languages[] | list | yes | must | DE B2 | | keep? |
| required_degrees[] | list | no | must/nice | | | keep? |
| required_certificates[] | list | no | must/nice | | | keep? |
| visa_sponsorship | bool | yes | — | | | keep? |
| description_raw | text | yes | — | | Bootstrap ingest | keep? |
| source_url | url | yes | — | | Lineage | keep? |
| requirements_inferred | bool | yes | — | | Label in UI | keep? |

## Acquisition seed (fill fully in DATA-ACQUISITION)

Default hypotheses: seeker fields = **user input**; job text fields = **feed/crawl + LLM extract** in bootstrap; commute = **computed**; culture/salary gaps = **enrichment or unknown**.
