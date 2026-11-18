---
type: client-phase
status: canonical
phase_type: audit
client_id: "<client_id>"
cycle_id: "<cycle_id>"
phase_id: "<cycle_id>-P01"
commercial_status: "<not_offered|offered|won|lost>"
quoted_amount_aed: "<quoted_amount>"
agreed_amount_aed: "<agreed_amount>"
pricing_policy_version: "<version_at_transaction>"
quoted_at: "<YYYY-MM-DD>"
payment_status: "<not_required|pending|partial|paid|refunded>"
paid_amount_aed: "<paid_amount>"
paid_at: "<YYYY-MM-DD>"
delivery_status: "<not_started|in_progress|delivered|accepted|cancelled>"
delivered_at: "<YYYY-MM-DD>"
accepted_at: "<YYYY-MM-DD>"
---

# Audit Phase Template

## Purpose

Copy this file as `P01-Audit.md` inside a Client Cycle. The resulting Phase owns the Audit's historical commercial, payment, delivery, and acceptance snapshot; it does not derive those facts from current policy after the transaction.

# Focused Audit

## Agreed scope snapshot

<scope agreed for this transaction>

## Audit work

- Scope:
- Understand:
- Evidence:
- Problem:
- Opportunity:
- Solution Options:
- Priority:
- Recommendation:
- Outcome: `<DO NOW|PREPARE FIRST|LATER|DON'T DO>`

## Material corrections

- Corrected value:
- Correction date:
- Reason:

Method: [[Paid-Audit]]. Current policy reference: [[Pricing-Policy]]. Never replace this historical snapshot when current policy changes.
