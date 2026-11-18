---
type: governance
status: canonical
---

# Knowledge Governance

## Purpose

This file is the authoritative source for Business Core architecture, retrieval, ownership, and knowledge-governance rules. It does not own business policies, client transactions, or research conclusions.

## Conceptual architecture freeze

As of 2026-09-14, the owner-approved conceptual AiA Business Architecture boundaries and information-ownership model are frozen. The frozen conceptual separation is:

- Core
- Capabilities
- Solutions
- Industries
- Offers
- How We Work
- Clients / Projects
- Learning / Evidence → Business Decision

The separation preserves these boundaries:

- Industry ≠ Solution
- Solution ≠ Capability
- Capability ≠ Offer
- Offer ≠ How We Work
- Current Strategy ≠ Historical Client Truth
- Business Foundation ≠ Current Market Wedge
- Website, social, and other channel outputs ≠ authoritative business truth

Freeze the architecture, not the business configuration inside it. Industries, Capabilities, Solutions, Offers, Pricing, ICP, Positioning, Market Wedge, Revenue Model, How We Work, GTM strategy, tools, and technologies remain mutable under their existing canonical ownership and governance.

The architecture must continue to support addition, change, retirement, multiple Industries, multiple Capabilities, multiple Solutions, multiple Offers, evolving delivery methodology, and preservation of historical Client and Project truth. Reopen the conceptual architecture only if future real-world evidence exposes a material architectural defect—not for stylistic preference or taxonomy optimization.

Decision rationale and review provenance: [[DR-0002-Freeze-AiA-Conceptual-Business-Architecture]].

## Four truth layers

1. **Current canonical truth** defines what is true now. Each fact has one authoritative source.
2. **Historical snapshots** preserve what was quoted, agreed, paid, delivered, accepted, or otherwise true for a transaction or event.
3. **Derived views** surface information owned elsewhere and are never sources of truth.
4. **Research and historical documentation** are non-canonical and must never silently become current truth.

```text
CURRENT / MUTABLE TRUTH
→ reference canonical source
→ fresh-read canonical source when answering

HISTORICAL / TRANSACTIONAL TRUTH
→ store snapshot
→ read snapshot when answering historical questions
```

Reference current truth. Snapshot historical truth. Fresh-read mutable truth. Never guess unavailable truth.

## Mutable Data Fresh-Read Rule

Whenever an AI answers a question involving information that can change over time, it MUST read the current canonical Obsidian source at answer time.

It MUST NOT answer mutable facts from model memory, previous conversations, cached context, previous summaries, previously retrieved values, or assumptions. Previous knowledge may be used only to locate the correct source; it must not be treated as authoritative.

Mutable data includes current pricing, offers, policy, client/cycle/phase status, payment status, outstanding payment, delivery status, meeting date/time, next action, current owner, active GTM decisions, market wedge, pipeline state, and any field explicitly designated mutable.

> Never answer mutable business facts from memory. Fresh-read the canonical Obsidian source before answering.

Memory may route retrieval; it may not replace retrieval. If the canonical source cannot be accessed, do not guess or use an old cached value; explicitly mark the current value as unverified.

## Source-of-truth map

