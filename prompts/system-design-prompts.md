# System Design Prompts

## Purpose
Design personal systems with clear architecture, tradeoffs, reliability, observability, failure modes, and MVP boundaries.

## When To Use
Use before building larger personal apps, automation systems, APIs, or integrations.

## Related Agents
- System Design Agent
- Backend Agent
- Web Development Agent
- Automation Agent

## Related Skills
- Architecture Review
- MVP Scope Control
- Requirements Discovery
- Technical Documentation

## Related Workflows
- System Design Workflow
- Backend API Workflow
- Web App Build Workflow
- Integration Safety Review Workflow

## Safety Notes
Do not connect accounts or deploy systems without approval. Do not include secrets or private data. Keep external integrations disabled unless explicitly approved.

## Prompts

### System Architecture
- Best use case: Design a new system.
- Prompt:
```text
Design the architecture for this personal system: [system].
Return: context, components, data flow, storage, APIs, dependencies, risks, MVP version, and future version.
```
- Expected output: Architecture plan.
- Safety/approval gates: Planning only.

### Tradeoff Analysis
- Best use case: Choose between options.
- Prompt:
```text
Compare these architecture options: [options].
Return: decision matrix, cost/complexity, security, reliability, maintainability, user impact, and recommendation.
```
- Expected output: Tradeoff decision.
- Safety/approval gates: No implementation.

### Scaling Plan
- Best use case: Avoid premature scaling.
- Prompt:
```text
Create a scaling plan for this personal app: [app].
Return: current expected load, bottlenecks, MVP limits, low-cost scaling path, and when to revisit.
```
- Expected output: Scaling notes.
- Safety/approval gates: No infrastructure changes.

### Reliability Review
- Best use case: Find weak spots.
- Prompt:
```text
Review this system for reliability: [design].
Return: single points of failure, data loss risks, retry behavior, backup needs, graceful degradation, and validation checks.
```
- Expected output: Reliability review.
- Safety/approval gates: No deployment.

### Observability Plan
- Best use case: Decide what to monitor.
- Prompt:
```text
Create an observability plan for this personal system: [system].
Return: logs, metrics, traces/events, alerts, dashboards, redaction rules, and manual troubleshooting steps.
```
- Expected output: Observability plan.
- Safety/approval gates: No account connections.

### Failure Modes
- Best use case: Stress-test a design.
- Prompt:
```text
List failure modes for this architecture: [architecture].
Return: failure, trigger, impact, detection, mitigation, rollback, and test idea.
```
- Expected output: Failure mode table.
- Safety/approval gates: No destructive testing.

### Architecture Decision Record
- Best use case: Document decisions.
- Prompt:
```text
Draft an ADR using templates/architecture-decision-record-template.md.
Decision: [decision]
Return: context, options, decision, consequences, risks, and follow-up.
```
- Expected output: ADR draft.
- Safety/approval gates: Draft only.

### MVP Vs Future Architecture
- Best use case: Keep architecture lean.
- Prompt:
```text
Split this architecture into MVP and future phases: [architecture].
Return: must-build now, defer, cut, migration path, risk accepted, and approval gates.
```
- Expected output: Phased architecture.
- Safety/approval gates: No build without approval.
