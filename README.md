# Buildxact (buildxact)

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

Buildxact is a Melbourne, Australia-headquartered construction estimating and project management SaaS for residential builders, remodelers, trade contractors, and building-material suppliers. Founded in 2011, the company operates regional offices in Austin, Texas (North America), and serves customers across Australia, New Zealand, the United Kingdom, the United States, and Canada. The platform spans the full residential job lifecycle — lead capture, digital takeoffs, AI-assisted estimating ("Blu"), customer quoting and e-signatures, supplier/dealer price-list integration, purchase orders, scheduling (Gantt), timesheets, variations/change orders, invoicing, and two-way accounting sync with Xero and QuickBooks Online. Buildxact exposes a public REST API and webhook surface at developer.buildxact.com, available to Merchant and Manufacturer partners as well as customer subscribers, using a Microsoft Azure API Management gateway (Ocp-Apim-Subscription-Key + bearer token). Endpoints support OData filtering and sorting, with a separate UAT/staging environment. In 2024, Autodesk announced an agreement to acquire Buildxact, positioning the product as a residential construction front-end alongside Autodesk's broader AEC portfolio.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/apis.yml)

## Scope

- **Type:** Provider
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Construction
- Residential Construction
- Construction Management
- Estimating
- Takeoffs
- Job Management
- Project Management
- Quoting
- Scheduling
- Purchase Orders
- Invoicing
- Supplier Integration
- Material Pricing
- Builders
- Remodelers
- Trades
- SaaS
- Australia
- Autodesk

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Buildxact Public API

Buildxact's public REST API exposes core construction-job data including estimates and estimate items, with related tax-context and reference data. The API is fronted by Azure API Management; every request must carry an Ocp-Apim-Subscription-Key header identifying the partner organization and an Authorization: Bearer access token scoped to a Buildxact user and tenant. Endpoints follow REST conventions with OData query support — $filter, $orderBy, $top, $skip, and $count=true (record total returned via the x-odata-total-count response header). A staging environment is available at developer-uat.buildxact.com. Rate-limited at 100 requests per 30-second window.

- **Human URL:** [https://developer.buildxact.com/apis](https://developer.buildxact.com/apis)
- **Base URL:** `https://api.buildxact.com`

#### Tags

- Construction
- Estimates
- Estimate Items
- REST
- OData

#### Properties

- [Documentation](https://developer.buildxact.com/getting-started)
- [Documentation](https://developer.buildxact.com/apis)
- [Documentation](https://developer.buildxact.com/estimate-data)
- [Authentication](https://developer.buildxact.com/authorization)
- [Sign Up](https://developer.buildxact.com/signup)
- [Plans](https://developer.buildxact.com/plans)
- [Help Center](https://help.buildxact.com/en/articles/4510284-buildxact-application-programming-interface-api)
- [OpenAPI](openapi/buildxact-public-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/buildxact-public-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildxact-public-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/buildxact-estimate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/buildxact-estimate-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/buildxact-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/buildxact-vocabulary.yml)
- [Rate Limits](rate-limits/buildxact-rate-limits.yml)

### Buildxact Webhooks

Buildxact's webhook surface lets partner and customer integrations receive real-time notifications when events occur inside the construction-management platform — including Estimate Accepted, Lead Created, and Lead Updated, plus additional event types reserved for Merchant and Manufacturer plan tiers. Webhooks are registered from the "My Business > API" panel of the Buildxact web app: provide a destination URL, choose events, store the signing secret used to verify payload authenticity, and inspect deliveries via the built-in Event Log. Payloads are JSON over HTTPS.

- **Human URL:** [https://developer.buildxact.com/webhooks](https://developer.buildxact.com/webhooks)

#### Tags

- Webhooks
- Events
- Estimates
- Leads
- Event-Driven

#### Properties

- [Documentation](https://developer.buildxact.com/webhooks)
- [AsyncAPI](asyncapi/buildxact-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/buildxact-public-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildxact-public-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.buildxact.com)
- [Australia Site](https://www.buildxact.com/au/)
- [U S Site](https://www.buildxact.com/us/)
- [U K Site](https://www.buildxact.com/uk/)
- [Developer Portal](https://developer.buildxact.com)
- [Help Center](https://help.buildxact.com)
- [A P I Help Article](https://help.buildxact.com/en/articles/4510284-buildxact-application-programming-interface-api)
- [Pricing](https://www.buildxact.com/us/pricing/)
- [Plans](https://help.buildxact.com/en/articles/11559145-which-buildxact-subscription-plan-is-right-for-my-business)
- [Integrations](https://www.buildxact.com/au/features/integrations/)
- [Accounting Integrations](https://www.buildxact.com/us/features/construction-accounting-software/)
- [Blu A I](https://www.buildxact.com/us/features/blu/)
- [Company](https://www.buildxact.com/au/company/)
- [Blog](https://www.buildxact.com/us/blog/)
- [Contact](https://www.buildxact.com/us/contact/)
- [Trial](https://www.buildxact.com/us/free-trial/)
- [LinkedIn](https://au.linkedin.com/company/buildxact)
- [Git Hub](https://github.com/Buildxact)
- [Terms of Service](https://www.buildxact.com/au/terms-of-use/)
- [Privacy Policy](https://www.buildxact.com/au/privacy-policy/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
