---
type: process
status: canonical
---

# Consultation Intake

## Purpose

This file owns AiA's current pre-consultation intake and meeting-logistics process. It does not own the Discovery method, exact questionnaire wording, sales pipeline state, lead destination or CRM ownership, Client-specific meeting records, detailed legal or privacy policy, Client-project tool selection, or a preferred-vendor policy for AiA delivery work.

Pre-consultation intake is not [[Assessment]], and the questionnaire is not [[Discovery]].

```text
Minimal intake form
→ Lead created immediately
→ WhatsApp message containing the questionnaire link
→ Questionnaire completed
→ Scheduling
→ Formal Consultation / Discovery meeting
```

## Initial lead capture

Capture only:

- Full Name
- WhatsApp Number
- Business / Industry
- Main Problem or Request

The Lead is created immediately after this first submission. Keep the first form minimal and do not add fields without decision value ([[Operating-Principles]] #16).

## Questionnaire handoff

After the Lead is created, send the Lead a WhatsApp message containing the questionnaire link.

The questionnaire uses an approved core question set with controlled problem-specific branching based on the problem or request already captured. Do not generate an unconstrained new questionnaire for each Lead.

Information already captured is never asked again.

Exact questionnaire wording and final options are governed separately and are not owned here.

## Scheduling

Scheduling happens only after the questionnaire information is complete.

- The scheduling step shows available meeting times.
- Selecting a time creates the appropriate calendar booking and meeting.
- When automated scheduling is unavailable or no appropriate slot exists, WhatsApp or manual scheduling is the fallback.

## Meeting platform

Google Meet is AiA's current required internal platform for formal Discovery and Consultation meetings. The reason is operational consistency and the need to capture meeting information for later processing.

This is an internal operating standard only. It is not a universal preferred vendor, not a requirement for Client implementations, and not an exception to [[Tool-Selection]] for Client projects.

## Transcript

A transcript is a required output of a formal Consultation or Discovery meeting.

Native Google Meet transcription must not be the sole transcription dependency. Use it where the Workspace edition and the meeting language support it. Where the language is unsupported or transcription otherwise fails, the approved fallback is:

```text
meeting recording / audio
→ approved transcription pipeline
→ transcript
→ AI processing
```

AiA conducts meetings in English, Persian, and Arabic, so a single-provider language dependency is not acceptable.

## Notice and consent

Before recording or transcription begins, the participant receives appropriate notice and any required consent is obtained. The detailed legal and privacy implementation is not owned here.

## Replaceability

No component of this flow may become an unremovable dependency. The meeting platform, the scheduling mechanism, and the transcription path must each remain replaceable without redesigning the intake process ([[Operating-Principles]] #13).

## Boundaries

- [[Assessment]] remains optional. This mandatory intake flow does not turn Assessment into a mandatory gate.
- [[Discovery]] remains a lean conversation. The questionnaire is input to Discovery; it does not replace or become Discovery.
- Client-specific meeting facts belong to the relevant Client Phase record under [[KNOWLEDGE-GOVERNANCE]].

Decision rationale: [[DR-0006-Adopt-Consultation-Intake-and-Meeting-Flow-v1]]. Related: [[Discovery]], [[Assessment]], [[Sales-Funnel]], and [[Tool-Selection]].
