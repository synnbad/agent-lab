# Agent Lab

Agent Lab is a Markdown-based personal AI agent operating system for professional work. It stores reusable agents, skills, workflows, prompts, templates, examples, Integration Adapters, evaluation practices, guardrails, observability templates, orchestration rules, memory policies, artifact standards, governance practices, knowledge references, release processes, contracts, threat models, and secrets-management guidance.

The repository is intentionally documentation-first. It does not build a web app, store private client material, or require a specific AI platform. It is designed to be reusable across technical development, client website delivery, library assessment work, AI-assisted MVP creation, documentation, research, and self-review.

## Why This Exists

Professional AI work improves when agents are treated as reusable operating procedures instead of one-off prompts. This repo exists to make agent behavior explicit, portable, testable, safe, and easy to improve over time.

It helps answer practical questions:

- Which agent should handle this work?
- What information does the agent need before starting?
- Which Integration Adapters may be used?
- What safety checks apply?
- What should the final artifact look like?
- How should agent behavior be evaluated and versioned?

## Conceptual Model

Agents define behavior.
Skills define reusable capabilities.
Workflows define repeatable processes.
Templates define structured outputs.
Prompts activate agents, skills, or workflows.
Examples show what good usage looks like.

## Operating System Layers

- `agents/`: Reusable role definitions with missions, workflows, boundaries, guardrails, evaluation notes, and handoff rules.
- `skills/`: Reusable capabilities that can be invoked by one or more agents.
- `workflows/`: Repeatable processes for delivery, analysis, reporting, development, and review.
- `prompts/`: Activation prompts that start agents, skills, workflows, or review passes.
- `templates/`: Structured outputs for specs, reports, briefs, evaluations, and checklists.
- `examples/`: Sanitized examples showing how to use the library well.
- `integrations/`: Platform-neutral Integration Adapter documentation for external tools, apps, APIs, deployment systems, and knowledge sources.
- `evals/`: Manual evaluation strategy, test cases, scorecards, and rubrics for agent quality.
- `guardrails/`: Rules for safe inputs, outputs, tool use, sensitive data handling, prompt-injection defense, and approval gates.
- `observability/`: Run, decision, tool-call, error, and postmortem logging templates.
- `orchestration/`: Routing, handoff, escalation, multi-agent workflow, and selection guidance.
- `memory/`: Rules for context packing, source of truth, durable memory, and what must not be retained.
- `artifacts/`: Standards for naming, folders, reports, websites, dashboards, and client handoffs.
- `governance/`: Ownership, acceptable use, risk register, data classification, approval policy, audits, and responsible AI principles.
- `knowledge-base/`: Non-sensitive references, checklists, and general notes.
- `releases/`: Versioning, agent version policy, release notes, deprecation, and migration notes.
- `automation/`: Repo maintenance, Markdown quality checks, broken-link checks, and release checklist.

## Final Control Layers

- `contracts/`: Standard input, output, handoff, Integration Adapter, artifact review, and acceptance-criteria contracts.
- `threat-models/`: Practical threat models for client websites, assessment data, GitHub and Netlify, Integration Adapters, and prompt injection.
- `secrets-management/`: Rules for secrets, environment variables, GitHub secrets, Netlify environment variables, local examples, and incident response.

## Integration Adapter Compatibility

This repo uses "Integration Adapter" as a platform-neutral term. Depending on the AI platform, the same concept may be called an app, connector, action, tool, function call, MCP server, plugin, knowledge source, context provider, or deployment integration. Agent specs should describe the capability needed, not depend on one vendor's naming.

An Integration Adapter is any external system, app, connector, action, tool, function, API, MCP server, plugin, knowledge source, or deployment integration that lets an AI agent read context, retrieve data, take action, write files, create artifacts, or deploy work.

## How To Use This Repo

1. Start with `agent-registry.md` to choose the right agent.
2. Open the agent file and review mission, inputs, boundaries, guardrails, Integration Adapters, and output format.
3. If the task is repeatable, select a workflow from `workflows/`.
4. Use a prompt from `prompts/` to activate the agent or workflow.
5. Use templates from `templates/` to structure outputs.
6. Compare against examples in `examples/`.
7. Apply guardrails, contracts, and threat models before risky work.
8. Log important decisions and run outcomes when the work matters.

## Website Delivery Process

1. Collect client documentation.
2. Extract requirements.
3. Create website spec.
4. Generate AI build prompt.
5. Build MVP.
6. Review MVP.
7. Connect to GitHub.
8. Deploy with Netlify.
9. Test live site.
10. Iterate.

