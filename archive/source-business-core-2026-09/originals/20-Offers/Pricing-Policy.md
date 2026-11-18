---
type: policy
status: canonical
policy_id: pricing
policy_version: 1
effective_from: 2026-09-13
---

# Pricing Policy

## Purpose

This file is the only authoritative source for current public and commercial pricing. It does not own historical Client quotes, agreed amounts, payments, or Client-specific scope.

## Current pricing

| Item | Current policy |
|---|---|
| Initial Assessment | Free |
| Discovery / Automation Opportunity Call | Free |
| Focused Business Automation & AI Audit | AED 990 |
| Implementation | Custom Quote |
| Third-Party Tools / Services | Separate; preferably paid directly by the Client |
| Post-Implementation | Scoped individually |

## Implementation commercial structure

Where practical, implementation proposals use fixed-scope, fixed-price milestones. Project-specific scope and delivery design remain in [[Implementation-Offer]].

## Transaction snapshot rule

When this policy is applied to a transaction, record the relevant quote, agreement, policy version, and dates in the appropriate Client Phase. That snapshot—not this live policy—answers historical transaction questions.

## Price-change behavior

When the current Focused Audit price changes:

- this policy records the new current price;
- future applicable transactions use the new policy;
- historical Clients retain the price recorded in their transaction snapshots;
- historical records are never recalculated from current policy.

For a material change, create a Decision Record, increment `policy_version`, update `effective_from`, and leave Client snapshots unchanged. A new policy applies prospectively unless its Decision Record explicitly states otherwise. See [[KNOWLEDGE-GOVERNANCE]].
