# GPT-5.6 Sol High - Combined Phase 3-4 Purple Team Release Record

Revision 2 | July 28, 2026

## Combined outcome

Phase 3 supplies the stable `PT-01` through `PT-24` operator prompts and `T-01` through `T-12` evidence templates. Phase 4 supplies the corrected base mappings, static audit, portable evaluation dataset, and `PT-EVAL-01` through `PT-EVAL-12` boundary cases.

The phases are combined at the release gate, not by mixing execution authority with evaluation. A prompt defines the authorized work contract; a template preserves evidence; an evaluation tests behavior; an accountable human makes the operational or risk decision.

## Crosswalk

| Prompt | Primary purpose | Evidence template | Lifecycle gate | Direct eval |
|---|---|---|---|---|
| PT-01 | Program governance | T-01 | G0-G1 | - |
| PT-02 | Authorization and ROE | T-02 | G1 | PT-EVAL-01 |
| PT-03 | Target and data boundaries | T-03 | G1 | PT-EVAL-02 |
| PT-04 | Safety and deconfliction | T-04, T-07 | G2 | PT-EVAL-05 |
| PT-05 | Threat objectives | T-10 | G0-G2 | - |
| PT-06 | ATT&CK hypothesis | T-10 | G2 | - |
| PT-07 | Scenario design | T-06 | G2 | PT-EVAL-10 |
| PT-08 | Technique-to-telemetry | T-05, T-10 | G2 | PT-EVAL-04 |
| PT-09 | Lab readiness | T-05 | G2 | - |
| PT-10 | Atomic run card | T-06 | G3 | PT-EVAL-09 |
| PT-11 | Tool/operator approval | T-04, T-06 | G2-G3 | PT-EVAL-03 |
| PT-12 | Stop and rollback | T-07 | G2-G3 | PT-EVAL-05 |
| PT-13 | Telemetry readiness | T-05 | G2 | PT-EVAL-04 |
| PT-14 | Detection validation | T-09 | G4 | PT-EVAL-07 |
| PT-15 | Triage and response observation | T-07, T-08 | G4 | - |
| PT-16 | Prevention and resilience | T-10 | G4 | - |
| PT-17 | Exercise orchestration | T-06, T-07 | G3 | PT-EVAL-08 |
| PT-18 | Evidence and findings | T-08 | G4 | PT-EVAL-06 |
| PT-19 | Remediation and retest | T-11 | G5 | PT-EVAL-11 |
| PT-20 | After-action and CAPA | T-12 | G5 | - |
| PT-21 | Coverage confidence | T-10 | G4-G6 | - |
| PT-22 | Program metrics | T-10, T-12 | G6 | - |
| PT-23 | Independent assurance | T-11, T-12 | G6 | - |
| PT-24 | Curriculum and competency | T-12 | G6 | PT-EVAL-12 |

## Phase 3 acceptance

- Prompts 01-80 remain unchanged and retain their identifiers.
- Purple-team prompts use the separate `PT-*` namespace.
- Every card includes authorization, model boundary, output, validation, and token-control clauses.
- Active or production-connected work remains human-gated.
- Prohibited activity routes to safe substitutes, not operational instructions.

## Phase 4 acceptance

- CYBER-07 maps to Prompt 68.
- CYBER-08 maps to Prompt 71.
- CYBER-10 maps to Prompt 67.
- The master index and static audit contain 104 unique prompt identifiers.
- The evaluation dataset contains 44 unique cases: 32 base cases and 12 purple-team cases.
- Runtime certification remains pending until named configurations are executed and scored.

## Integrated release rule

Release only when:

1. Authority, target, operator, environment, data, safety, and stop boundaries are complete.
2. The prompt, evidence template, lifecycle gate, and applicable eval case agree.
3. No claim relies only on a tool label, ATT&CK cell, screenshot, or one passing example.
4. Active execution and production changes remain under accountable human control.
5. Evidence distinguishes verified facts, assumptions, inferences, and unresolved questions.
6. The accountable human returns PASS, CONDITIONAL PASS, REWORK, STOP, or FAIL.

## Deferred organization-specific decisions

Legal authority, privacy and labor review, production permissions, approved tools and operators, evidence retention, competency thresholds, risk acceptance, and external communications remain enterprise decisions.
