# GPT-5.6 Sol High - Purple Team Operational Templates

Revision 2 | Compiled July 28, 2026

Fill these records with verified organizational facts. A completed template is evidence of planning; it is not authorization unless signed through the organization's approval process.

## T-01 - Purple Team Program Charter

```text
Sponsor / risk owner:
Program lead:
Business outcomes:
Critical services:
Scope and non-goals:
Decision rights:
Exercise intake and cadence:
Evidence retention:
Metrics:
Annual review / expiry:
```

## T-02 - Authorization and Rules of Engagement

```text
Authorizing owner:
Authority basis / signed record:
Operators:
Dates and time zone:
Authorized target identifiers:
Environment:
Permitted actions:
Prohibited actions:
Rate / resource limits:
Data handling:
Safety observer:
Stop conditions:
Emergency contacts:
Rollback owner:
External communication approval:
Completion and expiry:
```

## T-03 - Target Manifest

```text
Asset ID:
Owner:
Exact hostname / account / tenant / repo / namespace:
Environment:
Approved test identities:
Dependencies:
Mixed-tenant or third-party exposure:
Allowed dates:
Evidence classification:
Status: IN / OUT / UNRESOLVED
```

## T-04 - Safety and Risk Assessment

```text
Hazard / failure mode:
Likelihood:
Impact:
Affected service / data / people:
Preventive control:
Health indicator:
Stop threshold:
Rollback:
Owner:
Residual risk:
Approval:
```

## T-05 - Lab and Telemetry Readiness

```text
Isolation verified:
Synthetic identities and data:
Snapshots / reset tested:
Egress controls:
Sensors and log routes:
Time synchronization:
Expected event fields:
Preflight query:
Observer access:
Go / Conditional / No-go:
Approver:
```

## T-06 - Atomic Test Run Card

```text
Run ID / version:
Control objective:
ATT&CK mapping and version:
Approved target:
Prerequisites:
Operator action reference:
Expected prevention:
Expected telemetry:
Expected analytic / alert:
Evidence capture:
Cleanup:
Stop condition:
Approvals:
```

## T-07 - Deconfliction, Stop, and Deviation Log

```text
Timestamp and time source:
Run ID:
Signal / deviation:
Reporter:
Scope impact:
Decision: CONTINUE / PAUSE / STOP:
Decision authority:
Actions taken:
Evidence preserved:
Notifications:
Restart approval:
```

## T-08 - Evidence Ledger

```text
Evidence ID:
Run ID:
Timestamp:
Source system:
Collector:
Artifact locator / hash:
Description:
Classification:
Handling / redaction:
Fact / assumption / inference:
Confidence:
Related finding:
Retention / deletion date:
```

## T-09 - Detection Validation Record

```text
Analytic ID / version:
Hypothesis:
Required telemetry:
Positive tests:
Negative tests:
Boundary tests:
False-positive sample:
Observed latency:
Blind spots:
Result:
Tuning:
Owner:
Retest date:
```

## T-10 - Layered Coverage Matrix

```text
Threat behavior:
Business relevance:
Prevention:
Telemetry:
Analytic:
Alert:
Triage:
Response:
Recovery:
Evidence quality:
Last tested:
Confidence:
Gap owner:
```

## T-11 - Remediation and Retest

```text
Finding ID:
Root cause:
Business risk:
Corrective action:
Compensating control:
Owner / due date:
Change and rollback:
Positive / negative / regression tests:
Observability check:
Residual risk:
Retest evidence:
Closure approver:
```

## T-12 - After-Action and CAPA

```text
Exercise / date:
Objectives:
What occurred:
Expected vs. observed:
What worked:
Gaps and contributing conditions:
Safety deviations:
Corrective actions:
Preventive actions:
Owners / dates:
Validation:
Escalation:
Next exercise input:
```
