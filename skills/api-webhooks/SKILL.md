---
name: api-webhooks
description: Integrate SaaS products and internal systems using REST APIs, webhooks, authentication, pagination, rate limits, retries and event validation. Use when connecting services or designing event-driven automation.
---

# APIs and Webhooks

## Workflow
1. Identify the systems, API versions, business events and data owner.
2. Read official API documentation and confirm endpoint, method, schema and limits.
3. Choose supported authentication; store credentials in a secret manager or platform credential store.
4. Validate request and response schemas, content types and required fields.
5. For webhooks, verify signatures where supported and reject invalid or replayed events.
6. Respond promptly to webhook delivery and process heavier work asynchronously where appropriate.
7. Handle pagination, rate limits, transient failures and backoff.
8. Use idempotency and deduplication to prevent repeated side effects.
9. Minimize personal data and define retention and deletion behaviour.
10. Test error codes, expired credentials, duplicate events and service downtime.

## Deliverables
Integration specification, sequence diagram, field mapping, authentication plan, retry/idempotency design and test matrix.

## Guardrails
Never put tokens in public repositories, URLs, client-side code or logs. Do not bypass API permissions or rate limits. Treat inbound payloads as untrusted. Avoid logging full personal or payment data.
