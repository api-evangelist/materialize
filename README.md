# Materialize (materialize)

Materialize is an operational data warehouse that uses streaming SQL views maintained with sub-second latency. It exposes a PostgreSQL wire-compatible interface and a session-less HTTP API for SQL execution.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=materialize-api-evangelist&utm_content=repo)

## Type
- **x-type:** company

## APIs
- **Materialize HTTP API** - Session-less SQL over HTTPS at `https://{mz_host}/api/sql`. HTTP Basic auth (email + app password).
- **Materialize PostgreSQL Wire** - libpq/psql clients on port 6875.

## Tags
- Streaming, Data Warehouse, SQL, Real-Time, PostgreSQL Compatible

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## Common Properties
- [Website](https://materialize.com/)
- [Developer Portal](https://materialize.com/docs/)
- [Pricing](https://materialize.com/pricing)
- [Plans](plans/materialize-plans-pricing.yml)
- [RateLimits](rate-limits/materialize-rate-limits.yml)
- [FinOps](finops/materialize-finops.yml)

## Notes
- Pricing reconciled (research): Compute Credits at $1.50/credit-hour. Self-Managed Community is free up to 24 GiB memory / 48 GiB disk; Self-Managed Enterprise is annual.
- No published per-account API rate limit; bounded by cluster size.
- No official OpenAPI spec.

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
