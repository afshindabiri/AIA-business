---
type: decision
status: canonical
decision_id: DR-0005
decided_on: 2026-09-14
---

# Clarify Project/Cycle Semantics and PARA Navigation

## Purpose

This record owns the rationale and decision snapshot for the Project/Cycle naming clarification and lightweight PARA navigation. It does not own current Client, Cycle, Phase, payment, archive, or dashboard facts.

## Context

An independent review returned `ARCHITECTURE_PASS_WITH_CHANGES` with the recommendation `IMPLEMENT_MINIMAL_MODEL`; the resulting work was classified as `CLARIFICATION_DECISION_REQUIRED`, not an architecture reopen. The frozen architecture already defines Cycle as one independent project or engagement for a Client, but user-facing Project terminology, PARA entry points, engagement boundaries, direct Client navigation, System Care, and status-based historical navigation required explicit clarification without creating a second entity or moving records.

## Decision

- Project is the user-facing and operating-interface name for the existing canonical Cycle entity. No separate Project entity, file, ID, status, folder, database, or schema exists.
- Existing `CYCLE.md`, Cycle IDs, `cycle_status`, metadata, links, and ownership remain authoritative.
- Root `Projects.md` is derived navigation that surfaces the existing [[Active-Work]] contract; it is not an operational ledger.
- Root `Archive.md` is a derived `STATUS_VIEW` for completed, lost, and cancelled engagement navigation plus access to the existing internal `90-Archive`; it owns no historical transaction facts and moves no records.
- The canonical engagement, scope-expansion, completion, and reopening boundaries are maintained in [[Customer-Lifecycle#Project / engagement boundary]].
- System Care's Project boundary is maintained in [[Post-Implementation-Operations#System Care Project boundary]].
- The Cycle template standardizes direct navigation to the authoritative parent `CLIENT.md` without duplicating current Client identity.
- `cycle_status: completed` does not imply that Phase-owned payment, delivery, acceptance, or other obligations are settled.
- No canonical `current_phase` field is introduced.
- The architecture freeze in [[DR-0002-Freeze-AiA-Conceptual-Business-Architecture]] remains in force; this is clarification and implementation only.

## Consequences

- One Client may retain many independent Projects/Cycles, each with its own lifecycle, while the Client relationship persists.
- Projects and Archive provide PARA-compatible navigation without replacing authoritative Client/Cycle/Phase records.
- Completed Client engagements remain under `50-Clients/`; they do not become superseded internal documents or move into `90-Archive`.
- Active work excludes closed and Mock records; payment obligations remain visible from owning Phases even when a Project is completed.
- No Client/Project migration, record rename, physical move, new status, speculative template, knowledge subsystem, or architecture redesign is introduced.

Governance authority: [[KNOWLEDGE-GOVERNANCE]]. Shared terminology: [[GLOSSARY]].
