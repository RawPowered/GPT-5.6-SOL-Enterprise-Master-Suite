# Evaluation playbook

A polished prompt is not proof that a workflow is reliable. Evaluate the complete setup—prompt, model, tools, data, and human review—using representative tasks before relying on it.

## 1. Define the intended use

Record the users, task types, impact of errors, allowed data, connected tools, and actions the workflow may take. Name an accountable owner and a human approval point for consequential outcomes.

## 2. Build a representative test set

Use realistic examples that cover:

- Common requests and ordinary inputs
- Missing, ambiguous, or conflicting evidence
- Boundary cases and unusual formats
- Refusal or approval conditions
- Errors from tools or connected systems

Remove or mask sensitive information unless its use is approved. Keep test cases separate from the prompt where feasible so changes can be compared.

## 3. Set observable criteria

Write checks before running the evaluation. Include task completion, factual grounding, instruction and format adherence, boundary handling, and handling of uncertainty. Define hard failures for unsafe or unauthorized actions. Use human review for judgment-heavy criteria.

## 4. Test consistently

Record the prompt and version, model identifier, product surface, tool access, settings, data fixture, date, and reviewer. Compare candidate changes with the same cases and configuration. Repeat cases when outputs vary. A score from one run is not a guarantee of future performance.

## 5. Review failures

For each failure, capture the input, expected behavior, actual behavior, severity, likely cause, and corrective action. Add useful failures to the regression set. Check that a fix improves the target behavior without breaking other cases.

## 6. Decide and monitor

Set acceptance thresholds that match the impact of errors. Release only after required checks pass and an accountable owner accepts residual risk. Monitor real use under approved data and access policies. Define a stop, rollback, and re-review path.

## Experiment record

```yaml
experiment_id:
date:
owner:
intended_use:
prompt_version:
model_identifier:
product_surface:
settings:
tools_and_permissions:
fixture_version:
case_count:
trial_count:
acceptance_criteria:
results:
hard_failures:
human_reviewer:
known_limits:
release_decision:
rollback_or_stop_rule:
```

## Release decision

- **PASS** — Every required criterion and hard gate passed.
- **CONDITIONAL PASS** — Only named, accepted limitations remain; owner and conditions are recorded.
- **REWORK** — Changes and another evaluation are required.
- **FAIL** — A hard gate failed or the intended use is not supported.

Do not describe a workflow as production-certified based only on this checklist. Production readiness depends on the specific model, configuration, organization, data, permissions, and operating environment. Review the [current official evaluation documentation](official-resources.md) before choosing evaluation tooling.