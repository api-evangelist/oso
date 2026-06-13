# Oso Cloud

Oso Cloud is an authorization-as-a-service platform that provides a REST API for defining and enforcing relationship-based access control policies. It enables developers to model RBAC, ReBAC, and ABAC authorization patterns, manage authorization facts, and query permissions at runtime with sub-10ms latency and 99.99% availability.

## Links

- **Website:** https://www.osohq.com
- **Documentation:** https://www.osohq.com/docs
- **GitHub Org:** https://github.com/osohq
- **Blog:** https://www.osohq.com/blog
- **Pricing:** https://www.osohq.com/pricing
- **Status:** https://oso.statuspage.io/
- **LinkedIn:** https://www.linkedin.com/company/osohq
- **X:** https://x.com/osohq
- **Changelog:** https://www.osohq.com/docs/changelog/whats-new

## APIs

### Oso Cloud Authorization API

Base URL: `https://api.osohq.com/api`

Authentication: Bearer token via `Authorization: Bearer <api-key>` header

Key endpoints:
- `POST /authorize` — Check if an actor can perform an action on a resource
- `POST /list` — Get all resource IDs an actor can act on
- `POST /actions` — Get all actions an actor can perform on a resource
- `POST /query` — Query predicates with concrete or wildcard arguments
- `POST /authorize_resources` — Filter multiple resources by permission
- `GET /policy` — Retrieve the active Polar authorization policy
- `POST /policy` — Deploy an updated Polar authorization policy
- `POST /facts` — Add authorization facts
- `POST /bulk` — Add and delete facts atomically
- `POST /clear_data` — Clear all authorization data

## SDKs

- Node.js (v2.x) — https://github.com/osohq/oso-node
- Python (v2.x) — https://pypi.org/project/oso-cloud/
- Go (v2.x) — https://github.com/osohq/go-oso-cloud
- Java (v1.x)
- Ruby (v1.x)
- .NET/C# (v1.x)

## Artifacts

| File | Description |
|------|-------------|
| [apis.yml](apis.yml) | APIs.json 0.19 provider index |
| [plans/oso-plans-pricing.yml](plans/oso-plans-pricing.yml) | API Commons Plans 0.1 — pricing tiers |
| [rate-limits/oso-rate-limits.yml](rate-limits/oso-rate-limits.yml) | API Commons Rate Limits 0.1 |
| [finops/oso-finops.yml](finops/oso-finops.yml) | FinOps Framework 1.0 FOCUS-aligned |
