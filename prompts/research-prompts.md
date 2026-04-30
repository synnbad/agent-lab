# Research Prompts

## Purpose
Support safe public research, source comparison, claim checking, and citation-aware summaries.

## When To Use
Use when you need to refine a research question, compare sources, synthesize evidence, or summarize public information.

## Related Agents
- Research Agent
- Writing Agent
- Data Analysis Agent

## Related Skills
- Literature Review
- Mixed Methods Synthesis
- Technical Documentation

## Related Workflows
- Report Generation Workflow
- Data Analysis Workflow
- Project Triage Workflow

## Safety Notes
Use public or user-provided non-sensitive sources. Do not access job/workplace material. Do not paste private documents or secrets.

## Prompts

### Research Question Refinement
- Best use case: Turn an interest into a researchable question.
- Prompt:
```text
Refine this research interest into clear questions: [interest].
Return: primary question, subquestions, scope boundaries, keywords, source types, and exclusion criteria.
```
- Expected output: Research plan.
- Safety/approval gates: Public/non-sensitive topics only.

### Source Comparison
- Best use case: Compare competing sources.
- Prompt:
```text
Compare these public sources: [sources or summaries].
Return: claims, evidence quality, conflicts, dates, author credibility, limitations, and which claims are strongest.
```
- Expected output: Source comparison table.
- Safety/approval gates: Cite sources when browsing is used.

### Claim Checking
- Best use case: Verify a claim.
- Prompt:
```text
Check this claim using reliable public evidence: [claim].
Return: verdict, evidence, counterevidence, uncertainty, date sensitivity, and what would change the conclusion.
```
- Expected output: Claim check.
- Safety/approval gates: Browse only if approved or available.

### Literature-Style Synthesis
- Best use case: Summarize themes across sources.
- Prompt:
```text
Synthesize these source notes: [notes].
Return: themes, agreements, disagreements, evidence gaps, limitations, and practical implications.
```
- Expected output: Synthesis memo.
- Safety/approval gates: No private source material.

### Public Web Research
- Best use case: Research current public facts.
- Prompt:
```text
Conduct public web research on: [topic].
Use reliable sources, note dates, avoid private accounts, and return citations, summary, evidence table, limitations, and next questions.
```
- Expected output: Cited public research.
- Safety/approval gates: No account connections.

### Evidence Table
- Best use case: Organize research evidence.
- Prompt:
```text
Create an evidence table for this question: [question].
Columns: claim, source, evidence, date, quality, caveat, relevance, and confidence.
```
- Expected output: Evidence table.
- Safety/approval gates: Public evidence only.

### Citation-Aware Summary
- Best use case: Summarize with attribution.
- Prompt:
```text
Summarize these sources with citations: [sources].
Return: concise summary, citation map, strongest evidence, weak evidence, and open questions.
```
- Expected output: Attributed summary.
- Safety/approval gates: Avoid overquoting.
