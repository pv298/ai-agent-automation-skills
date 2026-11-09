---
name: n8n-automation
description: Plan, build, test and maintain n8n workflows for business process automation, API integration, AI-assisted tasks, notifications and data synchronization. Use when designing or troubleshooting n8n workflows.
---

# n8n Workflow Automation

## Workflow
1. Define the trigger, business outcome, inputs, outputs and workflow owner.
2. Confirm n8n deployment type/version and available credentials or nodes.
3. Sketch the workflow before implementation: trigger, validation, processing, branching, actions and completion.
4. Use native nodes where suitable; use HTTP Request for APIs when appropriate.
5. Validate and normalize incoming data before downstream actions.
6. Configure credentials securely; never hardcode API keys in Code nodes or workflow exports.
7. Add error branches, retry limits, timeouts and alerting.
8. Prevent duplicates with idempotency keys, event IDs or a reliable lookup strategy.
9. Test success, invalid input, API failure, rate limit, timeout and duplicate events.
10. Document activation, ownership, monitoring, backup and rollback.

## Deliverables
Workflow diagram, node-by-node configuration plan, field mapping, credential requirements, test cases and operations notes.

## Guardrails
Do not activate a production workflow or send real customer messages without approval. Treat webhook payloads as untrusted. Use least-privilege credentials and protect execution data that may contain personal information. Verify current node behaviour against the installed n8n version.
