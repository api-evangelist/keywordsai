# Keywords AI (keywordsai)

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
