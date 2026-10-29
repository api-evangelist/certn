# Certn

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

Certn is a Canada-based, globally operating background check and identity verification platform. Its RESTful API lets HR, property management, gig, and marketplace platforms order and retrieve criminal record checks, identity verification, credit, employment, education, credential, and reference checks across 200+ countries, then receive results and adjudicated reports. The API authenticates with OAuth 2.0 client credentials (Client ID / Client Secret exchanged for a Bearer token) and pushes status updates via signed webhooks. The original api.certn.co v1 REST API is deprecated (discontinued 2026-08-05) in favor of the newer CertnCentric APIs; both are modeled here honestly.

**Areas:** Background Checks · Identity Verification · Criminal Record Check · Screening · Human Resources · Compliance · Trust and Safety

## Certn on APIs.io

Everything profiled for Certn is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/certn/](https://apis.io/providers/certn/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Certn Applications API](https://apis.io/apis/certn/certn-applications-api/) — Invite or instantly screen applicants and list applications (HR and PM surfaces).
- [Certn Checks API](https://apis.io/apis/certn/certn-checks-api/) — Individual check types requested and returned within an application.
- [Certn Packages API](https://apis.io/apis/certn/certn-packages-api/) — Predefined bundles of checks and application upgrades.
- [Certn Reports API](https://apis.io/apis/certn/certn-reports-api/) — Consolidated applicant screening reports and results.
- [Certn Teams and Users API](https://apis.io/apis/certn/certn-teams-and-users-api/) — Organizational hierarchy - Superteams, Teams, Users, reference templates.
- [Certn Webhooks API](https://apis.io/apis/certn/certn-webhooks-api/) — Signed server-to-server callbacks for screening status updates.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Certn Agentic Access](https://apis.io/agentic-access/certn/certn-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Certn API](https://apis.io/collections/certn/open-certn/)
- [Certn Applications API](https://apis.io/collections/certn/open-certn-applications-api/)
- [Certn Applications Checks API](https://apis.io/collections/certn/open-certn-checks-api/)
- [Certn Applications Packages API](https://apis.io/collections/certn/open-certn-packages-api/)
- [Certn Applications Reports API](https://apis.io/collections/certn/open-certn-reports-api/)
- [Certn Applications Teams and Users API](https://apis.io/collections/certn/open-certn-teams-and-users-api/)
- [Certn Applications Webhooks API](https://apis.io/collections/certn/open-certn-webhooks-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Certn Authentication](https://apis.io/security/certn/certn-authentication/)
- [Certn Domain Security](https://apis.io/security/certn/certn-domain-security/)
- [Certn Vulnerability Disclosure](https://apis.io/security/certn/certn-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Certn Plans Pricing](https://apis.io/plans/certn/certn-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Certn Rate Limits](https://apis.io/rate-limits/certn/certn-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Certn Finops](https://apis.io/finops/certn/certn-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://certn.co)
- [Documentation](https://docs.certn.co/api)
- [Blog](https://certn.co/blog/feed)
- [GitHub](https://github.com/Certn)

## API Evangelist rating

**Kin Score 23.5** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 33.6 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 32.1 |
| Access clarity | 7.9 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 17.6** — Employment & Payroll

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/certn/](https://apis.io/providers/certn/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Certn: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/certn/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
