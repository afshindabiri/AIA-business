---
type: process
status: canonical
---

# Assessment

## Purpose

This file owns the optional initial Assessment method and the canonical Customer / Project Fit model. It does not own Discovery, Audit, current pricing, Client state, or final business decision authority.

Assessment is optional. It is a lightweight qualification and initial problem-orientation step that reduces friction before a conversation and helps determine whether deeper discussion is worthwhile.

Capture only enough to establish:

- the apparent problem or opportunity;
- basic business relevance;
- who should join the next conversation;
- the next step.

Do not turn Assessment into a mandatory gate, a large framework, or a substitute for [[Discovery]].

Assessment is not the mandatory pre-consultation intake flow owned by [[Consultation-Intake]]. That flow does not make Assessment mandatory.

## Customer / Project Fit model

Use this model when a meaningful Fit decision is needed for a potential Client, Project, or Opportunity. It is structured decision support, not an automatic qualification or acceptance system, and it remains optional for simple decisions.

The primary question is:

> Does this Client / Project represent a meaningful business problem that AiA can improve responsibly and economically through better processes, systems, automation, integration, software, AI, or a suitable combination of them?

Industry, company size, employee count, current technology, or a stated desire for AI does not determine Fit by itself. Industry is context, not the definition of Fit; the model must work across industries.

`Client Fit ≠ Project Fit`

A strong Client may propose a poor Project. A potentially valuable Project may exist with a Client who is not sufficiently ready for delivery. Evaluate both the opportunity and the Client's readiness without creating separate complex systems.

### Dimension classifications

Classify each core dimension from available evidence:

- `STRONG`
- `MODERATE`
- `WEAK`
- `UNKNOWN`

These are practical evidence classifications, not numeric scores. Do not calculate an overall average or use false precision; a material weakness in one dimension may outweigh strength elsewhere.

### 1. Problem & Business Impact Fit

Ask whether a real operational or business problem is worth solving. Relevant effects may include wasted time or cost, lost revenue or Leads, poor follow-up, delays, errors, duplicated work, poor customer experience, fragmented information, dependence on particular people, weak visibility or control, operational risk, difficulty finding correct information, or loss of business knowledge.

A request for AI based only on novelty or status is not evidence of a meaningful problem. Start from the business problem, not a preferred technology.

### 2. Solution / Systemizability Fit

Ask whether the problem can reasonably be improved through process improvement, standardization, systems, automation, integration, software, AI, or another capability available or responsibly deliverable by AiA.

Valid conclusions include simplifying or standardizing first, using an existing tool, integrating systems, automating, using AI, custom-building when justified, or declining to implement a technical solution. Apply [[Solution-Selection]]. Do not force an AiA implementation when the underlying issue is principally market demand, product-market fit, unresolved conflict, inappropriate pricing, hiring, or another problem automation would not materially solve.

### 3. Client Readiness Fit

Ask whether the Client is ready and willing to participate in successful delivery. Relevant evidence may include access to the decision maker; willingness to explain the process and provide necessary information, system or data access; responsible stakeholder availability; timely decisions, feedback, and approvals; realistic expectations; process-change adoption; and staff cooperation where relevant.

Readiness is not company size. A one-person company may be highly ready, while a large company may be poorly ready.

### 4. Delivery Feasibility Fit

Ask whether AiA can responsibly and realistically deliver the required outcome. Consider technical feasibility, data availability and quality, APIs and integrations, third-party dependencies, security, privacy, legal or regulatory constraints, required access, complexity, timeline, AiA capability, responsibly obtainable capability, and operational dependencies where material.

A requirement outside AiA's current standard Capabilities is not an automatic rejection. Determine whether AiA can responsibly deliver or source the required capability for the Project. One-off work must not automatically become an official AiA Capability.

### 5. Commercial / Economic Fit

Ask whether expected business value is reasonably justified relative to cost, complexity, effort, and risk.

- **Client perspective:** implementation and tool cost, process change, ongoing operating cost, and implementation effort relative to plausible improvement.
- **AiA perspective:** delivery effort, risk, complexity, support and dependency burden, and commercial exposure relative to the engagement.

Commercial Fit is not merely whether the Client can pay. Evaluate expected business value against cost, complexity, and risk. Do not invent precise ROI when evidence is insufficient.

### Strong Fit Signals

Positive signals may include repetitive manual work, high interaction volume, fragmented information, duplicated work, dependence on particular people, lost Leads, inconsistent follow-up, repeated customer questions, bottlenecks, slow information retrieval, weak visibility, repeated errors, manual reporting, disconnected systems, or business knowledge trapped in people, chats, or unstructured documents.

