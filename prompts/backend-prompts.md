# Backend Prompts

## Purpose
Plan and review APIs, data models, validation, authorization, errors, logging, security, and backend implementation.

## When To Use
Use for personal backend services, serverless functions, API routes, or backend portions of web apps.

## Related Agents
- Backend Agent
- System Design Agent
- Web Development Agent
- Data Governance Privacy Agent

## Related Skills
- Architecture Review
- Code Review
- Data Privacy Review
- Technical Documentation

## Related Workflows
- Backend API Workflow
- System Design Workflow
- Web App Build Workflow

## Safety Notes
Do not read hidden files or `.env` files. Do not print secrets. Do not connect databases, services, or accounts without approval. Do not deploy without approval.

## Prompts

### API Design
- Best use case: Plan endpoints.
- Prompt:
```text
Design an API for this personal project: [project].
Return: resources, endpoints, request/response shapes, validation, error codes, auth assumptions, rate limits, and acceptance criteria.
```
- Expected output: API spec.
- Safety/approval gates: No implementation.

### Data Model Planning
- Best use case: Define entities and relationships.
- Prompt:
```text
Plan the data model for this personal app: [app].
Return: entities, fields, relationships, indexes, constraints, privacy risks, and migration notes.
```
- Expected output: Data model plan.
- Safety/approval gates: No database changes.

### Validation Strategy
- Best use case: Prevent bad inputs.
- Prompt:
```text
Create a validation strategy for this API/form: [description].
Return: field rules, cross-field rules, server/client validation split, error messages, and tests.
```
- Expected output: Validation plan.
- Safety/approval gates: No code changes without approval.

### Auth And Authorization Planning
- Best use case: Scope access safely.
- Prompt:
```text
Plan authentication and authorization for this personal backend: [backend].
Return: roles, permissions, session/token assumptions, protected routes, abuse cases, and simpler alternatives.
```
- Expected output: Auth plan.
- Safety/approval gates: No account connections.

### Error Handling
- Best use case: Make failures predictable.
- Prompt:
```text
Design error handling for this backend flow: [flow].
Return: expected errors, user-facing messages, logs, retries, fallbacks, and test cases.
```
- Expected output: Error strategy.
- Safety/approval gates: Do not log secrets.

### Logging
- Best use case: Add observability without leaking data.
- Prompt:
```text
Design backend logging for this service: [service].
Return: events, fields, redactions, log levels, correlation IDs, retention concerns, and examples.
```
- Expected output: Logging plan.
- Safety/approval gates: No private data in logs.

### Security Review
- Best use case: Review backend risk.
- Prompt:
```text
Review this backend design for security: [design].
Check input validation, auth, secrets, injection risk, rate limiting, CORS, dependencies, logging, and deployment risk.
```
- Expected output: Security review.
- Safety/approval gates: No exploit execution.

### Backend Implementation
- Best use case: Implement approved backend work.
- Prompt:
```text
Implement the approved backend change in this personal repo: [repo path].
Approved files: [files]
Do not read hidden files or `.env` files. Do not print secrets. Do not deploy, commit, push, or connect accounts. Run safe validation and summarize changes.
```
- Expected output: Backend change and validation.
- Safety/approval gates: Stop before commit/deploy.
