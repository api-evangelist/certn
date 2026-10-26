# Certn (certn)

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

Certn is a Canada-based, globally operating background check and identity verification platform. Its RESTful API lets HR, property management, gig, and marketplace platforms order and retrieve criminal record checks, identity verification, credit, employment, education, credential, and reference checks across 200+ countries and territories, then receive results and adjudicated reports. The API authenticates with OAuth 2.0 client credentials (a Client ID and Client Secret exchanged for a Bearer token) and pushes status updates via signed webhooks. API access is free - you pay only for the checks you use.

**Note on API versions:** The original `api.certn.co` v1/v2 REST endpoints are documented and confirmed but were deprecated on 2026-04-13 and are scheduled for discontinuation on 2026-08-05 in favor of the newer CertnCentric APIs. The CertnCentric portal (`centric-api-docs.certn.co`) is a client-rendered SPA whose exact endpoint paths could not be scraped; its resource groupings (cases, checks, reports, packages, webhooks) are modeled honestly here and flagged with `x-endpoint-status` in the OpenAPI.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/apis.yml)

## Tags

- Background Checks
- Identity Verification
- Criminal Record Check
- Screening
- HR Tech
- Compliance
- Trust and Safety

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Authentication

OAuth 2.0 client credentials. Create a Client ID and Client Secret in the Partner tab under API Keys (the Client Secret is shown only at creation time), exchange them for an access token, and send it as `Authorization: Bearer {token}`. Base URL is `https://api.certn.co` for production and `https://demo-api.certn.co` for the demo environment.

## APIs

### Certn Applications API

Invite an applicant to complete a screen by email, or screen an applicant instantly from the request body, then list and filter applications. Covers the HR (`/api/v1/hr`) and Property Management (`/api/v1/pm`) surfaces.

- **Human URL:** [https://docs.certn.co/api/api-reference/hr](https://docs.certn.co/api/api-reference/hr)
- **Base URL:** `https://api.certn.co/api/v1`

### Certn Checks API

Request and retrieve individual check types - criminal record checks (Basic and Enhanced Canadian, US, international across 200+ countries), identity/OneID verification, credit reports, public records, employment, education, credential, professional reference, driver's abstract, working-with-children, and social media checks.

- **Human URL:** [https://docs.certn.co/api](https://docs.certn.co/api)
- **Base URL:** `https://api.certn.co/api/v1`

### Certn Reports API

Retrieve consolidated screening reports for an applicant - each requested check's status and findings, verified identity and financial data, and an overall risk assessment, paginated and filterable by team or owner.

- **Human URL:** [https://docs.certn.co/api/api-reference/hr](https://docs.certn.co/api/api-reference/hr)
- **Base URL:** `https://api.certn.co/api/v1`

### Certn Packages API

List the predefined screening packages (bundled check sets such as the CertnCentric Essential, Pro, and Elite tiers) and upgrade an existing application by adding further screening requests to an applicant.

- **Human URL:** [https://docs.certn.co/api/start/demo-account/understand-your-general-resources](https://docs.certn.co/api/start/demo-account/understand-your-general-resources)
- **Base URL:** `https://api.certn.co/api/v1`

### Certn Webhooks API

Receive server-to-server POST callbacks as screening results become available. Certn signs each payload with a `Certn-Signature` header (HMAC-SHA256 with a timestamp and v1 signature) and retries on 408/500/502/503/504. Webhook endpoints are registered in the Partner dashboard, not via a public REST endpoint.

- **Human URL:** [https://docs.certn.co/api/guides/use-the-api/webhooks](https://docs.certn.co/api/guides/use-the-api/webhooks)
- **Base URL:** `https://api.certn.co/api/v1`

### Certn Teams and Users API

Read the account's organizational hierarchy - Superteams contain Teams which contain Users - to scope applications, packages, and reports; retrieve the users in the account and the reference templates configured per team.

- **Human URL:** [https://docs.certn.co/api/start/demo-account/understand-your-general-resources](https://docs.certn.co/api/start/demo-account/understand-your-general-resources)
- **Base URL:** `https://api.certn.co/api/v1`

## Common Properties

- [GitHub Organization](https://github.com/Certn)
- [LinkedIn](https://www.linkedin.com/company/certn)
- [Website](https://certn.co)
- [Documentation](https://docs.certn.co/api)
- [Plans](plans/certn-plans-pricing.yml)
- [Rate Limits](rate-limits/certn-rate-limits.yml)
- [Fin Ops](finops/certn-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
