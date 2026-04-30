# Survey Assessment Prompts

## Purpose
Plan, review, analyze, and report on personal or public survey-style feedback projects.

## When To Use
Use for personal project feedback, portfolio research exercises, or redacted client discovery.

## Related Agents
- Research Agent
- Data Analysis Agent
- Writing Agent

## Related Skills
- Survey Instrument Design
- Assessment Question Design
- Mixed Methods Synthesis
- Data Privacy Review

## Related Workflows
- Survey To Insight Workflow
- Data Analysis Workflow
- Report Generation Workflow

## Safety Notes
Do not collect or expose sensitive personal data without explicit approval. Do not use workplace survey data. Redact private identifiers.

## Prompts

### Survey Goal Definition
- Best use case: Clarify why a survey exists.
- Prompt:
```text
Define the goal for this personal survey: [goal].
Return: research questions, audience, decisions supported, data needed, privacy risks, and success criteria.
```
- Expected output: Survey goal plan.
- Safety/approval gates: No collection yet.

### Survey Instrument Draft
- Best use case: Write questions.
- Prompt:
```text
Draft a survey instrument for this personal/public use case: [use case].
Return: intro text, consent/privacy note, questions, response options, skip logic, and bias risks.
```
- Expected output: Survey draft.
- Safety/approval gates: Review before sharing.

### Survey Quality Review
- Best use case: Improve a survey.
- Prompt:
```text
Review this survey for quality: [survey].
Check leading questions, double-barreled items, missing options, accessibility, privacy, length, and analysis readiness.
```
- Expected output: Survey critique.
- Safety/approval gates: No sending.

### Survey Analysis Plan
- Best use case: Prepare analysis before collection.
- Prompt:
```text
Create an analysis plan for this survey: [survey].
Return: metrics, cross-tabs, qualitative coding, limitations, data cleaning, and reporting outputs.
```
- Expected output: Analysis plan.
- Safety/approval gates: No raw sensitive data.

### Survey Findings Report
- Best use case: Summarize results.
- Prompt:
```text
Summarize these redacted survey results: [results].
Return: key findings, charts to create, quotes/themes, limitations, recommendations, and next steps.
```
- Expected output: Findings summary.
- Safety/approval gates: Redact identifiers.