| Concept | Authoritative source |
|---|---|
| Business Definition | [[Business-Definition]] |
| Positioning | [[Positioning]] |
| Current Pricing | [[Pricing-Policy]] |
| Current Offer Structure | [[Offer-Architecture]] |
| Audit Methodology | [[Paid-Audit]] |
| Customer / Project Fit Model | [[Assessment#Customer / Project Fit model]] |
| Solution Selection | [[Solution-Selection]] |
| Tool Selection | [[Tool-Selection]] |
| AI Recommendation / Final Business Decision Authority | [[Operating-Principles#AI recommendation and Owner decision authority]] |
| Sales Stage Definitions | [[Pipeline-Definition]] |
| Client Identity | `CLIENT.md` in the relevant Client folder |
| Project Objective / Next Action | `CYCLE.md` in the relevant Cycle folder |
| Discovery Events | `P00-Discovery.md` in the relevant Cycle folder |
| Audit Quote / Payment / Delivery | `P01-Audit.md` in the relevant Cycle folder |
| Implementation Quote / Payment / Delivery | `P02-Implementation.md` in the relevant Cycle folder |
| Reason a policy changed | Relevant Decision Record in `70-Decisions/Records/` |
| Views | Derived only |
| Research | Non-canonical |

## Retrieval policy

Start at [[README]], classify the question, locate the authoritative source, fresh-read mutable data, and open only the minimum linked files required. Use Client snapshots for historical transaction questions, Decision Records for reasons behind changes, Research only for unresolved questions, and Archive only when superseded history is explicitly needed.

## Source-of-truth and no-cascade rules

- Reference current truth with links; do not duplicate it.
- A pricing change edits [[Pricing-Policy]] plus a Decision Record—not every Offer or GTM note.
- An Audit methodology change edits [[Paid-Audit]]—not historical Client phases.
- A sales-funnel change edits [[Sales-Funnel]]—not completed historical Cycles.
- A Client payment change edits the relevant Client Phase only—not indexes, views, or unrelated files.

## Snapshot and policy applicability rules

- When a current policy becomes a real transaction, snapshot only historically meaningful fields such as quoted/agreed amount, pricing policy version, quote date, agreed scope, offer version, payment, delivery, and acceptance.
- Do not copy an entire policy into a Client record.
- A new policy applies prospectively from `effective_from` unless a Decision Record explicitly says otherwise.
- A policy change never retroactively rewrites historical snapshots.
- Important transactional or commercial policies—such as pricing, material offer terms, and major commercial rules—use explicit versions. Do not version every note.
- For such a policy change: create a Decision Record, update the current policy, increment its version, update its effective date, and leave historical snapshots unchanged.

## Corrections

Policy Change ≠ Historical Data Correction.

A snapshot may be corrected only when the recorded historical fact was wrong. A material correction records the corrected value, correction date, and reason; it must not be disguised as a policy update.

## Client data ownership

- **Client:** owns identity, contacts, relationship context/source/status, and links to Cycles. It does not duplicate live phase or Cycle status.
- **Cycle:** owns objective, Cycle status, owner, exactly one high-level Next Action, Phase links, key decisions, and final outcome.
- **Phase:** owns transactional state, including commercial, payment, delivery, meeting, and acceptance facts relevant to that Phase.
- When continuity of the same Client entity is confirmed, retain its stable Client ID and update current identity, contacts, or relationship context only in its `CLIENT.md`. Do not infer continuity from similar names alone.
- When a transaction-time Client name or contact role is materially relevant to what was agreed or delivered, preserve it in the applicable historical Project/Phase snapshot. Later current-identity changes must not retroactively rewrite that history; do not add speculative historical fields without a real need.
- Completed Clients and Cycles remain in `50-Clients/`; they are business knowledge, not Archive material.
- Detailed engineering work belongs in a separate technical project workspace and may be linked from Business Core.

## Status vocabularies

- Document lifecycle: `canonical`, `draft`, `candidate`, `superseded`
- Cycle: `lead`, `active`, `on_hold`, `completed`, `lost`, `cancelled`
- Commercial: `not_offered`, `offered`, `won`, `lost`
- Payment: `not_required`, `pending`, `partial`, `paid`, `refunded`
- Delivery: `not_started`, `in_progress`, `delivered`, `accepted`, `cancelled`
- Discovery meeting: `scheduled`, `completed`, `cancelled`, `no_show`

Do not add synonyms without an operational need and an approved governance change.

## Naming, IDs, and metadata

- Client ID: `CL-0001`
- Cycle ID: `CL-0001-C01`
- Phase ID: `CL-0001-C01-P01`
- Example folder pattern: `CL-0001-Client-Name/C01-Project-Name/`
- Names may change; IDs do not.
- Metadata stays minimal and must have an operational or retrieval purpose.
- Canonical notes use `type` and `status`. Policies additionally use `policy_id`, `policy_version`, and `effective_from` when historical applicability matters.

## Linking

- Prefer Obsidian links to repeated prose or values.
- Use transclusion only when a live canonical section genuinely needs to be visible elsewhere.
- Avoid circular duplicated summaries.
- Routine AI answers should normally require [[README]] plus one authoritative note, or for Client questions, [[README]] → [[CLIENT-INDEX]] → one relevant Client/Cycle/Phase path.

## Decisions, research, and archive

- Material changes to pricing, ICP, market wedge, core offer/process, ownership, or architecture require a Decision Record and an entry in [[DECISION-LOG]].
- Promotion path: Client Finding → Repeated Pattern → Research / Validation → Decision → Canonical Core / Playbook.
- One Client finding must never become a universal rule automatically.
- Research is non-canonical until an explicit Decision promotes it.
- Archive is for superseded methodologies, old pricing models, previous architecture versions, and historical internal documents—not Client history.

## Raw data and sensitive information

- Business Core stores extracted business knowledge, summaries, findings, evidence references, and appropriate links—not database dumps, large CRM exports, recordings, raw conversation archives, confidential spreadsheets, or large generated datasets.
- Never store passwords, API keys, private keys, recovery codes, payment-card data, or authentication secrets here. Reference a secure storage location only when appropriate and safe.

## Technical project separation

Business Core answers who, what project, what business problem, stage, commercial/payment state, result, and next action. A linked technical workspace owns architecture, code, engineering tasks, tests, deployment, and technical artifacts.
