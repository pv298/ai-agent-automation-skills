---
name: multi-agent-orchestration
description: Plan and coordinate multiple specialized AI agents with clear roles, task boundaries, shared state, handoffs, verification and escalation. Use when a task benefits from parallel or staged agent collaboration.
---

# Multi-Agent Orchestration

## When to use
Use multiple agents only when work can be meaningfully decomposed and the coordination cost is justified. Prefer a single agent or deterministic workflow for simple tasks.

## Workflow
1. Define the final outcome and acceptance criteria.
2. Decompose work into bounded tasks with explicit dependencies.
3. Assign each agent a single role, scope, input and expected output.
4. Identify tasks that can run in parallel and tasks requiring sequential handoff.
5. Define shared data formats and a single source of truth.
6. Require agents to cite evidence, label assumptions and report uncertainty.
7. Add a coordinator that checks completeness, conflicts and consistency.
8. Limit delegation depth, retries, tool permissions and total runtime.
9. Escalate unresolved conflicts or high-impact decisions to a human.
10. Evaluate the complete system, not only each agent in isolation.

## Handoff format
Each handoff should include: task, context, completed work, evidence, assumptions, open questions, files or references, and recommended next action.

## Deliverables
Task graph, agent role cards, handoff schema, shared-state design, failure policy and end-to-end test cases.

## Guardrails
Do not give every agent every tool. Prevent circular delegation and uncontrolled agent spawning. Treat another agent's output as unverified until checked.