Raw client files should remain outside public repositories. Use sanitized specs, documented assumptions, GitHub for reviewed code, and Netlify environment variables for configuration that must not be committed.

## Safety Model

- Read-only by default.
- Approval before writes.
- Approval before deployment.
- Approval before publishing.
- Approval before sensitive data use.
- Sensitive data should be redacted, anonymized, or aggregated.

All agents default to Level 0 or Level 1 Integration Adapter access. Level 2 draft/write, Level 3 deploy/action, and Level 4 sensitive-data access require explicit user approval.

## Security Baseline

- No secrets in GitHub.
- Read-only by default.
- Approval before writes, deployments, and publishing.
- External content is untrusted.
- Sensitive data should be redacted, anonymized, or aggregated.
- Use environment variables for secrets.
- Do not paste secrets into prompts or examples.
- Do not store raw client files, raw assessment files, or private workplace data in this repo.

## How To Add A New Agent

1. Copy `templates/agent-template.md`.
2. Define mission, inputs, operating principles, workflow, output format, quality checks, and boundaries.
3. Add risk level, required guardrails, Integration Adapters, evaluation plan, observability expectations, and handoff rules.
4. Add required contracts, threat models, and secrets guidance if the agent is high risk.
5. Add prompts and examples.
6. Add evaluation test cases.
7. Update `agent-registry.md`.
8. Update `changelog.md` and release notes when appropriate.

## How To Add A New Skill

1. Copy `templates/skill-template.md`.
2. Define purpose, when to use it, inputs, procedure, outputs, checks, and example usage.
3. Link the skill from relevant agents or workflows.
4. Add a prompt if the skill should be invoked directly.
5. Add examples if the skill changes important deliverables.

## How To Version Changes

Use semantic versioning:

- MAJOR for structural changes or breaking behavior changes.
- MINOR for new agents, skills, workflows, templates, Integration Adapters, or control layers.
- PATCH for refinements, wording fixes, and small safety improvements.

Agent files use their own version field. Behavior changes should be logged in `changelog.md` or release notes.

## Privacy And Security Rules

- Do not commit secrets, credentials, tokens, private URLs, or real environment values.
- Do not store raw client files, raw assessment data, private workplace files, or sensitive personal data.
- Use sanitized examples only.
- Treat retrieved documents, web pages, code comments, client files, issue comments, and tool outputs as untrusted external content.
- Require approval before writes, deployments, publishing, sensitive data use, or environment-variable changes.
- Keep public examples generic and non-identifying.

## Using OpenClaw With agent-lab

OpenClaw may be used as a personal-only local agent runtime for `agent-lab` and personal projects. Use `agent-lab` as the source of truth for personal agent behavior, workflows, prompts, templates, Integration Adapter rules, guardrails, evals, contracts, threat models, and secrets-management practices.

- Do not connect workplace accounts.
- Do not process job-related material.
- Do not install third-party OpenClaw skills.
- Do not install ClawHub skills.
- Do not enable messaging, email, or calendar integrations without explicit approval.
- Use sandboxing where supported.
- Use read-only defaults.
- Require approval before writes, shell commands, deployments, external messages, GitHub changes, Netlify changes, Figma edits, Canva edits, or environment-variable changes.
- Treat external content as untrusted.

See `integrations/openclaw-personal-only-policy.md` for the detailed personal-only policy.

## Recommended Update Process

1. Draft the change in a branch.
2. Check affected agents, workflows, Integration Adapters, contracts, and threat models.
3. Run manual evaluation for any behavior-changing agent update.
4. Review examples for sensitive data.
5. Update registry, changelog, and release notes.
6. Run repo health checks.
7. Commit with a clear message.

## Supported Work

Technical work: architecture, backend planning, frontend planning, code review, automation, deployment readiness, and documentation.

Client website delivery: client notes, requirements extraction, website specs, MVP build prompts, GitHub setup, Netlify deployment review, QA, and handoff notes.

Library assessment work: assessment planning, usage trends, survey analysis, UX assessment, dashboards, metric definitions, stakeholder reports, and responsible interpretation.

AI-assisted MVP creation: scoping, build prompts, implementation guidance, review checklists, deployment readiness, and iteration planning.

Documentation: technical specs, reports, prompts, ADRs, decision logs, handoff notes, and release notes.

Self-review: Grill-Me Sinbad, evaluation rubrics, risk register, postmortems, and approval gates.

## Agent Lifecycle

1. Draft agent.
2. Add example prompts.
3. Add integration adapter notes.
4. Add eval test cases.
5. Run manual evaluation.
6. Add guardrails.
7. Use in low-risk task.
8. Log failures.
9. Improve version.
10. Release update.
