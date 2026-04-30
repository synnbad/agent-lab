# Dashboard Reporting Prompts

## Purpose
Plan personal or public-data dashboards and reports with clear metrics, privacy boundaries, and narrative structure.

## When To Use
Use for personal dashboards, public datasets, portfolio data stories, or non-sensitive reporting prototypes.

## Related Agents
- Data Analysis Agent
- Writing Agent
- UI Agent

## Related Skills
- Dashboard Quality Review
- Dashboard Storytelling
- Metric Definition
- Data Privacy Review

## Related Workflows
- Dashboard Development Workflow
- Data Analysis Workflow
- Report Generation Workflow

## Safety Notes
Do not use workplace datasets. Do not include private identifiers, secrets, or raw sensitive data. Ask before writing files or connecting data sources.

## Prompts

### Dashboard Requirements
- Best use case: Define dashboard purpose.
- Prompt:
```text
Draft dashboard requirements for this personal/public data project: [project].
Return: audience, decisions supported, metrics, filters, views, data sources, privacy risks, and acceptance criteria.
```
- Expected output: Dashboard requirements.
- Safety/approval gates: No data connection.

### Metric Review
- Best use case: Validate metrics.
- Prompt:
```text
Review these dashboard metrics: [metrics].
Return: definitions, formulas, grains, caveats, misleading interpretations, and improvements.
```
- Expected output: Metric critique.
- Safety/approval gates: No sensitive data.

### Dashboard Story
- Best use case: Improve narrative.
- Prompt:
```text
Create a dashboard story from these safe findings: [findings].
Return: headline, narrative sequence, chart roles, annotations, caveats, and action prompts.
```
- Expected output: Storyboard.
- Safety/approval gates: No private data.

### Dashboard Quality Review
- Best use case: Review dashboard before sharing.
- Prompt:
```text
Review this dashboard plan: [plan].
Check clarity, metric quality, layout, accessibility, privacy, performance, and misleading visuals. Return prioritized fixes.
```
- Expected output: Quality review.
- Safety/approval gates: No publishing.

### Report Companion
- Best use case: Pair dashboard with written summary.
- Prompt:
```text
Draft a report companion for this dashboard: [dashboard notes].
Return: summary, key insights, limitations, methodology, and recommended next steps.
```
- Expected output: Report draft.
- Safety/approval gates: Redact sensitive details.
