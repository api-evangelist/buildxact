# Buildxact (buildxact)

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
