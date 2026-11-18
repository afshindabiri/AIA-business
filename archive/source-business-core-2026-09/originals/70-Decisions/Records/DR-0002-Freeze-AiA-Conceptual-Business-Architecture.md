---
type: decision
status: canonical
decision_id: DR-0002
decided_on: 2026-09-14
---

# Freeze the AiA Conceptual Business Architecture

## Purpose

This record owns the rationale and decision snapshot for freezing the conceptual AiA Business Architecture. It does not freeze mutable business configuration, create new filesystem structure, or replace the current architecture authority in [[KNOWLEDGE-GOVERNANCE]].

## Context

The owner considered an independent architecture review completed on 2026-09-14. Its verdict was `ARCHITECTURE_PASS_WITH_MINOR_NOTES`: no material architectural defects, structural redesign, Vault migration, or new folder architecture were required before proceeding.

## Decision

- Owner decision: `FREEZE_ARCHITECTURE` as of 2026-09-14.
- The freeze applies to the conceptual architecture boundaries and information-ownership model recorded in [[KNOWLEDGE-GOVERNANCE]].
- The frozen conceptual separation is Core; Capabilities; Solutions; Industries; Offers; How We Work; Clients / Projects; and Learning / Evidence → Business Decision.
- Freeze the architecture, not the business configuration inside it. Industries, Capabilities, Solutions, Offers, Pricing, ICP, Positioning, Market Wedge, Revenue Model, How We Work, GTM strategy, tools, and technologies remain mutable under their existing canonical owners.
- Reopen the conceptual architecture only when future real-world evidence exposes a material architectural defect, not for stylistic preference or taxonomy optimization.

## Supporting review evidence

- Review date: 2026-09-14
- Verdict: `ARCHITECTURE_PASS_WITH_MINOR_NOTES`
- Stress-test summary: 10 PASS, 4 RISK, 0 FAIL
- Three RISK items concerned future ownership of Solution ↔ Industry and Solution ↔ Capability relationships; one concerned future SaaS product-definition ownership.

The external review is supporting evidence only. The canonical truth is the owner's decision recorded in this Vault.

## Minor review guardrails

1. **Relationship ownership:** When Solution ↔ Capability or Solution ↔ Industry relationships are stored, one side owns each fact and the other references or derives it. No relationship map is created by this decision.
2. **Avoid duplicate mutable truth:** One canonical owner remains authoritative for a current rule; other notes may reference or summarize it without becoming competing owners. This decision does not initiate a Vault-wide cleanup.
3. **Contextual naming:** Ambiguous labels such as CRM should be contextualized when needed—for example, CRM implementation as a Capability, a specific CRM product as a Tool, and Lead Operations System as a Solution. No larger taxonomy system is created.
4. **SaaS / Managed Services later:** If AiA actually enters SaaS or Managed Services, product or solution definition, commercial Offer, operating method, technical implementation, and actual Client commitments must remain distinguishable. No Product or SaaS architecture is created now.

## Consequences

- No architecture redesign, Vault migration, folder restructuring, or speculative future structure is required by this decision.
- The architecture remains able to support additions, changes, retirements, multiplicity across its conceptual areas, and evolving delivery methodology.
- Mutable business configuration continues to change through its existing canonical owners and governance.
- Existing historical snapshot and no-cascade rules in [[KNOWLEDGE-GOVERNANCE]] remain authoritative; this decision does not rewrite historical Client or Project truth.
- The four minor review notes remain guardrails, not current structural projects.

Governance authority: [[KNOWLEDGE-GOVERNANCE]].
