# Jobber (jobber)

Jobber is field service management software for home and commercial service businesses, serving 100,000+ businesses across more than 50 trade verticals (cleaning, HVAC, plumbing, electrical, landscaping, roofing, painting, handyman, and more). The platform covers the full service-delivery lifecycle — requests, assessments, quotes, scheduling, visits, time tracking, expenses, invoicing, payments, and reporting — with first-party iOS and Android apps for technicians. The Jobber Developer API is a single GraphQL endpoint at `https://api.getjobber.com/api/graphql` secured by OAuth 2.0, versioned by date via the `X-JOBBER-GRAPHQL-VERSION` header, and throttled by a leaky-bucket query-cost budget on top of a 2,500-requests / 5-minute DDoS guard. Third-party apps are published in the Jobber App Marketplace.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Field Service Management, Home Service, Scheduling, Quoting, Invoicing, Dispatching, Mobile Workforce, CRM, SaaS, GraphQL

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Jobber Developer API

GraphQL API for accessing and modifying data on Jobber accounts. Top-level objects include Clients, Requests, Quotes, Jobs, Invoices, Visits, Assessments, Properties, Products, Services, Expenses, TimeSheetEntries, Users, Accounts, and CustomFieldConfigurations.

**Human URL:** [https://developer.getjobber.com](https://developer.getjobber.com)
**Base URL:** `https://api.getjobber.com/api/graphql`

- [Documentation](https://developer.getjobber.com/docs/)
- [Getting Started](https://developer.getjobber.com/docs/getting_started/)
- [API Rate Limits](https://developer.getjobber.com/docs/using_jobbers_api/api_rate_limits/)
- [Changelog](https://developer.getjobber.com/docs/changelog/)
- [Developer Center Signup](https://developer.getjobber.com/signup/)
- [OpenAPI](openapi/jobber-developer-api-openapi.yml)
- [JSON Schema — Client](json-schema/jobber-client-schema.json)
- [JSON Schema — Job](json-schema/jobber-job-schema.json)
- [JSON Schema — Invoice](json-schema/jobber-invoice-schema.json)
- [JSON-LD](json-ld/jobber-context.jsonld)
- [Example — List Jobs](examples/jobber-list-jobs-example.json)
- [Example — Create Invoice](examples/jobber-create-invoice-example.json)
- [Naftiko Capability — Developer API GraphQL](capabilities/developer-api-graphql.yaml)

## Common Properties

- [Portal](https://getjobber.com)
- [Developer Center](https://developer.getjobber.com)
- [Pricing](https://getjobber.com/pricing/)
- [Login](https://secure.getjobber.com/login)
- [App Marketplace](https://secure.getjobber.com/app_marketplace)
- [GitHub Organization](https://github.com/GetJobber)
- [Jobber App Template (React)](https://github.com/GetJobber/Jobber-AppTemplate-React)
- [Jobber App Template (Rails API)](https://github.com/GetJobber/Jobber-AppTemplate-RailsAPI)
- [iOS App](https://apps.apple.com/app/jobber-on-the-go/id577517234)
- [Android App](https://play.google.com/store/apps/details?id=com.getjobber.jobber)
- [Jobber Academy](https://getjobber.com/academy/)
- [Masters of Home Service Podcast](https://getjobber.com/podcast/)
- [API Support — api-support@getjobber.com](mailto:api-support@getjobber.com)
- [Plans](plans/jobber-plans-pricing.yml)
- [Rate Limits](rate-limits/jobber-rate-limits.yml)
- [FinOps](finops/jobber-finops.yml)
- [Spectral Rules](rules/jobber-rules.yml)
- [Vocabulary](vocabulary/jobber-vocabulary.yml)

## Plans

| Plan | Monthly | Annual (Prepaid) | Users Included | Highlights |
|---|---|---|---|---|
| Core | $49/mo | $29/mo | 1 | Quotes, invoicing, online payments, website, reporting |
| Connect | $139/mo | $99/mo | 5 ($29/user add'l) | Automations, QuickBooks Online sync, time and expense tracking |
| Grow | $199/mo | $149/mo | 10 ($29/user add'l) | Advanced quoting, job costing, two-way SMS, custom workflows |
| Plus | $699/mo | $529/mo | 15 ($29/user add'l) | Marketing Suite, AI Receptionist, Pipeline, premium support, API walkthrough |

14-day free trial of the Grow plan, no credit card required.

## Rate Limits

| Control | Scope | Budget | Replenish | On Exceed |
|---|---|---|---|---|
| DDoS guard | app + account | 2,500 requests / 5 min | Fixed window | HTTP 429 |
| GraphQL cost | app + account | 10,000 points (default) | 500 points / sec | GraphQL `THROTTLED` error |

Cost telemetry is returned in every GraphQL response under `extensions.cost` — including `requestedQueryCost`, `actualQueryCost`, and `throttleStatus.currentlyAvailable`.

## Features

- GraphQL Developer API at `https://api.getjobber.com/api/graphql`
- OAuth 2.0 authorization with scoped access tokens via the Developer Center
- Date-based API versioning via the `X-JOBBER-GRAPHQL-VERSION` header
- Leaky-bucket query-cost throttling with telemetry in `extensions.cost`
- Built-in GraphiQL console with 60-minute test tokens
- App Marketplace for publishing third-party integrations
- 90-day developer testing accounts for app development
- Encoded global IDs for cross-account safety
- iOS and Android mobile apps for technicians
- First-party Jobber Payments for card and ACH processing
- Custom field configurations attachable to all major resources

## Use Cases

- CRM and client communications sync
- Quote-to-job-to-invoice workflow automation
- Accounting and FinOps integration (QuickBooks, Xero, BI warehouses)
- Field workforce analytics (utilization, productivity, routing)
- Marketing attribution from inbound Requests
- Subcontractor and crew dispatching
- AI receptionist and voice booking pipelines

## Integrations

QuickBooks Online · Jobber Payments / Stripe · Mailchimp · Zapier · Google Calendar · NiceJob · Jobber Capital

## Solutions

Cleaning · HVAC · Plumbing · Electrical · Landscaping · Lawn Care · Tree Care · Painting · Roofing · Construction · Handyman · Pest Control · Pool Care · 50+ other home and commercial service trades

## Maintainers

- Kin Lane — info@apievangelist.com — [apievangelist.com](https://apievangelist.com)
