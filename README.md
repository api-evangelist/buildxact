# Buildxact

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

**Areas:** Construction · Residential Construction · Construction Management · Estimating · Takeoffs · Job Management · Project Management · Quoting · Scheduling · Purchase Orders · Invoicing · Supplier Integration

## Buildxact on APIs.io

Everything profiled for Buildxact is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/buildxact/](https://apis.io/providers/buildxact/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Buildxact Webhooks](https://apis.io/apis/buildxact/buildxact-webhooks/) — Buildxact's webhook surface lets partner and customer integrations receive real-time notifications when events occur inside the construction-management…
- [Buildxact Authentication API](https://apis.io/apis/buildxact/buildxact-authentication-api/) — First-party login and bearer token refresh.
- [Buildxact Estimate Items API](https://apis.io/apis/buildxact/buildxact-estimate-items-api/) — Line items inside an estimate (materials, labor, assemblies).
- [Buildxact Estimates API](https://apis.io/apis/buildxact/buildxact-estimates-api/) — Construction estimates — the top-level pricing document for a job.
- [Buildxact Tax Context API](https://apis.io/apis/buildxact/buildxact-tax-context-api/) — Tax rates and inclusivity rules applied to estimate totals.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Buildxact Webhooks](https://apis.io/asyncapis/buildxact/buildxact-webhooks-asyncapi/)

#### Event channels (3)

Individual events and webhooks the provider emits.

- [estimate.accepted](https://apis.io/channels/buildxact/estimate-accepted/)
- [lead.created](https://apis.io/channels/buildxact/lead-created/)
- [lead.updated](https://apis.io/channels/buildxact/lead-updated/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Buildxact Agentic Access](https://apis.io/agentic-access/buildxact/buildxact-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Buildxact Estimate](https://apis.io/schemas/buildxact/buildxact-estimate/)
- [Buildxact Estimate Item](https://apis.io/schemas/buildxact/buildxact-estimate-item/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Buildxact Context](https://apis.io/jsonld/buildxact/buildxact-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Buildxact Vocabulary](https://apis.io/vocabularies/buildxact/buildxact-vocabulary/)

#### Examples (2)

Example requests and responses.

- [Buildxact Estimate Accepted Event Example](https://apis.io/examples/buildxact/buildxact-estimate-accepted-event-example/)
- [Buildxact List Estimates Example](https://apis.io/examples/buildxact/buildxact-list-estimates-example/)

#### Collections (5)

Postman and Open Collection request collections.

- [Buildxact Public Authentication API](https://apis.io/collections/buildxact/open-buildxact-authentication-api/)
- [Buildxact Public Authentication Estimate Items API](https://apis.io/collections/buildxact/open-buildxact-estimate-items-api/)
- [Buildxact Public Authentication Estimates API](https://apis.io/collections/buildxact/open-buildxact-estimates-api/)
- [Buildxact Public API](https://apis.io/collections/buildxact/open-buildxact-public-api/)
- [Buildxact Public Authentication Tax Context API](https://apis.io/collections/buildxact/open-buildxact-tax-context-api/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Buildxact — asyncapi rules](https://apis.io/rules/buildxact/buildxact-asyncapi-spectral-rules/)
- [Buildxact — jsonschema rules](https://apis.io/rules/buildxact/buildxact-jsonschema-spectral-rules/)
- [Buildxact API Rules](https://apis.io/rules/buildxact/buildxact-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Buildxact Authentication](https://apis.io/security/buildxact/buildxact-authentication/)
- [Buildxact Domain Security](https://apis.io/security/buildxact/buildxact-domain-security/)
- [Buildxact Vulnerability Disclosure](https://apis.io/security/buildxact/buildxact-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Buildxact Plans Pricing](https://apis.io/plans/buildxact/buildxact-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Buildxact Rate Limits](https://apis.io/rate-limits/buildxact/buildxact-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Buildxact Finops](https://apis.io/finops/buildxact/buildxact-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.buildxact.com)
- [Pricing](https://www.buildxact.com/us/pricing/)
- [Blog](https://www.buildxact.com/us/blog/)
- [Terms of service](https://www.buildxact.com/au/terms-of-use/)
- [Privacy policy](https://www.buildxact.com/au/privacy-policy/)

## API Evangelist rating

**Kin Score 47.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 66.7 |
| Contract governance | 27.3 |
| Operational transparency | 21.1 |
| Developer ergonomics | 39.3 |
| Access clarity | 50.0 |

**Agent readiness 21.7** — agent-aware

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
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 26.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/buildxact/](https://apis.io/providers/buildxact/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Buildxact: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/buildxact/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
