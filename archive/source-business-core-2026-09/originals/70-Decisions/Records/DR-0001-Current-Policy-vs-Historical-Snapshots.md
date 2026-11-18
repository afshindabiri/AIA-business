---
type: decision
status: canonical
decision_id: DR-0001
decided_on: 2026-09-13
---

# Separate Current Policy from Historical Snapshots

## Purpose

This record owns the rationale for separating mutable current policy from immutable historical transaction facts. It does not own current pricing or any Client transaction.

## Context

Current policies must be able to change without altering what a Client was quoted, agreed to, paid, received, or accepted in an earlier transaction.

## Decision

- Current mutable policy has one canonical source and must be fresh-read at answer time.
- When a policy is applied to a real transaction, historically meaningful values are snapshotted in the relevant Client Phase.
- Later policy changes apply prospectively unless an explicit Decision Record states otherwise.
- Historical snapshots are corrected only when the recorded historical fact itself was wrong.

## Consequences

- Current questions route to the canonical policy, such as [[Pricing-Policy]].
- Historical questions route to the relevant Client Phase snapshot.
- Policy changes do not cascade into completed or active historical records.
- Material policy changes require a new Decision Record and the applicable policy version/effective-date update.

Governance authority: [[KNOWLEDGE-GOVERNANCE]].
