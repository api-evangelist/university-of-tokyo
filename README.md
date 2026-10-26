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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Tokyo (東京大学, UTokyo) is Japan's oldest and largest national research university, founded in 1877. This repository catalogs its **institution-operated** machine-readable footprint as an APIs.json profile, under the API Evangelist university pipeline — which settles *who operates each surface* before saving anything, because most of what a university appears to publish is a vendor's contract running under the institution's name.

**For this institution, none of it is.** Every surface below runs on a host under `u-tokyo.ac.jp`. No Figshare, Elsevier Pure, Symplectic, Dataverse or Canvas tenancy could be substantiated (`u-tokyo.figshare.com` → HTTP 202 zero bytes; `utokyo.pure.elsevier.com` → 301 to a hostname that does not resolve; `utokyo.instructure.com` → 404). The university self-hosts its repository software rather than buying a hosted one.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-tokyo-api-evangelist&utm_content=repo

## Type

- `x-type: university`
- `x-category: Public Research University`
- Index · Consumer · 3rd-Party

## Tags

University, Higher Education, Education, Japan, Public Research University, Research Data, Research Repository, Library, Digital Archives, Identity Federation, IIIF, OAI-PMH, Open Access, Metadata

## Surfaces — all `x-operator: institution`

| Surface | Host | Verified |
|---|---|---|
| **Academic Assets Archives Portal API** — OpenSearch-described search, item representations in JSON-LD / CSV / refer-BibIX via `_format` | `da.dl.itc.u-tokyo.ac.jp` | Item JSON-LD 200 (`application/ld+json`, DC-NDL). Search endpoint **403** to external automated clients. |
| **IIIF Presentation + Image APIs** | `da.dl.itc.u-tokyo.ac.jp`, `iiif.dl.itc.u-tokyo.ac.jp` | Presentation 2.1 manifest 200; Image API 2.0 **level2** `info.json` 200 |
| **OAI-PMH metadata harvesting** — two independent endpoints | `repository.dl.itc.u-tokyo.ac.jp/oai`, `da.dl.itc.u-tokyo.ac.jp/portal/oai` | Both `Identify` 200. Repository: 7 metadata formats. Portal: 5 formats, 1,957 sets. |
| **Repository Records API** — undocumented but live JSON, 69,549 records | `repository.dl.itc.u-tokyo.ac.jp/api/records/` | 200, paged, `links.next` |
| **GakuNin identity federation** — 3 SAML 2.0 entities | `gidp.adm.`, `shibbi.pki.itc.`, `step10.adm.s.u-tokyo.ac.jp` | Present in the 650-entity GakuNin aggregate, `registrationAuthority https://www.gakunin.jp` |

## Two findings that change how you read this profile

**1. The documentation is Japanese-only, and the English page hides it.** `https://da.dl.itc.u-tokyo.ac.jp/portal/en/help/api` returns 200 with a single line — *"Only available in Japanese"* — and links across. The Japanese page at `/portal/help/api` carries the full verb, parameter, format and `resumptionToken` paging tables. A survey conducted in English finds no API here at all. That is how the June 2026 profile of this institution under-counted it.

**2. `repository.dl.itc.u-tokyo.ac.jp` blocks browsers, not bots.** It returns **HTTP 406** to a desktop-browser `User-Agent` and **HTTP 200** to a plain client. This is inverted from the usual bot challenge, so the standard "retry with a browser UA" heuristic makes a fully live host read as dead. `da.dl.itc.u-tokyo.ac.jp` does the opposite. The two institution hosts have opposite edge policies and must be configured separately — see [rules/university-of-tokyo-harvest-rules.yml](rules/university-of-tokyo-harvest-rules.yml).

## Standards conformance (`education` regime)

Verified live, never claimed from prose — see [conformance/university-of-tokyo-conformance.yml](conformance/university-of-tokyo-conformance.yml).

