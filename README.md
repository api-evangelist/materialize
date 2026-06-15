# Materialize (materialize)

Materialize is an operational data warehouse that uses streaming SQL views maintained with sub-second latency. It exposes a PostgreSQL wire-compatible interface and a session-less HTTP API for SQL execution.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/apis.yml)

## Tags

- Streaming
- Data Warehouse
- SQL
- Real-Time
- PostgreSQL Compatible

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-29

## APIs

### Materialize HTTP API

Session-less HTTP API for executing SQL statements against a Materialize region. Authenticates with HTTP Basic (email + app password). Supports a simple mode with a single query and an extended mode that submits an array of queries, each with optional parameters. Does not support session-bound statements such as SUBSCRIBE, DECLARE, FETCH, or COPY.

- **Human URL:** [https://materialize.com/docs/integrations/http-api/](https://materialize.com/docs/integrations/http-api/)
- **Base URL:** `https://{mz_host}/api/sql`

#### Tags

- SQL
- HTTP
- Streaming

#### Properties

- [Documentation](https://materialize.com/docs/integrations/http-api/)
- [Authentication](https://materialize.com/docs/manage/access-control/)
- [Postman Collection](collections/materialize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/materialize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Materialize PostgreSQL Wire Protocol

Materialize speaks the PostgreSQL wire protocol on port 6875, so any psql or libpq-based client (Go, Java, Node.js, PHP, Python, Ruby, Rust) can connect and run streaming SQL.

- **Human URL:** [https://materialize.com/docs/integrations/](https://materialize.com/docs/integrations/)
- **Base URL:** `postgres://{user}@{mz_host}:6875/materialize`

#### Tags

- SQL
- PostgreSQL
- psql
- Wire Protocol

#### Properties

- [Documentation](https://materialize.com/docs/integrations/)
- [Postman Collection](collections/materialize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/materialize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Materialize Streaming Sources and Sinks (AsyncAPI)

AsyncAPI 2.6 description of Materialize's event-driven integration surface: Kafka sources (CREATE SOURCE ... FROM KAFKA), Kafka sinks (CREATE SINK ... INTO KAFKA), and HTTP webhook sources (CREATE SOURCE ... FROM WEBHOOK). SUBSCRIBE is documented in the spec as an informational pgwire server only; AsyncAPI 2.6 has no standard binding for the PostgreSQL wire protocol, so it is intentionally not modelled as a channel.

- **Human URL:** [https://materialize.com/docs/sql/create-source/](https://materialize.com/docs/sql/create-source/)
- **Base URL:** `https://materialize.com/docs/`

#### Tags

- Streaming
- Kafka
- Webhooks
- AsyncAPI
- Sources
- Sinks

#### Properties

- [AsyncAPI](asyncapi/materialize-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Documentation](https://materialize.com/docs/sql/create-source/kafka/)
- [Documentation](https://materialize.com/docs/sql/create-sink/kafka/)
- [Documentation](https://materialize.com/docs/sql/create-source/webhook/)
- [Documentation](https://materialize.com/docs/sql/subscribe/)
- [Postman Collection](collections/materialize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/materialize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/MaterializeInc)
- [LinkedIn](https://www.linkedin.com/company/materializeinc)
- [Website](https://materialize.com/)
- [Portal](https://materialize.com/docs/)
- [Pricing](https://materialize.com/pricing)
- [Plans](plans/materialize-plans-pricing.yml)
- [Rate Limits](rate-limits/materialize-rate-limits.yml)
- [Fin Ops](finops/materialize-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
