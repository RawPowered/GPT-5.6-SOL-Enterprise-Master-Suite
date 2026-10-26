# Prompt templates

Adapt these templates to the actual task. Replace bracketed text, remove irrelevant instructions, and keep approval boundaries clear.

## Compact task brief

```text
Role: Act as [role responsible for this work].

Goal: Produce [observable result] for [audience].

Evidence: Use [approved inputs]. Treat [source] as authoritative.
Separate confirmed facts, assumptions, and unknowns.

Scope and constraints: [in scope, out of scope, requirements].
Do not [prohibited actions]. Ask before [approval-gated actions].

Acceptance: The result is complete when [measurable checks].

Output: Return [format, sections, length].
Verify the result against the evidence and acceptance criteria.
Report material uncertainty and unverified items.
```

## Higher-assurance task brief

```text
ACCOUNTABILITY
Responsible role: [role]. Audience: [audience].
Decision authority: [recommend / draft / edit local artifact / test].
Excluded authority: [production approval / legal sign-off / external communication].

OBJECTIVE
[Observable result, intended use, and consequence of error.]

AUTHORIZED EVIDENCE
Sources: [files, systems, official references].
Authority order: [which source wins if sources conflict].
Freshness requirement: [date or rule].
Known gaps: [missing or disputed evidence].

SCOPE AND APPROVALS
In scope: [assets and actions].
Out of scope: [exclusions].
Allowed without further approval: [safe actions].
Approval required for: [external, destructive, costly, or consequential actions].

METHOD
Address: [required questions].
Map material conclusions to evidence. Label inference and assumptions.
Identify conflicts rather than resolving them without a stated rule.

VALIDATION
Check: [tests, calculations, citations, review, or render].
Pass criteria: [thresholds].
State failures, exceptions, and areas not tested.

RETURN
[Decision or artifact, evidence map, prioritized findings, next steps,
residual risks, and unresolved decisions.]

COMPLETION
Use PASS, CONDITIONAL PASS, REWORK, or FAIL only as defined above.
Do not claim a check passed unless it was actually performed.
```

## Approval boundary

For read, explain, review, or plan requests, inspect and report. For explicitly requested local edits, make the scoped change and verify it. Seek approval before external writes, destructive changes, purchases, or material scope expansion. Adapt this rule to the organization's policies and the permissions of the connected system.

## Evidence labels

When accuracy matters, label important statements as one of:

- **Provided fact** — present in user-supplied or authorized material
- **Verified source** — checked against a current authoritative source
- **Test result** — produced by a named check that was actually run
- **Inference** — reasoned from evidence but not directly stated
- **Assumption** — used because evidence is incomplete
- **Unknown** — not established from available information