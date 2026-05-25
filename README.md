# Buildxact

Buildxact — residential construction estimating and project management software (Melbourne, Australia). An API Evangelist profile covering Buildxact's Public REST API, webhooks, pricing, rate limits, and integration surface.

## About

Founded in 2011 in Melbourne, Buildxact serves residential builders, remodelers, trade contractors, and building-material suppliers across Australia, New Zealand, the UK, the US, and Canada. The platform spans the full residential job lifecycle — lead capture, digital takeoffs, AI-assisted estimating ("Blu"), customer quoting and e-signatures, supplier/dealer price-list integration, purchase orders, scheduling, timesheets, change orders, invoicing, and two-way accounting sync with Xero and QuickBooks Online. In 2024 Autodesk announced an agreement to acquire Buildxact.

## API Surface

Buildxact exposes a public REST API and webhook channel at `developer.buildxact.com`, fronted by Azure API Management.

- Base URL: `https://api.buildxact.com`
- UAT: `https://developer-uat.buildxact.com`
- Auth: `Ocp-Apim-Subscription-Key` (partner) + `Authorization: Bearer` (user/tenant)
- Query: OData (`$filter`, `$orderBy`, `$top`, `$skip`, `$count=true`)
- Rate limit: 100 requests per 30-second sliding window
- Webhooks: `estimate.accepted`, `lead.created`, `lead.updated` (plus events reserved for Merchant / Manufacturer plans)

## Catalog Artifacts

| Type | Path |
|------|------|
| APIs.json catalog | [apis.yml](apis.yml) |
| OpenAPI (Public API) | [openapi/buildxact-public-api-openapi.yml](openapi/buildxact-public-api-openapi.yml) |
| AsyncAPI (Webhooks) | [asyncapi/buildxact-webhooks-asyncapi.yml](asyncapi/buildxact-webhooks-asyncapi.yml) |
| JSON Schema — Estimate | [json-schema/buildxact-estimate-schema.json](json-schema/buildxact-estimate-schema.json) |
| JSON Schema — Estimate Item | [json-schema/buildxact-estimate-item-schema.json](json-schema/buildxact-estimate-item-schema.json) |
| JSON-LD Context | [json-ld/buildxact-context.jsonld](json-ld/buildxact-context.jsonld) |
| Naftiko Capability — Estimates | [capabilities/estimates.yaml](capabilities/estimates.yaml) |
| Naftiko Capability — Webhooks | [capabilities/webhooks.yaml](capabilities/webhooks.yaml) |
| Spectral Rules | [rules/buildxact-rules.yml](rules/buildxact-rules.yml) |
| Vocabulary | [vocabulary/buildxact-vocabulary.yml](vocabulary/buildxact-vocabulary.yml) |
| Plans & Pricing | [plans/buildxact-plans-pricing.yml](plans/buildxact-plans-pricing.yml) |
| Rate Limits | [rate-limits/buildxact-rate-limits.yml](rate-limits/buildxact-rate-limits.yml) |
| FinOps | [finops/buildxact-finops.yml](finops/buildxact-finops.yml) |
| Examples | [examples/](examples/) |

## Source References

- Website: <https://www.buildxact.com>
- Developer portal: <https://developer.buildxact.com>
- Getting started: <https://developer.buildxact.com/getting-started>
- API help article: <https://help.buildxact.com/en/articles/4510284-buildxact-application-programming-interface-api>
- Pricing: <https://www.buildxact.com/us/pricing/>
- GitHub org (empty as of profile date): <https://github.com/Buildxact>

Maintainer: Kin Lane &lt;kin@apievangelist.com&gt;
