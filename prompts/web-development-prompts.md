# Web Development Prompts

## Purpose
Plan, inspect, review, and safely implement personal web apps and websites.

## When To Use
Use for React/Vite apps, routing, components, state/data flow, build errors, performance, and accessibility-aware reviews.

## Related Agents
- Web Development Agent
- UI Agent
- Backend Agent
- Accessibility Agent

## Related Skills
- Code Review
- Architecture Review
- Technical Documentation
- Deployment Readiness Review

## Related Workflows
- Web App Build Workflow
- Accessibility Audit Workflow
- Backend API Workflow
- Client Website Delivery Workflow

## Safety Notes
Do not read hidden files or `.env` files. Do not access job/workplace material. Ask before writing files. Do not commit, push, deploy, or connect accounts unless approved.

## Prompts

### Web App Planning
- Best use case: Plan before building.
- Prompt:
```text
Plan a personal web app for this idea: [idea].
Return: user goal, routes, components, data model, state flow, API needs, accessibility notes, MVP scope, deferred scope, and build steps.
```
- Expected output: Build plan.
- Safety/approval gates: No implementation.

### React/Vite Project Inspection
- Best use case: Understand an existing app.
- Prompt:
```text
Inspect this React/Vite project in read-only mode: [path].
Allowed: non-hidden source, config, package scripts, docs. Forbidden: hidden files, `.env`, secrets.
Return: stack, routes, components, state/data flow, scripts, risks, and recommended next step.
```
- Expected output: Project summary.
- Safety/approval gates: Read-only.

### Component Structure Review
- Best use case: Improve maintainability.
- Prompt:
```text
Review component structure for this app: [path or notes].
Return: component responsibilities, duplication, prop/data flow, naming, reusable pieces, and refactor recommendations.
```
- Expected output: Component review.
- Safety/approval gates: No edits unless approved.

### Routing Review
- Best use case: Check navigation.
- Prompt:
```text
Review routing for this web app: [routes or code].
Return: route map, broken/unclear flows, accessibility notes, loading/error states, and recommended changes.
```
- Expected output: Routing assessment.
- Safety/approval gates: Review only.

### State And Data Flow Review
- Best use case: Simplify data flow.
- Prompt:
```text
Review state and data flow: [description or files].
Return: sources of truth, derived state, side effects, API boundaries, caching needs, and simplification plan.
```
- Expected output: Data flow map.
- Safety/approval gates: No implementation.

### Build Error Triage
- Best use case: Fix broken build.
- Prompt:
```text
Triage this build error: [error].
Inspect relevant non-hidden files only. Return: root cause, minimal fix, validation command, and regression risk.
```
- Expected output: Fix plan or safe fix.
- Safety/approval gates: Ask before editing.

### Performance Review
- Best use case: Improve page speed.
- Prompt:
```text
Review this web app for performance risks.
Check bundle size, images/media, rendering patterns, data loading, unnecessary dependencies, and caching. Return prioritized fixes.
```
- Expected output: Performance plan.
- Safety/approval gates: No package installs without approval.

### Accessibility-Aware Frontend Review
- Best use case: Combine frontend and accessibility.
- Prompt:
```text
Review this frontend for accessibility-aware implementation.
Check semantics, headings, controls, forms, focus, keyboard flow, link text, alt text, and responsive behavior. Return issues and fixes.
```
- Expected output: Frontend accessibility review.
- Safety/approval gates: No edits without approval.
