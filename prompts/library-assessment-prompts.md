# Library Assessment Prompts

## Purpose
Support generic collection, resource, and service assessment-style projects using public, personal, synthetic, or redacted data.

## When To Use
Use for personal learning projects, portfolio case studies, or public-data assessment simulations.

## Related Agents
- Research Agent
- Data Analysis Agent
- Writing Agent

## Related Skills
- Assessment Question Design
- Assessment Report Writing
- Mixed Methods Synthesis
- Data Privacy Review

## Related Workflows
- Library Assessment Cycle Workflow
- Data Analysis Workflow
- Report Generation Workflow

## Safety Notes
Do not use workplace material or institutional datasets. Use generic "blocked workplace-related items" wording for anything outside personal/public scope.

## Prompts

### Assessment Question Design
- Best use case: Create evaluation questions.
- Prompt:
```text
Design assessment questions for this public or personal learning project: [project].
Return: primary questions, subquestions, data needed, methods, limitations, and privacy notes.
```
- Expected output: Assessment question set.
- Safety/approval gates: No workplace data.

### Assessment Plan
- Best use case: Plan an assessment cycle.
- Prompt:
```text
Create an assessment plan for this generic project: [project].
Return: purpose, audience, methods, data sources, timeline, analysis plan, risks, and reporting format.
```
- Expected output: Assessment plan.
- Safety/approval gates: Use safe data only.

### Mixed Methods Synthesis
- Best use case: Combine qualitative and quantitative notes.
- Prompt:
```text
Synthesize these safe assessment notes: [notes].
Return: quantitative findings, qualitative themes, convergence, contradictions, limitations, and recommendations.
```
- Expected output: Synthesis summary.
- Safety/approval gates: Redact private details.

### Assessment Report
- Best use case: Write a final report.
- Prompt:
```text
Draft an assessment-style report from these safe findings: [findings].
Return: executive summary, method, findings, limitations, recommendations, and appendix needs.
```
- Expected output: Report draft.
- Safety/approval gates: No private/raw data.

### Portfolio Case Study
- Best use case: Turn assessment work into public portfolio content.
- Prompt:
```text
Convert this generic assessment project into a portfolio case study: [notes].
Return: problem, method, tools, findings, impact, limitations, and sanitized project card copy.
```
- Expected output: Portfolio case study.
- Safety/approval gates: Avoid workplace-specific details.
