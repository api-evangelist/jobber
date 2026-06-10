# Jobber GraphQL API

Jobber's Developer API is a GraphQL API for accessing and modifying data on Jobber accounts.
Top-level query objects include Clients, Requests, Quotes, Jobs, Invoices, Visits, Assessments,
Properties, Products, Services, Expenses, TimeSheetEntries, Users, Accounts, and
CustomFieldConfigurations. Authentication is OAuth 2.0 with scoped access tokens issued via the
Jobber Developer Center; access tokens are passed in the `Authorization: bearer ...` header and
requests are versioned with the `X-JOBBER-GRAPHQL-VERSION` date-based header. Rate limiting
combines a 2,500 requests / 5 minutes DDoS guard with a leaky-bucket GraphQL query-cost budget
surfaced through the `extensions.cost` response envelope.

**Endpoint:** https://api.getjobber.com/api/graphql

**Documentation:** https://developer.getjobber.com

**References:**

- Documentation: https://developer.getjobber.com/docs/
- GettingStarted: https://developer.getjobber.com/docs/getting_started/
