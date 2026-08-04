# University of Tokyo (university-of-tokyo)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Tokyo (UTokyo) is Japan's leading national research university, founded in 1877 and ranked #29 in the QS World University Rankings 2025. This repository catalogs its public, machine-readable developer/API footprint as an APIs.json profile. UTokyo's confirmed public APIs are library and digital-humanities oriented — IIIF digital archive services and an OAI-PMH institutional repository — rather than a unified developer portal.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-tokyo-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Japan, Research, Library, Digital Archives, IIIF, Open Data, OAI-PMH

## APIs

- **UTokyo Digital Archive Portal (IIIF)** — IIIF Image/Presentation APIs plus downloadable IIIF Collections and JSON-LD/RDF/CSV/TEI datasets from the UTokyo Academic Assets Archives. Docs: https://da.dl.itc.u-tokyo.ac.jp/portal/en/help/api (full API docs Japanese-only). Source/data: https://github.com/utda/dataset
- **UTokyo Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting endpoint for the WEKO institutional repository. Base URL: https://repository.dl.itc.u-tokyo.ac.jp/oai . Docs: https://www.lib.u-tokyo.ac.jp/en/library/contents/database/15

## Plans, Rate Limits & FinOps

- Plans / Pricing: [plans/university-of-tokyo-plans-pricing.yml](plans/university-of-tokyo-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-tokyo-rate-limits.yml](rate-limits/university-of-tokyo-rate-limits.yml)
- FinOps: [finops/university-of-tokyo-finops.yml](finops/university-of-tokyo-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.u-tokyo.ac.jp/en/
- GitHub: https://github.com/utda
- LinkedIn: https://www.linkedin.com/school/university-of-tokyo/
- Developer Portal: https://da.dl.itc.u-tokyo.ac.jp/portal/en/help/api
- Source Code: https://github.com/utda/dataset
- Library System: https://www.lib.u-tokyo.ac.jp/en/

## Notes

All URLs in this profile were probed live during cataloging on 2026-06-03. The OAI-PMH endpoint was verified to return a valid OAI-PMH 2.0 Identify response (WEKO platform, repositoryName "UTokyo Repository"). The official `github.com/UTokyo` organization exists but currently has no public repositories; the active digital-archives code presence is `github.com/utda`. The LinkedIn school page returns HTTP 999 (LinkedIn's automated-access block), not a dead link. No course/SIS/timetable/SSO developer APIs were found publicly documented; nothing in this profile is fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