These are signals, not mandatory requirements. Repetition or volume is not a gate: a low-frequency problem may still be a strong opportunity when each occurrence consumes substantial executive time or creates material financial or operational risk.

### Knowledge Capture & Compounding Potential

Evaluate this separately as a Strategic Value Multiplier using `HIGH`, `MEDIUM`, `LOW`, or `UNKNOWN`.

Ask whether the system can make valuable operational activity, decisions, exceptions, interactions, or learned patterns observable, documentable, structured, retrievable, and reusable. Potential knowledge may include customer questions, objections, successful responses, reasons for lost sales, exceptions, decision rules, operating knowledge, repeated mistakes, or useful process knowledge.

`Low Knowledge Potential ≠ Reject`

Low knowledge-compounding potential does not prevent an otherwise strong Project. Business Second Brain remains a potential cumulative outcome, not a mandatory Project output; see [[Business-Definition#Business knowledge beyond task automation]].

### Red Flags / Anti-Fit

Identify material Red Flags without assuming each one requires rejection:

- **Problem:** no identifiable or meaningful problem; novelty-only technology request; outcome outside AiA's operating boundary.
- **Client readiness:** essential information or access refused without a workaround; no reachable decision authority; persistent inability or unwillingness to decide or participate; materially unrealistic expectations that cannot be corrected.
- **Feasibility:** proven technical impossibility; unavailable critical data or access without a workaround; unacceptable security, privacy, legal, or regulatory exposure; critical dependencies; no responsible way to obtain required capability.
- **Commercial:** value does not justify cost or complexity; disproportionate scope, risk, support, dependency, or commercial exposure; incompatible expectations after clarification.

Classify each material concern as:

- `UNKNOWN` — evidence is insufficient; normally move toward `NEEDS_MORE_INFORMATION`.
- `REMEDIABLE` — a real weakness may be corrected, such as assigning a decision maker, cleaning data, narrowing scope, changing timeline, or clarifying expectations. State the condition to resolve; do not automatically decline.
- `MATERIAL / NON-REMEDIABLE` — evidence shows the engagement should not reasonably proceed in its current form, such as unlawful conditions, unmitigable security or privacy risk, no meaningful problem, commercially irrational scope without viable rescoping, proven infeasibility, or refusal of essentials for responsible delivery.

### Recommendation logic

Use professional judgment rather than a rigid algorithm:

```text
Available Evidence
→ Evaluate Five Core Dimensions
→ Identify Strong Fit Signals
→ Evaluate Knowledge Multiplier
→ Classify Unknown, Remediable, and Material Red Flags
→ Material evidence missing? → NEEDS_MORE_INFORMATION
→ Material non-remediable weakness? → RECOMMEND_DECLINE
→ Otherwise reasonably valuable, feasible, and commercially justified? → RECOMMEND_ACCEPT
```

- `RECOMMEND_ACCEPT` — evidence supports a reasonably valuable, feasible, and commercially justified opportunity with no unresolved material non-remediable weakness.
- `RECOMMEND_DECLINE` — evidence establishes a material non-remediable weakness that makes responsible pursuit unreasonable in the current form.
- `NEEDS_MORE_INFORMATION` — material evidence is missing, so a stronger recommendation would require guessing.

Do not accept based on a strong average that hides a severe risk. Do not decline automatically because of a single non-material or remediable weakness.

### Practical output

For a meaningful evaluation, record concisely where appropriate:

- Opportunity name or reference
- Each core dimension classification and reason
- Strong Fit Signals
- Material Risks / Red Flags
- Remediable Issues
- Missing Evidence
- Knowledge Capture & Compounding Potential and reason
- AI Recommendation
- Confidence: High, Medium, or Low
- Key Reasoning

This is an output pattern, not a required dedicated template or file.

### Authority and historical traceability

The AI recommendation is advisory. Final authority remains exclusively governed by [[Operating-Principles#AI recommendation and Owner decision authority]]: the Owner reviews and decides `ACCEPT`, `DECLINE`, or `DEFER`, and may override the recommendation. No Fit evaluation may autonomously change a Client, Project, or Opportunity state.

A Fit evaluation belongs to the evidence and context available when made. Do not silently overwrite it when evidence later changes; keep reassessments distinguishable in the applicable existing business context under [[KNOWLEDGE-GOVERNANCE]]. Later outcomes may inform learning without creating a separate versioning, scoring, or machine-learning system.

Related context: [[Market-and-ICP]], [[Discovery]], [[Solution-Selection]], and [[Tool-Selection]].
