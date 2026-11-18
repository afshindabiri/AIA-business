---
type: decision
status: canonical
decision_id: DR-0003
decided_on: 2026-09-14
---

# AI Recommends; the Owner Decides

## Purpose

This record owns the rationale and decision snapshot for separating AI evaluation and recommendation from final business authority. It does not own current operating rules or a specific Client, Project, Opportunity, or transaction decision.

## Context

AiA may use AI to evaluate evidence, surface strengths, weaknesses, risks, and missing information, and recommend a course of action. Recommendation quality and confidence do not grant AI authority to accept or reject work, commit AiA, close an Opportunity, or change an approval-dependent business state.

## Decision

- AI evaluation describes what available evidence indicates.
- AI recommendation is advisory and may use `RECOMMEND_ACCEPT`, `RECOMMEND_DECLINE`, or `NEEDS_MORE_INFORMATION`.
- Insufficient material evidence must be identified rather than guessed around.
- The Owner makes the final business decision and may `ACCEPT`, `DECLINE`, `DEFER`, request more evidence, follow the AI recommendation, or override it.
- When the Owner differs from the recommendation, `Override: YES` records the difference. An explanation is optional and cannot constrain Owner authority.
- An AI recommendation must never automatically change a business state that requires Owner approval.
- The current authoritative rule and its Customer / Project Fit application are maintained in [[Operating-Principles#AI recommendation and Owner decision authority]].

## Consequences

- The decision flow is Evidence → AI Evaluation → AI Recommendation → Owner Decision → Execution → Actual Outcome → Learning.
- Earlier recommendations remain attributable to the evidence and context available at the time; later reassessments remain distinguishable through existing current-versus-historical truth governance.
- Actual outcomes may inform future criteria without creating an autonomous decision system, mandatory scoring model, competing history system, or Business Second Brain architecture.
- No new Offer, Solution, Product, folder structure, workflow engine, or automatic Project acceptance mechanism is created by this decision.

Governance authority: [[KNOWLEDGE-GOVERNANCE]]. Current rule: [[Operating-Principles#AI recommendation and Owner decision authority]].
