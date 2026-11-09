---
name: evaluation-observability
description: Test and monitor AI agents and automations for task success, correctness, safety, latency, cost and reliability. Use when preparing a release or diagnosing failures in production.
---

# Agent Evaluation and Observability

## Workflow
1. Define success criteria tied to the actual user task.
2. Build a representative test set with normal, edge, ambiguous and adversarial cases.
3. Include expected outcomes, unacceptable outcomes and scoring guidance.
4. Test tool selection, argument validity, output correctness and action boundaries.
5. Evaluate retrieval and citation quality when using knowledge sources.
6. Run regression tests after prompt, model, tool or workflow changes.
7. Instrument latency, token or operation cost, error rate, retries and completion rate.
8. Record traces with redaction and retention controls.
9. Set alerts for failures, unusual volume, cost spikes and downstream service errors.
10. Review incidents and update tests to prevent recurrence.

## Deliverables
Evaluation dataset, rubric, regression suite, dashboard metrics, alert thresholds and incident review template.

## Guardrails
Do not use sensitive production data in tests without authorization and protection. Avoid logging secrets or full personal records. Do not treat a single successful demo as proof of reliability.
