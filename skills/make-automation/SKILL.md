---
name: make-automation
description: Design and troubleshoot Make.com scenarios using triggers, modules, routers, filters, iterators, aggregators and error handlers. Use when automating workflows across SaaS applications with Make.
---

# Make.com Scenario Automation

## Workflow
1. Define the trigger event, business outcome, expected volume and latency.
2. Identify connected apps, module availability, permissions and plan limits.
3. Map data fields and required transformations.
4. Design modules in order; use filters and routers for explicit branches.
5. Handle arrays with iterators and aggregators only where needed.
6. Plan for duplicates, out-of-order events and partial completion.
7. Add error handlers, bounded retries and notification routes.
8. Track operations, execution history, rate limits and scenario costs.
9. Test normal, empty, malformed, duplicate and failed responses.
10. Document ownership, recovery steps and change history.

## Deliverables
Scenario map, module configuration, field mapping, error strategy, test matrix and monitoring checklist.

## Guardrails
Never expose connection secrets in screenshots or exported blueprints. Avoid infinite retry loops. Do not enable scenarios that send messages, charge customers or change production data without explicit approval. Confirm current module behaviour and plan limits in Make documentation.
