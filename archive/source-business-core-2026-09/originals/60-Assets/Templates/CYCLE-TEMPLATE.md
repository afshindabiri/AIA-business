---
type: client-cycle
status: canonical
client_id: "<client_id>"
cycle_id: "<cycle_id>"
cycle_status: "<lead|active|on_hold|completed|lost|cancelled>"
owner: "<current_owner>"
next_action: "<exactly one high-level next action>"
---

# Cycle Template

## Purpose

Copy this file to `50-Clients/CL-0001-Client-Name/C01-Project-Name/CYCLE.md`. The resulting record is the authoritative Cycle and user-facing Project record for one engagement. It owns the objective, high-level state, owner, and exactly one Next Action; technical task management belongs elsewhere.

# <Project Name>

## Client

When instantiating this template, add a direct Obsidian link to the authoritative parent Client record using this pattern without code formatting: `Client: [[../CLIENT]]`.

The link is navigation only. Keep the stable `client_id` in frontmatter, and do not copy mutable Client identity or relationship fields into the Project.

## Objective

<one clear business objective>

## Phases

- Discovery: `<link to P00-Discovery.md when created>`
- Audit: `<link to P01-Audit.md when created>`
- Implementation: `<link to P02-Implementation.md when created>`

Create only the Phases that apply. Fresh-read the Phase that owns transactional state.

## Key decisions

- <decision or link>

## Technical project workspace

- <link when applicable>

## Final outcome

<complete only when the Cycle reaches an outcome>
