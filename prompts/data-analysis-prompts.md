# Data Analysis Prompts

## Purpose
Plan and produce privacy-safe personal or public data analysis.

## When To Use
Use for exploratory analysis, cleaning plans, metric definitions, dashboard planning, and report-ready findings.

## Related Agents
- Data Analysis Agent
- Data Governance Privacy Agent
- Writing Agent
- Research Agent

## Related Skills
- Data Cleaning
- Metric Definition
- Data Privacy Review
- Dashboard Storytelling
- Mixed Methods Synthesis

## Related Workflows
- Data Analysis Workflow
- Report Generation Workflow
- Project Triage Workflow

## Safety Notes
Keep datasets personal, public, redacted, or synthetic. Do not include workplace-specific datasets. Do not print secrets or private identifiers. Ask before writing files or generating reports from sensitive data.

## Prompts

### Exploratory Data Analysis
- Best use case: Understand a safe dataset.
- Prompt:
```text
Plan an exploratory data analysis for this personal/public dataset: [dataset description].
Return: questions, fields to inspect, quality checks, summary stats, visual ideas, privacy risks, and expected findings format.
```
- Expected output: EDA plan.
- Safety/approval gates: No sensitive data exposure.

### Cleaning Plan
- Best use case: Prepare messy data.
- Prompt:
```text
Create a data cleaning plan for this dataset: [description].
Return: missingness checks, type normalization, deduping, outlier handling, derived fields, validation rules, and audit notes.
```
- Expected output: Cleaning checklist.
- Safety/approval gates: Ask before modifying source data.

### Metric Definitions
- Best use case: Define clear measures.
- Prompt:
```text
Define metrics for this analysis goal: [goal].
For each metric return: name, definition, formula, grain, filters, caveats, examples, and misuse risks.
```
- Expected output: Metric dictionary.
- Safety/approval gates: Do not infer private facts.

### Dashboard Planning
- Best use case: Plan a personal dashboard.
- Prompt:
```text
Plan a dashboard for this personal/public data use case: [use case].
Return: audience, decisions supported, key metrics, views, filters, data freshness, accessibility notes, and risks.
```
- Expected output: Dashboard spec.
- Safety/approval gates: No workplace dashboards.

### Report-Ready Findings
- Best use case: Turn analysis into a narrative.
- Prompt:
```text
Turn these safe analysis notes into report-ready findings: [notes].
Return: executive summary, key findings, evidence, limitations, caveats, recommended next steps, and plain-language version.
```
- Expected output: Findings report.
- Safety/approval gates: Redact private data.

### Limitations Review
- Best use case: Prevent overclaiming.
- Prompt:
```text
Review this analysis for limitations: [analysis].
Identify sample issues, missing data, confounders, measurement flaws, privacy risk, uncertainty, and claims to soften.
```
- Expected output: Limitations section.
- Safety/approval gates: No unsupported claims.

### Data Storytelling
- Best use case: Build a clear narrative.
- Prompt:
```text
Create a data story from these safe findings: [findings].
Return: audience, headline, narrative arc, key chart ideas, annotations, caveats, and call to action.
```
- Expected output: Storytelling outline.
- Safety/approval gates: Keep generic and non-sensitive.

### Privacy-Safe Analysis
- Best use case: Check data risk.
- Prompt:
```text
Review this analysis plan for privacy risk: [plan].
Return: sensitive fields, re-identification risk, aggregation needs, redaction needs, allowed outputs, blocked outputs, and approval gates.
```
- Expected output: Privacy review.
- Safety/approval gates: Do not process sensitive raw data without approval.
