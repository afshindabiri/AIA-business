---
type: client-phase
status: canonical
phase_type: implementation
client_id: "<client_id>"
cycle_id: "<cycle_id>"
phase_id: "<cycle_id>-P02"
commercial_status: "<not_offered|offered|won|lost>"
quoted_amount_aed: "<quoted_amount>"
agreed_amount_aed: "<agreed_amount>"
offer_version: "<commercial_offer_version_if_applicable>"
quoted_at: "<YYYY-MM-DD>"
payment_status: "<not_required|pending|partial|paid|refunded>"
paid_amount_aed: "<paid_amount>"
paid_at: "<YYYY-MM-DD>"
delivery_status: "<not_started|in_progress|delivered|accepted|cancelled>"
delivered_at: "<YYYY-MM-DD>"
accepted_at: "<YYYY-MM-DD>"
---

# Implementation Phase Template

## Purpose

Copy this file as `P02-Implementation.md` inside a Client Cycle. The resulting Phase owns the implementation transaction and delivery snapshot; detailed engineering execution belongs in a linked technical workspace.

# Implementation

## Agreed scope snapshot

<scope and milestones agreed for this transaction>

## Delivery gates

- READY TO BUILD:
- READY TO TEST:
- READY TO RELEASE / PILOT:
- READY FOR PRODUCTION:
- READY FOR ACCEPTANCE:
- READY FOR HANDOVER:

## Pilot

- Required: `<yes|no>`
- Outcome: `<SCALE|IMPROVE|PREPARE FIRST|STOP>` (leave blank when no Pilot is used)

## Technical project workspace

- <link>

## Handover and result

- Ownership transferred:
- Known limitations:
- Final result:

## Material corrections

- Corrected value:
- Correction date:
- Reason:

Methods: [[Implementation-Delivery]], [[Pilot]], and [[Acceptance-and-Handover]]. Never replace this historical snapshot when current policy changes.
