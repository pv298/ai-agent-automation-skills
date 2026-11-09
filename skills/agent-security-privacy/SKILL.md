---
name: agent-security-privacy
description: Review AI agents and automation workflows for prompt injection, data leakage, excessive permissions, unsafe tool actions, secret exposure and privacy risks. Use during design, testing and security reviews.
---

# Agent Security and Privacy

## Threat review
Consider malicious user inputs, prompt injection in retrieved content, compromised tools, leaked credentials, excessive permissions, data exfiltration, unsafe code execution and unintended external actions.

## Workflow
1. Inventory data, tools, identities, trust boundaries and external destinations.
2. Classify data and define allowed processing, storage and retention.
3. Apply least privilege to users, agents, service accounts and API credentials.
4. Keep secrets in managed credential stores; rotate and revoke when needed.
5. Treat retrieved web pages, files, emails and tool outputs as untrusted data.
6. Validate and constrain tool arguments; use allowlists where practical.
7. Separate planning from execution and require approval for high-impact actions.
8. Limit file, network and code execution capabilities to the task.
9. Redact logs and define incident detection, response and recovery.
10. Test prompt injection, data exfiltration attempts, authorization boundaries and failure modes.

## Deliverables
Threat model, data-flow map, permission matrix, control checklist, test cases and incident response plan.

## Guardrails
Prompt instructions are not a substitute for access controls. Never publish secrets or personal data. Do not design systems to evade security controls, exfiltrate data or perform unauthorized actions. Follow applicable laws, contracts and platform policies.
