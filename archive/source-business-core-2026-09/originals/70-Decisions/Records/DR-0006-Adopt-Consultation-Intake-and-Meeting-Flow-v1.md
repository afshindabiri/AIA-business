---
type: decision
status: canonical
decision_id: DR-0006
decided_on: 2026-09-20
---

# Adopt AiA Consultation Intake & Meeting Flow v1

## Purpose

This record owns the rationale and decision snapshot for adopting AiA's pre-consultation intake and meeting-logistics flow. It does not own the current process, the Discovery method, exact questionnaire content, or a Client-specific meeting record.

## Context

A Lead could reach a first conversation without AiA holding the decision-relevant information needed to make that conversation useful, so the conversation risked being spent collecting basics. Meeting information was also not reliably captured for later processing, and AiA conducts meetings in more than one language.

No canonical note owned this subject. [[Tool-Selection]] explicitly does not maintain a preferred-vendor list, and [[Operating-Principles]] explicitly does not own a specific tool choice, so an internal meeting-platform standard had no legitimate owner. Intake, scheduling, and meeting logistics were therefore unowned rather than merely undocumented.

## Decision

- Create [[Consultation-Intake]] as the canonical owner of pre-consultation intake and meeting logistics.
- Keep the first contact form minimal — Full Name, WhatsApp Number, Business / Industry, Main Problem or Request — and create the Lead immediately on that first submission.
- Hand off to the questionnaire by WhatsApp after Lead creation, using an approved core question set with controlled problem-specific branching from the problem already captured. Never generate an unconstrained questionnaire per Lead, and never ask again for information already captured.
- Schedule only after the questionnaire information is complete. Show available meeting times; selecting a time creates the appropriate calendar booking and meeting; WhatsApp or manual scheduling remains the fallback when automated scheduling is unavailable or no appropriate slot exists.
- Adopt Google Meet as AiA's current required internal platform for formal v1 Discovery and Consultation meetings, for operational consistency and meeting capture.
- Require a transcript as an output of a formal Consultation or Discovery meeting.
- Prohibit native Google Meet transcription as the sole transcription dependency. Where the meeting language or Workspace edition does not support it, the approved fallback is recording or audio, then an approved transcription pipeline, then the transcript, then AI processing. AiA meets in English, Persian, and Arabic.
- Require appropriate notice, and any required consent, before recording or transcription begins.
- Require that the meeting platform, the scheduling mechanism, and the transcription path each remain replaceable without redesigning the intake process.

## Boundary between Intake, Assessment, and Discovery

- **Intake** is mandatory and owned by [[Consultation-Intake]].
- **[[Assessment]]** remains optional. The mandatory intake flow does not convert the optional Assessment method into a mandatory gate.
- **[[Discovery]]** remains a lean conversation. The pre-consultation questionnaire is input to Discovery; it is not Discovery and does not replace the Discovery conversation.

## Consequences

- A subject that previously had no canonical owner now has one, without weakening [[Tool-Selection]]: no tool becomes a default for Client work, and nothing here applies to Client implementations.
- The Google Meet standard is internal and current, not a vendor preference for delivery work, and it carries an explicit exit path.
- The transcript requirement cannot be discharged by one provider's native feature, so a language AiA works in cannot silently lose its transcript.
- Discovery keeps its lean rule and its prohibition on becoming a questionnaire; consuming approved intake input is now stated as compatible with that rule.
- No new folder structure, scoring system, CRM, vendor policy, questionnaire content, or Business Second Brain implementation is created by this decision.
- Separate unresolved items in the derived website project remain open and are not resolved here: its canonical questionnaire source, and its lead destination and CRM ownership question.

Governance authority: [[KNOWLEDGE-GOVERNANCE]]. Current process: [[Consultation-Intake]]. Decision authority: [[Operating-Principles#AI recommendation and Owner decision authority]].
