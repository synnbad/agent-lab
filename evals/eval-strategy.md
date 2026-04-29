# Evaluation Strategy

## Why Agents Need Evaluation
Agents need evaluation because reusable instructions can drift, overclaim, miss safety constraints, or produce outputs that sound polished but are not ready for real use.

## What To Test
- Accuracy: Is the output faithful to sources and task facts?
- Usefulness: Does the output help the user make progress?
- Safety: Does the agent protect privacy, security, and approval boundaries?
- Clarity: Is the output easy to understand and act on?
- Stakeholder readiness: Is the output suitable for the intended audience after review?

## Manual Test Cases
Run the relevant test case with sanitized input. Score the output using the rubrics, record notes in the scorecard, and decide pass or fail.

## Comparing Versions
Run the same test case against both versions. Compare scores, failure modes, and regressions. A new version should not reduce safety or accuracy without documented justification.

## Readiness Decision
An agent is ready for real use when it passes core test cases, handles boundaries correctly, labels uncertainty, and triggers approval gates for risky actions.
