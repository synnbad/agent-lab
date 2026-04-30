# UX Assessment Prompts

## Purpose
Plan and synthesize usability, heuristic, and experience reviews for personal websites and apps.

## When To Use
Use before redesigning a flow, after launch feedback, or when a UI feels confusing.

## Related Agents
- UX Assessment Agent
- UI Agent
- Accessibility Agent
- Web Development Agent

## Related Skills
- Requirements Discovery
- Mixed Methods Synthesis
- Technical Documentation

## Related Workflows
- UX Study Workflow
- Accessibility Audit Workflow
- Web App Build Workflow

## Safety Notes
Use redacted feedback. Do not include private identities or workplace material. Do not record or contact users without approval.

## Prompts

### UX Study Plan
- Best use case: Plan a lightweight study.
- Prompt:
```text
Plan a lightweight UX study for this personal project: [project].
Return: goal, participants, tasks, prompts, success measures, notes template, risks, and consent/privacy language.
```
- Expected output: UX study plan.
- Safety/approval gates: No outreach without approval.

### Heuristic Review
- Best use case: Evaluate UX without users.
- Prompt:
```text
Run a heuristic review on this UI: [description].
Return: usability issues, severity, affected flow, evidence, fix recommendation, and priority.
```
- Expected output: Heuristic report.
- Safety/approval gates: Review only.

### User Journey Review
- Best use case: Improve end-to-end flow.
- Prompt:
```text
Map the user journey for this personal app/site: [flow].
Return: stages, user goal, friction, emotion, missing feedback, accessibility risks, and improvements.
```
- Expected output: Journey map.
- Safety/approval gates: No edits.

### Usability Findings Synthesis
- Best use case: Turn notes into findings.
- Prompt:
```text
Synthesize these redacted usability notes: [notes].
Return: themes, evidence, severity, recommendations, design implications, and follow-up questions.
```
- Expected output: Findings synthesis.
- Safety/approval gates: Redact private details.

### UX Remediation Plan
- Best use case: Convert findings into work.
- Prompt:
```text
Create a remediation plan from these UX findings: [findings].
Return: quick wins, design changes, content changes, technical changes, validation steps, and approval gates.
```
- Expected output: UX action plan.
- Safety/approval gates: Ask before implementation.