- **Conforms:** `oai-pmh` 2.0 (two endpoints), `saml` 2.0, `shibboleth`, IIIF Presentation 2.1, IIIF Image 2.0 level2, JSON-LD 1.1, JPCOAR 2.0, robots.txt; OpenSearch 1.1 *partial* (description conforms, described endpoint is 403).
- **Does not:** `orcid` (only WEKO-internal author IDs observed), `datacite` and `crossref` (DOIs are minted under prefix `10.15083` through **JaLC**, a different registration agency), `scim`, `lti`, `oneroster`, `ed-fi`, `caliper`, `qti`, `security.txt`, `llms.txt`, OpenAPI.

## Artifacts

| | |
|---|---|
| OpenAPI (derived / probed — **not the university's**) | [openapi/](openapi/) + [openapi/_original/](openapi/_original/) |
| JSON Schema | [json-schema/](json-schema/) |
| Live captured payloads | [examples/](examples/) |
| Conformance | [conformance/university-of-tokyo-conformance.yml](conformance/university-of-tokyo-conformance.yml) |
| Authentication + federation entities | [authentication/university-of-tokyo-authentication.yml](authentication/university-of-tokyo-authentication.yml) |
| OAuth scopes (recorded absent) | [scopes/university-of-tokyo-scopes.yml](scopes/university-of-tokyo-scopes.yml) |
| Error handling | [errors/university-of-tokyo-error-handling.yml](errors/university-of-tokyo-error-handling.yml) |
| Lifecycle + versioning | [lifecycle/university-of-tokyo-lifecycle.yml](lifecycle/university-of-tokyo-lifecycle.yml) |
| Metadata vocabularies | [vocabulary/university-of-tokyo-vocabulary.yml](vocabulary/university-of-tokyo-vocabulary.yml) |
| Consumption rules | [rules/university-of-tokyo-harvest-rules.yml](rules/university-of-tokyo-harvest-rules.yml) |
| JSON-LD context | [json-ld/university-of-tokyo-context.jsonld](json-ld/university-of-tokyo-context.jsonld) |
| Plans · Rate limits · FinOps · Domain security | [plans/](plans/) · [rate-limits/](rate-limits/) · [finops/](finops/) · [security/](security/) |

**Every OpenAPI in this repository was derived by API Evangelist from live probes and carries an `x-provenance` block saying so.** The University of Tokyo publishes no OpenAPI, AsyncAPI, GraphQL schema, Postman collection or JSON Schema of its own. Nothing here should be read as an artifact the university authored.

## Institutional pointers

- Website: https://www.u-tokyo.ac.jp/en/
- Terms / Site policy: https://www.u-tokyo.ac.jp/en/general/site_policy.html
- Privacy policy: https://www.u-tokyo.ac.jp/en/general/privacy_policy.html
- Research repository: https://repository.dl.itc.u-tokyo.ac.jp/
- Open data (collection list): https://da.dl.itc.u-tokyo.ac.jp/portal/en/database/list
- Library catalog (OPAC): https://opac.dl.itc.u-tokyo.ac.jp/
- Course catalog: https://catalog.he.u-tokyo.ac.jp/
- Identity federation (GakuNin metadata): https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
- Research computing: https://www.cc.u-tokyo.ac.jp/en/supercomputer/
- AI policy: https://utelecon.adm.u-tokyo.ac.jp/en/docs/ai-tools-in-classes/
- AI tooling: https://utelecon.adm.u-tokyo.ac.jp/notice/2024/0327-ai-service/
- GitHub (digital archives): https://github.com/utda — note `github.com/UTokyo` exists but has **0** public repositories
- LinkedIn: https://www.linkedin.com/school/university-of-tokyo/ (HTTP 999 is LinkedIn's automated-access block, not a dead link)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19 (re-profiled under the university pipeline)

## Maintainers

- Kin Lane — kin@apievangelist.com
