# Jobber

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

Jobber is field service management software for home and commercial service businesses, serving
100,000+ businesses across more than 50 trade verticals (cleaning, HVAC, plumbing, electrical,
landscaping, roofing, painting, handyman, and more). The platform covers the full service-delivery
lifecycle — requests, assessments, quotes, scheduling, visits, time tracking, expenses, invoicing,
payments, and reporting — with first-party iOS and Android apps for technicians. The Jobber
Developer API is a single GraphQL endpoint at https://api.getjobber.com/api/graphql secured by
OAuth 2.0, versioned by date via the X-JOBBER-GRAPHQL-VERSION header, and throttled by a
leaky-bucket query-cost budget on top of a 2,500-requests / 5-minute DDoS guard. Third-party apps
are published in the Jobber App Marketplace.

**Areas:** Field Service Management · Home Service · Scheduling · Quoting · Invoicing · Dispatching · Mobile Workforce · CRM · Software-as-a-Service · GraphQL · Canada

## Jobber on APIs.io

Everything profiled for Jobber is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/jobber/](https://apis.io/providers/jobber/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Jobber Graph QL API](https://apis.io/apis/jobber/jobber-graph-ql-api/) — The Graph QL API from Jobber — 1 operation(s) for graph ql.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Jobber GraphQL API](https://apis.io/graphqls/jobber/jobber-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [jobber](https://apis.io/servers/jobber/jobber/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Jobber Agentic Access](https://apis.io/agentic-access/jobber/jobber-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Jobber Client](https://apis.io/schemas/jobber/jobber-client/)
- [Jobber Invoice](https://apis.io/schemas/jobber/jobber-invoice/)
- [Jobber Job](https://apis.io/schemas/jobber/jobber-job/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Jobber Context](https://apis.io/jsonld/jobber/jobber-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Jobber Vocabulary](https://apis.io/vocabularies/jobber/jobber-vocabulary/)

#### Examples (2)

Example requests and responses.

- [Jobber Create Invoice Example](https://apis.io/examples/jobber/jobber-create-invoice-example/)
- [Jobber List Jobs Example](https://apis.io/examples/jobber/jobber-list-jobs-example/)

#### Collections (2)

Postman and Open Collection request collections.

- [Jobber Developer API](https://apis.io/collections/jobber/open-jobber-developer-api/)
- [Jobber Developer GraphQL API](https://apis.io/collections/jobber/open-jobber-graphql-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Jobber — jsonschema rules](https://apis.io/rules/jobber/jobber-jsonschema-spectral-rules/)
- [Jobber API Rules](https://apis.io/rules/jobber/jobber-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Jobber Authentication](https://apis.io/security/jobber/jobber-authentication/)
- [Jobber Domain Security](https://apis.io/security/jobber/jobber-domain-security/)
- [Jobber Vulnerability Disclosure](https://apis.io/security/jobber/jobber-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Jobber Plans Pricing](https://apis.io/plans/jobber/jobber-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Jobber Rate Limits](https://apis.io/rate-limits/jobber/jobber-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Jobber Finops](https://apis.io/finops/jobber/jobber-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.getjobber.com/)
- [Documentation](https://developer.getjobber.com)
- [Pricing](https://getjobber.com/pricing/)
- [GitHub](https://github.com/GetJobber)

## API Evangelist rating

**Kin Score 50.4** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 68.3 |
| Contract quality | 64.9 |
| Contract governance | 27.3 |
| Operational transparency | 36.8 |
| Developer ergonomics | 54.8 |
| Access clarity | 39.5 |

**Agent readiness 45.3** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/jobber/](https://apis.io/providers/jobber/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Jobber: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/jobber/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
