# Keywords AI (keywordsai)

Keywords AI is an LLM observability and gateway platform. It exposes an OpenAI-compatible proxy (chat completions across 250+ models) plus REST APIs for request logging, prompt management, threads, evaluations, and traces - all under a single Bearer-authenticated API at https://api.keywordsai.co/api. (The company is rebranding to Respan; the keywordsai.co host and API remain active.)

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Observability
- Gateway
- Monitoring

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Keywords AI LLM Proxy (Chat Completions)

OpenAI-compatible chat completions proxy that routes requests to 250+ LLMs through one unified endpoint, with streaming (SSE), tool calling, structured outputs, fallbacks, load balancing, caching, and automatic request logging.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/integration/chat-completions](https://docs.keywordsai.co/api-endpoints/integration/chat-completions)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Chat
- Completions
- Gateway
- LLM

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/integration/chat-completions)
- [API Reference](https://docs.keywordsai.co/api-endpoints/integration/chat-completions)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/keywordsai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Keywords AI Logging API

Asynchronous request-logging endpoint for ingesting LLM call telemetry (model, prompt/completion messages, tokens, cost, latency, customer identifier, metadata) when calls are not routed through the gateway proxy.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/async-endpoints/request-logging-endpoint](https://docs.keywordsai.co/api-endpoints/async-endpoints/request-logging-endpoint)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Logging
- Observability
- Request Logs

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/async-endpoints/request-logging-endpoint)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Keywords AI Prompts API

Manage prompts and prompt versions outside of application code - create, list, retrieve, update, and delete prompts; create, commit, and deploy versions with templated messages, models, fallbacks, and sampling parameters.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/prompt-endpoints/create-prompts](https://docs.keywordsai.co/api-endpoints/prompt-endpoints/create-prompts)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Prompts
- Prompt Management
- Versioning

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/prompt-endpoints/create-prompts)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Keywords AI Threads API

Query multi-turn conversation threads grouped from logged LLM calls, with filtering and pagination for reconstructing end-user sessions.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/data-endpoints/list-threads](https://docs.keywordsai.co/api-endpoints/data-endpoints/list-threads)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Threads
- Conversations
- Observability

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/data-endpoints/list-threads)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Keywords AI Evaluations API

Create and run evaluators to score LLM outputs - manage evaluator definitions and execute them against logs and datasets to measure quality, correctness, and safety.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/evaluator-endpoints/create-evaluator](https://docs.keywordsai.co/api-endpoints/evaluator-endpoints/create-evaluator)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Evaluations
- Evaluators
- Quality

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/evaluator-endpoints/create-evaluator)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Keywords AI Traces API

List, retrieve, and delete distributed traces (OpenTelemetry-aligned spans) capturing agent and multi-step LLM workflows for observability and debugging.

- **Human URL:** [https://docs.keywordsai.co/api-endpoints/data-endpoints/list-traces](https://docs.keywordsai.co/api-endpoints/data-endpoints/list-traces)
- **Base URL:** `https://api.keywordsai.co/api`

#### Tags

- Traces
- OpenTelemetry
- Observability

#### Properties

- [Documentation](https://docs.keywordsai.co/api-endpoints/data-endpoints/list-traces)
- [OpenAPI](openapi/keywordsai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keywordsai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keywordsai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/Keywords-AI)
- [LinkedIn](https://www.linkedin.com/company/keywordsai)
- [Website](https://www.keywordsai.co)
- [Documentation](https://docs.keywordsai.co)
- [Plans](plans/keywordsai-plans-pricing.yml)
- [Rate Limits](rate-limits/keywordsai-rate-limits.yml)
- [Fin Ops](finops/keywordsai-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
