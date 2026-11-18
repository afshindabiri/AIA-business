---
type: core
status: canonical
---

# Customer Lifecycle

## Purpose

This file owns the current end-to-end customer lifecycle. It does not own pricing, detailed Phase methods, or an individual Client's state.

```text
Lead
→ Optional Assessment / Direct Conversation
→ Discovery
→ Focused Audit
→ Recommendation
→ Implementation
→ Optional Pilot
→ Production
→ Stabilization
→ Acceptance
→ Handover
→ Client Takeover / System Care / Continuous Improvement
```

- Assessment is optional.
- Discovery is lean.
- Audit is focused.
- Implementation is custom scoped and follows a validated recommendation.
- Pilot is conditional.
- Stabilization belongs to delivery.
- Acceptance is explicit.
- Handover is explicit.
- Post-implementation services are optional.

## Project / engagement boundary

Project is the user-facing name for the existing Cycle entity defined in [[GLOSSARY]]. One Client may have many independent Projects/Cycles, each with its own `cycle_status`, objective, owner, Next Action, Phases, decisions, and outcome. Completing one Project does not close a sibling Project, close the Client relationship, rewrite another Project, or move the Client.

Keep work in the same Project while it advances the same business objective within one continuing engagement. Discovery, Audit, Recommendation, Implementation, Pilot, and Handover remain one Project when they advance that objective; a new Phase, invoice, separately paid Audit, Pilot, or routine scope clarification does not by itself create a new Project.

Create a new Project/Cycle when:

1. the business objective materially changes;
2. the work needs an independent overall lifecycle or obligation boundary; or
3. new work is commissioned after the earlier engagement genuinely closed.

### Scope expansion

Keep an expansion in the same Project when the underlying objective and overall engagement boundary remain unchanged. Preserve the original agreement and record the dated amendment and updated commitment in the appropriate owning Phase; do not silently overwrite historical scope.

Create a new Project when the expansion represents a materially different objective or independently manageable engagement.

### Reopening

The same Project may resume when the same unfinished or previously paused commitment continues and the original Project boundary still accurately describes the work. Preserve the earlier closure or on-hold context in a historically traceable way.

Create a new Project for newly commissioned work after genuine closure, especially when it has a new objective or independent lifecycle. Do not reopen an old Project merely to avoid creating a new one.

### Completion semantics

`cycle_status: completed` is only the high-level Project state. It does not automatically mean all invoices are paid, all financial obligations are settled, every Phase status is closed, or the Client relationship ended. Phase-owned delivery, acceptance, payment, and other obligations remain independently authoritative.

System Care boundaries are owned by [[Post-Implementation-Operations#System Care Project boundary]].

Current commercial terms: [[Pricing-Policy]]. Operating methods: [[Assessment]], [[Discovery]], [[Paid-Audit]], [[Implementation-Delivery]], [[Pilot]], and [[Acceptance-and-Handover]].
