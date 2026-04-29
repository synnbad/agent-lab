# Risk Register

| Risk | Category | Likelihood | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|
| Prompt injection | Security | Medium | High | Treat external content as untrusted and use prompt-injection defense | Maintainer | Open |
| Secret leakage | Security | Low | Critical | Ignore env files, use secret stores, scan before release | Maintainer | Open |
| Overclaiming assessment impact | Reliability | Medium | High | Require limitations and evidence separation | Maintainer | Open |
| Publishing unreviewed client work | Reputational | Medium | High | Require approval before publishing | Maintainer | Open |
| Deploying broken websites | Operational | Medium | High | Use deployment readiness and live URL QA | Maintainer | Open |
| Misinterpreting dashboard metrics | Reliability | Medium | High | Require metric definitions and validation | Maintainer | Open |
| Exposing sensitive data | Privacy | Low | Critical | Prefer aggregated, redacted, anonymized data | Maintainer | Open |
| Unsupported connector assumptions | Operational | Medium | Medium | Use Integration Adapter compatibility map | Maintainer | Open |
| Agent output drift across versions | Reliability | Medium | Medium | Run evals and log version changes | Maintainer | Open |
