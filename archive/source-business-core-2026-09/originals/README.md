---
type: router
status: canonical
---

# AiA Business Core — AI Router

## Purpose

This file is the AI entry point. It owns retrieval routing and does not own detailed business facts, client state, research, or history.

> [!IMPORTANT] Mutable Data Fresh-Read Rule
> Never answer mutable business facts from memory. Fresh-read the canonical Obsidian source before answering.
>
> Memory may route retrieval; it may not replace retrieval. If the canonical source cannot be accessed, do not guess or reuse an old cached value; explicitly mark the current value as unverified.

## Truth model

```text
CURRENT / MUTABLE TRUTH
→ reference canonical source
→ fresh-read canonical source when answering

HISTORICAL / TRANSACTIONAL TRUTH
→ store snapshot
→ read snapshot when answering historical questions
```

Reference current truth. Snapshot historical truth. Fresh-read mutable truth. Never guess unavailable truth.

Full rules: [[KNOWLEDGE-GOVERNANCE]]. Human navigation: [[HOME]]. System/document state map: [[CURRENT-STATE]]. Customer lifecycle: [[Customer-Lifecycle]].

## Retrieval sequence

1. Read this README.
2. Classify the question.
3. Locate the authoritative source.
4. Fresh-read mutable data.
5. Open only the minimum required linked files.
6. Stop once sufficient evidence is available.
7. Use Client snapshots for historical transactional questions.
8. Use Decision Records when the question is “why did this change?”
9. Read Research only for unresolved or research questions.
10. Read Archive only when historical or superseded material is explicitly needed.

## Retrieval priority

1. README
2. Relevant canonical source
3. Relevant Client → Cycle → Phase
4. Decision Record when change history is needed
5. Assets when proof or an example is needed
6. Research when unresolved knowledge is needed
7. Archive only when explicitly required

## Routing map

| Question | Authoritative route |
|---|---|
| What is AiA? | [[Business-Definition]] |
| Current positioning? | [[Positioning]] |
| Current pricing? | [[Pricing-Policy]] |
| What can clients buy? | [[Offer-Architecture]] |
| How is Audit performed? | [[Paid-Audit]] |
| How do we choose a solution? | [[Solution-Selection]] |
| How do we select tools? | [[Tool-Selection]] |
| Client status? | [[CLIENT-INDEX]] → Client → Cycle |
| Historical client quote or payment? | Relevant Client Phase snapshot |
| Why did a policy change? | [[DECISION-LOG]] → relevant Decision Record |
| Unresolved research? | [[Research-Index]] |
| Superseded methodology? | `90-Archive/` only when explicitly needed |

## Retrieval boundaries

- Do not treat Views, Research, Archive, prior chat context, or cached summaries as current truth.
- Do not scan the entire vault for routine questions when the route above is sufficient.
- For technical implementation detail, follow the linked technical project workspace; Business Core does not own engineering execution.
