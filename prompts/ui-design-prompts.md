# UI Design Prompts

## Purpose
Review and improve interface layout, hierarchy, responsiveness, forms, portfolio cards, and design-to-code handoff.

## When To Use
Use before implementing UI changes or when a page feels unclear, crowded, or generic.

## Related Agents
- UI Agent
- UX Assessment Agent
- Web Development Agent
- Accessibility Agent

## Related Skills
- Code Review
- Requirements Discovery
- MVP Scope Control

## Related Workflows
- Web App Build Workflow
- Accessibility Audit Workflow
- UX Study Workflow

## Safety Notes
Do not use icon-dependent instructions. Do not deploy or write files without approval. Keep reviews personal-project focused and avoid job/workplace material.

## Prompts

### UI Critique
- Best use case: Improve a page.
- Prompt:
```text
Critique this UI: [description or screenshot notes].
Return: clarity issues, hierarchy issues, spacing/layout problems, interaction risks, accessibility risks, and prioritized fixes.
```
- Expected output: UI critique.
- Safety/approval gates: Review only.

### Homepage Layout Review
- Best use case: Improve landing/home page.
- Prompt:
```text
Review this homepage layout: [content or sections].
Return: first-viewport message, section order, scanning path, CTAs, proof points, mobile risks, and revised structure.
```
- Expected output: Homepage plan.
- Safety/approval gates: No file edits.

### Component Hierarchy
- Best use case: Clarify reusable UI.
- Prompt:
```text
Review the component hierarchy for this UI: [components].
Return: parent/child responsibilities, reusable components, state boundaries, naming, and simplification opportunities.
```
- Expected output: Component hierarchy plan.
- Safety/approval gates: No implementation.

### Visual Hierarchy
- Best use case: Make content easier to scan.
- Prompt:
```text
Improve visual hierarchy for this page: [content].
Return: primary message, secondary content, grouping, typography scale, spacing, emphasis, and what to remove.
```
- Expected output: Hierarchy recommendations.
- Safety/approval gates: No edits.

### Mobile Responsiveness
- Best use case: Catch mobile layout issues.
- Prompt:
```text
Review mobile responsiveness for this UI: [description].
Return: likely breakpoints, stacking order, tap targets, text wrapping risks, overflow risks, and mobile QA checklist.
```
- Expected output: Mobile review.
- Safety/approval gates: Test before launch.

### Form UX
- Best use case: Improve forms.
- Prompt:
```text
Review this form UX: [form fields/flow].
Return: field order, labels, helper text, validation, error states, success state, privacy copy, and accessibility checks.
```
- Expected output: Form UX plan.
- Safety/approval gates: No messages or submissions.

### Portfolio Project Card Design
- Best use case: Improve portfolio cards.
- Prompt:
```text
Review these portfolio project cards: [cards].
Return: card hierarchy, proof gaps, tech stack clarity, outcome clarity, link placement, mobile behavior, and revised card structure.
```
- Expected output: Better card design.
- Safety/approval gates: Avoid workplace-specific details.

### Design-To-Code Handoff
- Best use case: Prepare implementation.
- Prompt:
```text
Turn this UI plan into a design-to-code handoff: [plan].
Return: components, states, responsive rules, accessibility requirements, content slots, acceptance criteria, and files likely to change.
```
- Expected output: Implementation-ready handoff.
- Safety/approval gates: Approval before writing files.
