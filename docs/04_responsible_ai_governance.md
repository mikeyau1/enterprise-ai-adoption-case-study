# 4. Responsible AI Governance

## Control objectives

Responsible AI governance should ensure that a use case is lawful, appropriate, understandable, secure, monitored and subject to meaningful human authority.

## Risk domains

### Data and privacy

- classify data before use;
- minimise the data shared with a model;
- prohibit unsupported sensitive-data use;
- use explicit allowlists rather than broad access;
- define retention and deletion expectations;
- record cross-border and residency constraints.

### Model and output risk

- document the model and intended task;
- define known limitations;
- require source attribution where decisions depend on facts;
- validate outputs independently;
- prevent unsupported automated decisions;
- monitor changes in model behaviour or availability.

### Operational risk

- require clean baselines before material changes;
- separate read-only and write authority;
- use exact approval boundaries;
- preserve audit trails;
- test rollback procedures;
- prohibit silent scope expansion.

### Human and conduct risk

- make accountability explicit;
- train users on appropriate and inappropriate use;
- provide escalation routes;
- avoid incentives based only on usage volume;
- assess impacts on customers, employees and vulnerable groups.

## Risk-tier example

| Tier | Example | Typical control posture |
|---|---|---|
| Low | Drafting internal summaries from non-sensitive text | User review and approved tool |
| Moderate | Workflow recommendations using internal information | Data approval, validation and monitoring |
| High | Customer, financial or regulated decision support | Formal governance, independent assurance and strong human control |
| Prohibited | Unreviewed autonomous decisions or unapproved protected-data use | Do not proceed |

## Fail-closed principle

When required evidence, permission or data classification is missing, the workflow should stop rather than infer authority. A blocked workflow is safer than a persuasive but unsupported completion.

## Evidence expected for approval

- use-case record;
- risk assessment;
- data classification;
- human-oversight design;
- test and validation results;
- user training plan;
- monitoring metrics;
- incident and rollback plan;
- named approvers.
