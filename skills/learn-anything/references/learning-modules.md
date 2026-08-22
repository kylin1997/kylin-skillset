# Adaptive Learning Modules

Use these rules for diagnosis, planning, lessons, assessment, transfer, review, and the six named modules.

## Shared Mastery Rubric

Use qualitative evidence by default:

| State | Evidence |
|---|---|
| 尚未掌握 / Not yet mastered | Cannot perform the target task reliably even with basic prompting, or holds a blocking misconception. |
| 部分掌握 / Partially mastered | Handles familiar examples with support but is inconsistent, incomplete, or fragile under variation. |
| 稳定掌握 / Stably mastered | Performs representative tasks accurately without material support and can explain key decisions. |
| 能够迁移 / Transferable | Applies the skill to a meaningfully different real context, justifies adaptations, and detects limitations. |

Give a numeric score only when the user requests one or an external rubric requires it. A correct answer may show stable recall but does not alone prove transfer.

## Adaptive Diagnosis

Ask one item at a time and wait for the learner's response.

1. Begin with a short application, explanation, prediction, or worked example near the claimed level.
2. If the answer is strong, increase difficulty or variation.
3. If it is weak, test the nearest prerequisite rather than asking another equally difficult question.
4. Use supplied artifacts, prior work, or observable performance as stronger evidence than self-ratings.
5. Stop when the highest stable ability and the first limiting gap are identified, or after 7 items—whichever comes first.

State the inferred starting boundary, evidence, uncertainty, and recommended entry point. Do not diagnose unrelated subdomains.

## Lesson Delivery Contract

Before each lesson, ask the learner to choose:

- **Interactive:** explain or demonstrate one small unit, prompt the learner, and wait; adapt the next step to the response.
- **Complete lesson:** provide objectives, concise instruction, examples, guided practice, independent practice, self-check, common errors, and next step in one response.

Do not assume a previous choice applies to every future lesson. Ask again at the start of each lesson, but if the learner has explicitly set a standing preference, confirm only when context or difficulty changes materially.

## Module 1: Learning Ladder

Build five levels by default, changing the count only when the domain structure clearly requires it or the user asks. For each level include:

- level name and role in the journey;
- prerequisites and target understanding;
- observable mastery evidence using the four-state rubric;
- high-leverage concepts or skills;
- milestone and stopping condition;
- hands-on practice;
- real transfer task(s);
- common errors;
- short self-check;
- next review window.

Do not advance because time elapsed or content was viewed. Advance when the level milestone is demonstrated or when the learner knowingly accepts an unresolved gap.

## Module 2: Time-Budgeted Core 20% Plan

Treat “core 20%” as a prioritization heuristic, not a mathematical guarantee. Ask for the actual time budget, cadence, goal, and constraints if missing. A user may choose 20 hours, but never promise mastery within it.

Identify the smallest set of concepts and skills most likely to unlock the user's target use. Explain both the expected leverage and what the plan omits. Allocate sessions around practice and feedback, not equal content slices. For each session include:

- learning objective;
- prerequisite or dependency;
- key concept or skill;
- practice or mini-project;
- suitable resource if needed;
- evidence expected at completion;
- review or retrieval prompt;
- adaptation rule if performance is weak or strong.

End with a goal-aligned project or performance task and explicit success criteria.

## Module 3: Adaptive Quiz

Ask one question at a time. Unless the user requests a fixed test length, stop when the ability boundary is clear, coverage is adequate for the stated goal, or further questions have low information value.

After each answer:

1. identify what is correct;
2. identify the exact gap, error, or uncertainty;
3. give the four-state mastery judgment for the tested capability;
4. re-teach only what is needed;
5. choose the next question adaptively.

If the answer is weak, probe or remediate the underlying gap before advancing. If strong, increase difficulty, variation, or transfer demand. At the end, report evidence-backed strengths, gaps, recommended revision, review timing, and optional challenge items. Use numeric grades only if requested.

## Module 4: One-Page Cheat Sheet

Create a compact, five-minute review artifact tuned to the learner's use case. Include:

- plain-language definition and scope;
- essential concepts, rules, formulas, or steps;
- a compact table, flow, diagram, or mental model only when it improves recall;
- concrete examples;
- common mistakes and edge cases;
- a before-use checklist;
- rapid retrieval questions.

Keep uncertainty and context-dependent rules visible. Do not compress away safety constraints or turn disputed claims into settled facts.

## Module 5: Resource Curation

Ask what access, format, language, cost, and time constraints matter. Research current resources when freshness or availability matters and follow `research-stage.md` when research triggers are met.

Recommend only the smallest high-leverage set. For each resource include:

- name, type, creator, and link or identifier;
- why it fits this learner and goal;
- exact scope it covers;
- level and prerequisites;
- how to use it;
- limitation, blind spot, or material to skip.

Order the resources by dependency and use, not popularity. Do not invent availability or treat repeated recommendations as independent quality evidence.

## Module 6: Feynman Loop

Run this as an interactive loop unless the user explicitly asks for a demonstration.

1. Give a short, plain-language explanation with a concrete example or analogy.
2. Ask the learner to explain it back in their own words.
3. Mark what is accurate and locate every material gap, ambiguity, or misconception.
4. Re-teach only the missing part.
5. Ask for a cleaner explanation or a varied application.
6. Repeat until the target explanation is simple, accurate, complete enough for the goal, and survives one transfer check.

Stop when the agreed success criterion is met, not when the explanation merely sounds fluent. End with a clean saveable explanation and note any intentionally excluded complexity.

## Transfer Tasks

Assign one real transfer task per ladder level by default. Increase to 2–3 when a level contains multiple distinct abilities or one task cannot sample the important variation. The learner may request transfer testing at any time.

A transfer task must change at least one meaningful dimension from practice: context, data, constraints, audience, tool, representation, or failure mode. State what successful transfer would demonstrate.

Before proposing or initiating a task involving significant time, money, public posting, account changes, physical risk, or other external operations, explain the commitment and ask the user first. Prefer a low-cost simulation when it can test the same ability.

## Dynamic Difficulty

- Two strong performances across different examples: raise variation or reduce scaffolding.
- One strong performance: verify with a different representation or context before declaring stable mastery.
- A partial performance: retain level, target the exact gap, then retry with a near variant.
- A blocking misconception or repeated failure: step down to the nearest prerequisite and shorten the review interval.
- A successful real transfer: mark “能够迁移” only for the demonstrated scope, not the entire domain.

## Stopping Conditions

Stop a lesson or module when one of these applies:

- the agreed objective and evidence criterion are met;
- the next step depends on user input, external research, consent, or a future review interval;
- cognitive load or repeated errors indicate that consolidation is more useful than new material;
- the time budget is reached, with unfinished scope and tradeoffs stated;
- continued questioning adds little diagnostic value.

Never continue solely to complete an arbitrary number of questions, exercises, or levels.

## Performance-Based Spaced Review

Set a review window rather than pretending to know an exact optimal date:

| Current evidence | Default action and next review |
|---|---|
| 尚未掌握 | Correct or rebuild the prerequisite in the same session; review again within 1 day. |
| 部分掌握 | Use targeted retrieval or a near-variant task in 1–2 days. |
| 稳定掌握 | Use mixed retrieval or a harder variation in 3–7 days. |
| 能够迁移 | Revisit in 7–14 days or at the next real milestone. |

After success, lengthen the next interval and increase variation gradually. After failure, shorten the interval, identify whether the issue is recall, understanding, or transfer, and remediate before retesting. Adjust for deadlines, task frequency, difficulty, and learner preference.
