# Jobber (jobber)

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

Jobber is field service management software for home and commercial service businesses, serving
100,000+ businesses across more than 50 trade verticals (cleaning, HVAC, plumbing, electrical,
landscaping, roofing, painting, handyman, and more). The platform covers the full service-delivery
lifecycle — requests, assessments, quotes, scheduling, visits, time tracking, expenses, invoicing,
payments, and reporting — with first-party iOS and Android apps for technicians. The Jobber
Developer API is a single GraphQL endpoint at https://api.getjobber.com/api/graphql secured by
OAuth 2.0, versioned by date via the X-JOBBER-GRAPHQL-VERSION header, and throttled by a
leaky-bucket query-cost budget on top of a 2,500-requests / 5-minute DDoS guard. Third-party apps
are published in the Jobber App Marketplace.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Field Service Management
- Home Service
- Scheduling
- Quoting
- Invoicing
- Dispatching
- Mobile Workforce
- CRM
- SaaS
- GraphQL

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Jobber Developer API

Jobber's Developer API is a GraphQL API for accessing and modifying data on Jobber accounts.
Top-level query objects include Clients, Requests, Quotes, Jobs, Invoices, Visits, Assessments,
Properties, Products, Services, Expenses, TimeSheetEntries, Users, Accounts, and
CustomFieldConfigurations. Authentication is OAuth 2.0 with scoped access tokens issued via the
Jobber Developer Center; access tokens are passed in the `Authorization: bearer ...` header and
requests are versioned with the `X-JOBBER-GRAPHQL-VERSION` date-based header. Rate limiting
combines a 2,500 requests / 5 minutes DDoS guard with a leaky-bucket GraphQL query-cost budget
surfaced through the `extensions.cost` response envelope.

- **Human URL:** [https://developer.getjobber.com](https://developer.getjobber.com)
- **Base URL:** `https://api.getjobber.com/api/graphql`

#### Tags

- Field Service Management
- GraphQL
- Home Service
- Scheduling
- Invoicing
- CRM

#### Properties

- [Documentation](https://developer.getjobber.com/docs/)
- [Getting Started](https://developer.getjobber.com/docs/getting_started/)
- [Rate Limits](https://developer.getjobber.com/docs/using_jobbers_api/api_rate_limits/)
- [Changelog](https://developer.getjobber.com/docs/changelog/)
- [Sign Up](https://developer.getjobber.com/signup/)
- [Console](https://developer.getjobber.com/apps)
- [OpenAPI](openapi/jobber-developer-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jobber-developer-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jobber-developer-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/jobber-client-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/jobber-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/jobber-invoice-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/jobber-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/jobber-list-jobs-example.json)
- [Example](examples/jobber-create-invoice-example.json)

## Common Properties

- [Portal](https://getjobber.com)
- [Documentation](https://developer.getjobber.com)
- [Sign Up](https://developer.getjobber.com/signup/)
- [Console](https://secure.getjobber.com/login)
- [Sign Up](https://getjobber.com/sign-up/)
- [Pricing](https://getjobber.com/pricing/)
- [Documentation](https://getjobber.com/about/)
- [Academy](https://getjobber.com/academy/)
- [Documentation](https://getjobber.com/podcast/)
- [Tools](https://getjobber.com/free-tools/)
- [Documentation](https://getjobber.com/grants/)
- [Documentation](https://getjobber.com/summit/)
- [Marketplace](https://secure.getjobber.com/app_marketplace)
- [GitHub Organization](https://github.com/GetJobber)
- [GitHub Repository](https://github.com/GetJobber/Jobber-AppTemplate-React)
- [GitHub Repository](https://github.com/GetJobber/Jobber-AppTemplate-RailsAPI)
- [Application](https://apps.apple.com/app/jobber-on-the-go/id577517234)
- [Application](https://play.google.com/store/apps/details?id=com.getjobber.jobber)
- [Support](mailto:api-support@getjobber.com)
- [Plans](plans/jobber-plans-pricing.yml)
- [Rate Limits](rate-limits/jobber-rate-limits.yml)
- [Fin Ops](finops/jobber-finops.yml)
- [Spectral Rules](rules/jobber-rules.yml)
- [Vocabulary](vocabulary/jobber-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
