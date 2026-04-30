# Accessibility Prompts

## Purpose
Review and improve accessibility for personal websites, web apps, docs, and UI plans.

## When To Use
Use before launch, after UI changes, or when planning remediation.

## Related Agents
- Accessibility Agent
- UI Agent
- Web Development Agent

## Related Skills
- Code Review
- Technical Documentation
- Deployment Readiness Review

## Related Workflows
- Accessibility Audit Workflow
- Web App Build Workflow
- Client Website Delivery Workflow

## Safety Notes
Do not deploy or edit files without approval. Do not read hidden files or `.env` files. Keep reviews focused on personal projects.

## Prompts

### WCAG-Focused Page Review
- Best use case: Review a page for accessibility risks.
- Prompt:
```text
Review this page for WCAG-oriented accessibility risks: [page or code].
Return: issues by severity, affected users, evidence, remediation, and validation steps.
```
- Expected output: Prioritized accessibility review.
- Safety/approval gates: Review only.

### Alt Text Review
- Best use case: Improve image descriptions.
- Prompt:
```text
Review image alt text for this page: [image list/context].
Return: decorative vs informative classification, proposed alt text, missing context, and risks.
```
- Expected output: Alt text plan.
- Safety/approval gates: Do not invent visual details.

### Heading Structure
- Best use case: Fix document/page outline.
- Prompt:
```text
Review the heading structure: [outline or HTML].
Return: current outline, issues, revised outline, and why it improves navigation.
```
- Expected output: Heading remediation.
- Safety/approval gates: No edits without approval.

### Link Text
- Best use case: Make links meaningful.
- Prompt:
```text
Review link text in this content: [content].
Return: vague links, improved text, destination clarity, and keyboard/screen reader notes.
```
- Expected output: Link text fixes.
- Safety/approval gates: Draft only.

### Keyboard Navigation
- Best use case: Check interactive flows.
- Prompt:
```text
Plan a keyboard navigation audit for this UI: [UI description].
Return: tab order checks, focus traps, skip links, modals, menus, forms, and pass/fail checklist.
```
- Expected output: Keyboard audit checklist.
- Safety/approval gates: No browser automation unless approved.

### Focus States
- Best use case: Review visible focus.
- Prompt:
```text
Review focus state risks for this component set: [components].
Return: missing focus indicators, contrast risks, interaction states, and remediation guidance.
```
- Expected output: Focus remediation.
- Safety/approval gates: No implementation unless approved.

### Color Contrast Risk
- Best use case: Flag likely contrast problems.
- Prompt:
```text
Review this color and typography plan for contrast risk: [colors/content].
Return: likely failures, safer pairings, text-size concerns, and checks to run.
```
- Expected output: Contrast risk notes.
- Safety/approval gates: Verify with tooling before launch.

### Reduced Motion Review
- Best use case: Check animations.
- Prompt:
```text
Review motion/animation behavior: [description or code].
Return: motion risks, reduced-motion fallback, essential vs decorative motion, and test steps.
```
- Expected output: Reduced motion plan.
- Safety/approval gates: No edits without approval.

### Accessibility Remediation Checklist
- Best use case: Turn findings into work.
- Prompt:
```text
Convert these accessibility findings into a remediation checklist: [findings].
Return: priority, affected files, acceptance criteria, validation steps, and release risk.
```
- Expected output: Actionable checklist.
- Safety/approval gates: Approval before file edits.
