# AI Agent & Automation Skills

An open-source collection of practical agent skills, automation patterns, integration guides and implementation templates for builders, marketers, operators and developers.

The repository focuses on reusable workflows: define a task, provide the right context and tools, execute safely, verify the result and document what happened.

## Skill library

Browse the [skills index](skills/README.md).

### AI agent engineering
- [Agent design and architecture](skills/agent-design/SKILL.md)
- [Tool calling and integrations](skills/tool-use/SKILL.md)
- [Multi-agent orchestration](skills/multi-agent-orchestration/SKILL.md)
- [Prompt engineering](skills/prompt-engineering/SKILL.md)
- [Retrieval-augmented generation (RAG)](skills/rag-systems/SKILL.md)

### Automation and integrations
- [n8n workflow automation](skills/n8n-automation/SKILL.md)
- [Make.com scenario automation](skills/make-automation/SKILL.md)
- [APIs and webhooks](skills/api-webhooks/SKILL.md)
- [Browser automation](skills/browser-automation/SKILL.md)
- [CRM and lead operations](skills/crm-lead-automation/SKILL.md)

### Reliability and governance
- [Agent evaluation and observability](skills/evaluation-observability/SKILL.md)
- [Security and privacy](skills/agent-security-privacy/SKILL.md)

## Templates
- [Automation project brief](templates/automation-project-brief.md)
- [Agent test plan](templates/agent-test-plan.md)

## How to use a skill

1. Open the relevant `SKILL.md`.
2. Check its prerequisites and required context.
3. Give your agent the task, constraints, relevant data and permitted tools.
4. Ask it to follow the workflow and return the specified deliverables.
5. Test in a safe environment before connecting production systems.
6. Review actions, logs and outputs; keep a human approval step for consequential actions.

## Design principles

- Start with the simplest reliable workflow; use an autonomous agent only when the task needs one.
- Use least-privilege credentials and narrowly scoped tools.
- Validate inputs and outputs at system boundaries.
- Make workflows observable, retry-safe and recoverable.
- Require approval before sending external messages, spending money, deleting data or changing production systems.
- Never expose secrets, tokens or personal data in prompts, logs or public issues.
- Document assumptions and distinguish tested behaviour from examples.

## Compatibility

Skills are written in Markdown with YAML frontmatter and follow a portable folder-based convention. They are guidance files, not executable plugins. Tool availability, skill loading and execution behaviour depend on the agent platform.

## Maintainers

- [FSIDM — Full Stack Institute of Digital Marketing](https://fsidm.in/)
- [Pranav Veerani](https://pranavveerani.com/)

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Suggestions, examples and tested improvements are welcome.

## License

Original repository content is licensed under the MIT License. Third-party names, services and trademarks belong to their respective owners.
