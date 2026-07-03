# Certn (certn)

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
