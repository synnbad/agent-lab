# Stakeholder Insight Prompts

## Purpose
Turn personal project feedback, audience notes, or user research into clear insights and briefings.

## When To Use
Use for personal clients, collaborators, users, or public audience analysis.

## Related Agents
- Writing Agent
- Research Agent
- Data Analysis Agent

## Related Skills
- Stakeholder Briefing
- Mixed Methods Synthesis
- Requirements Discovery
- Data Privacy Review

## Related Workflows
- Stakeholder Reporting Workflow
- Report Generation Workflow
- Project Triage Workflow

## Safety Notes
Do not include private identities, raw client files, or workplace material. Redact sensitive details before summarizing.

## Prompts

### Audience Map
- Best use case: Clarify who the project serves.
- Prompt:
```text
Map the audience for this personal project: [project].
Return: audience segments, needs, anxieties, success criteria, content implications, and product implications.
```
- Expected output: Audience map.
- Safety/approval gates: No private identifiers.

### Feedback Synthesis
- Best use case: Turn feedback into themes.
- Prompt:
```text
Synthesize this redacted feedback: [feedback].
Return: themes, evidence, conflicts, priority, likely actions, and questions to ask next.
```
- Expected output: Feedback themes.
- Safety/approval gates: Redacted input only.

### Insight Brief
- Best use case: Create a concise briefing.
- Prompt:
```text
Create an insight brief from these safe notes: [notes].
Return: summary, top insights, evidence, implications, risks, and recommended next steps.
```
- Expected output: Briefing draft.
- Safety/approval gates: Draft only.

### Decision Support
- Best use case: Use insights to choose direction.
- Prompt:
```text
Use these audience insights to support a decision: [insights].
Return: decision options, evidence, tradeoffs, recommendation, and open questions.
```
- Expected output: Decision memo.
- Safety/approval gates: No external actions.

### Briefing Review
- Best use case: Check clarity and privacy.
- Prompt:
```text
Review this briefing for clarity, privacy, and actionability: [briefing].
Return: unclear claims, missing evidence, sensitive details to redact, and revised summary.
```
- Expected output: Safer briefing.
- Safety/approval gates: Do not publish.
