---
type: core
status: canonical
---

# Operating Principles

## Purpose

This file owns the principles used to make business and delivery decisions. It does not own a specific offer, tool choice, or Client decision.

1. Problem first, technology second.
2. Remove before automating.
3. Simplify before adding tooling.
4. Standardize before automating.
5. Prefer existing tools where they solve the problem well.
6. Integrate before custom-building when appropriate.
7. Use AI only where AI provides meaningful value.
8. Custom-build only when justified.
9. Use the minimum necessary complexity.
10. Keep Client-facing processes simple.
11. Require evidence before assumption.
12. Do not promote one Client-specific pattern into a universal rule without repeated evidence.
13. Avoid artificial vendor or Client lock-in.
14. The Client should own Client-specific operational assets where practical.
15. Third-party services should normally be Client-owned and direct-billed.
16. Do not create processes, fields, metrics, or forms without decision value.
17. Prefer the fastest correct operational path.

## AI recommendation and Owner decision authority

AI evaluates and recommends. The Owner makes the final business decision.

```text
AI Recommendation ≠ Final Decision
Owner Decision = Final Business Authority
```

AI may collect and inspect available evidence; evaluate a potential Client, Project, Opportunity, Solution, or other relevant business decision; identify strengths, weaknesses, risks, and missing information; and provide a reasoned recommendation with appropriate confidence. It may not autonomously accept or reject a Project, commit AiA commercially, close an Opportunity, change an approval-dependent business state, or override the Owner.

The lightweight decision flow is:

```text
Evidence
→ AI Evaluation
→ AI Recommendation
→ Owner Decision
→ Execution
→ Actual Outcome
→ Learning
```

### Evidence and no-guessing

Evaluation uses only relevant available evidence. Depending on the decision, evidence may include the operational problem and business impact; systemizability, feasibility, and economic justification; repetitive work, fragmented information, dependency on particular people, lost follow-ups, delays, poor visibility, errors, or duplication; knowledge-capture potential; risks; Client readiness; available data; and implementation constraints. Not every evaluation requires every criterion, and simple decisions must not acquire mandatory bureaucracy.

If material evidence is missing, use `NEEDS_MORE_INFORMATION`, identify the important gaps, and request or investigate relevant evidence where appropriate. Do not guess merely to force a yes/no recommendation.

### AI evaluation and recommendation

Evaluation describes what the evidence indicates; recommendation is the advisory conclusion. Use these recommendation states unless an established owning process defines an equivalent:

- `RECOMMEND_ACCEPT`
- `RECOMMEND_DECLINE`
- `NEEDS_MORE_INFORMATION`

Where practical and material, record the Recommendation, Confidence, Key Reasons, Main Risks, and Material Missing Information. Avoid false precision. Confidence never grants decision authority.

### Owner decision and override

The Owner may `ACCEPT`, `DECLINE`, or `DEFER`; follow or override the AI recommendation; or request more evidence or analysis. An AI recommendation must never automatically change a business state that requires Owner approval.

When the Owner decision differs from the AI recommendation, record `Override: YES`. An `Override Reason` may be recorded when useful for learning, but it is optional and its absence must not block the Owner's decision. Agreement between AI and Owner requires no override explanation.

### Historical traceability and learning

An AI recommendation belongs to the evidence and context available when it was made. Do not overwrite it because later evidence, criteria, decisions, or outcomes differ. A later reassessment must remain distinguishable under the existing current-versus-historical truth governance; do not create a competing history or versioning system.

Where useful, compare actual outcomes with the original evidence, AI recommendation, Owner decision, and optional override reasoning to improve future decision criteria. This does not create a learning platform, scoring engine, or Business Second Brain architecture.

### Customer / Project Fit application

Any current or future Customer / Project Fit evaluation is decision support, not decision authority. AI gathers relevant evidence, evaluates fit, and recommends; the Owner reviews and makes the final decision. No AI recommendation may autonomously accept, reject, or change the state of a potential Client or Project.

Operational application: [[Solution-Selection]] and [[Tool-Selection]].
