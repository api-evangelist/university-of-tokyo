# University of Tokyo (university-of-tokyo)

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
