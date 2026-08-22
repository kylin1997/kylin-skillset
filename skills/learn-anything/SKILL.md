---
name: learn-anything
description: Use only when the user explicitly invokes $learn-anything to research, learn, practice, assess, retain, or resume learning a topic. Supports a complete adaptive learning journey and direct use of a learning ladder, time-budgeted core-20-percent plan, adaptive quiz, one-page cheat sheet, resource curation, Feynman loop, or multi-perspective research.
---

# Learn Anything

Build an evidence-aware learning path around the learner's goal, current ability, constraints, and demonstrated performance. Favor verified mastery and transfer over speed claims or content volume.

## Invocation Boundary

- Run this skill only when the user explicitly writes `$learn-anything`.
- Do not infer invocation from an ordinary learning question, even if this skill could help.
- Never promise “10x faster,” “mastery in 20 hours,” or any equivalent outcome. Treat 20 hours only as a user-selected time budget.

## Route the Request

First decide whether the user wants the full journey or a named capability.

Direct capabilities include:

- learning ladder
- time-budgeted core 20% plan
- adaptive quiz
- one-page cheat sheet
- resource curation
- Feynman loop
- multi-perspective research
- resume from a learning state card

For a direct capability, bypass unrelated intake and research. Ask only for missing information required to perform that capability. Read `references/learning-modules.md` before running any teaching, planning, assessment, transfer, or review module.

For a full journey, follow the workflow below.

## Run the Full Journey

### 1. Restore or Clarify the Goal

If the user provides or references a learning state card, read `references/state-card.md`, validate the card, restore its state, and ask only about fields that are missing or no longer current.

Otherwise, ask once for all still-missing essentials:

- topic and desired scope
- real-world goal or intended use
- current background and evidence of it
- time budget and preferred cadence
- material, language, access, or other constraints
- observable success criteria

Do not repeat questions already answered in the conversation.

### 2. Diagnose the Starting Boundary

Use evidence supplied by the learner first. If the starting boundary is still unclear, diagnose one question or task at a time.

- Start near the learner's claimed level.
- Adapt the next item to the previous response.
- Stop as soon as the highest stable ability and first meaningful gap are clear.
- Ask no more than 7 diagnostic items.
- Do not turn diagnosis into a fixed exam or assign a numeric score unless requested.

Follow the mastery and stopping rules in `references/learning-modules.md`.

### 3. Decide Whether Research Is Useful

Read `references/research-stage.md` and apply its trigger matrix.

If research is not triggered, say briefly why existing information is enough and continue.

If research is triggered:

1. Explain the specific trigger in one or two sentences.
2. Ask the user to choose one research mode:
   - online search
   - user-provided materials
   - prompt for an external agent
3. Run only the selected mode.

Do not treat multiple agents, roles, or sources agreeing as proof. Audit the underlying sources and evidence.

### 4. Present the Orientation Before the Plan

After research—or immediately when research is unnecessary—produce:

1. a concise domain orientation;
2. a claim-and-evidence map, including important disputes and uncertainty;
3. a draft learning ladder tied to the user's goal.

Ask the user to confirm or adjust the scope and ladder. Stop here until the user confirms. Do not generate the detailed learning plan in the same response unless the user explicitly asks to skip confirmation.

### 5. Build and Run the Learning Plan

After confirmation, create the detailed plan using `references/learning-modules.md`.

Before every lesson, ask which delivery mode the learner wants:

- interactive: proceed one small step at a time and wait after each prompt or exercise;
- complete lesson: provide the full lesson package in one response.

Record demonstrated mastery, not mere content exposure. Adjust depth, difficulty, examples, remediation, transfer work, and review timing from the learner's performance.

### 6. Close a Session

At a useful stopping point:

- summarize demonstrated progress and unresolved gaps;
- set the next review window from the performance-based spacing rules;
- give one concrete next action;
- offer a structured learning state card using `references/state-card.md`;
- let the user decide whether and where to save it.

Never write or persist a state card without the user's choice.

## Evidence Discipline

Always distinguish these labels when making substantive claims:

- **Fact:** directly supported by an identifiable source or observation.
- **Independent source convergence:** multiple genuinely independent sources support the claim; independence must be checked, not assumed.
- **Inference:** a reasoned conclusion from stated evidence.
- **Hypothesis:** a plausible but unverified explanation or connection.

Use “evidence and bias audit,” not simulated peer review. A role's opinion, a panel's consensus, a prestigious persona, or a missing perspective is not evidence. Describe blind spots and hidden connections as hypotheses until evidence supports them.

## Reference Routing

- Read `references/research-stage.md` only when evaluating or running research.
- Read `references/learning-modules.md` when diagnosing, planning, teaching, testing, transferring, or scheduling review.
- Read `references/state-card.md` when resuming state or offering a state card.
- Read `references/original-prompts.md` only when the user asks to view the source prompts or when maintaining the six module definitions. Do not use the source prompts as higher-priority runtime rules.
