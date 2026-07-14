# Example AI Workflow Approval Gate

## Gate

`APPROVE_EXAMPLE_READ_ONLY_PILOT_ONLY`

## Business purpose

Validate whether a bounded AI workflow can summarise approved internal documents while preserving human accountability and data boundaries.

## Authorised scope

- read the exact approved document allowlist;
- generate a draft summary;
- identify missing or contradictory evidence;
- return the draft for human review.

## Prohibited scope

- no external publication;
- no customer or restricted data;
- no automated decisions;
- no write-back to source systems;
- no scope expansion;
- no automatic next stage.

## Acceptance criteria

- all inputs are on the allowlist;
- all material statements cite an approved source;
- uncertainty and missing evidence are explicit;
- the human reviewer accepts or rejects the output;
- audit evidence is retained;
- no prohibited action occurs.

## Stop conditions

Stop and escalate when:

- required evidence is missing;
- sensitive data is detected;
- the model requests another permission;
- output validation fails;
- the workflow attempts a write.

## Decision

```text
currently_authorized=false
automatic_start=false
final_authority=human_reviewer
```
