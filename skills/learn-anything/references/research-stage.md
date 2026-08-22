# Adaptive Research Stage

Use this reference to decide whether research will materially improve the learning route, select a research mode with the user, and audit the result.

## Trigger Matrix

Trigger research when one or more of these conditions applies:

| Condition | Why research helps |
|---|---|
| The user explicitly requests research or current sources | Research is part of the requested task. |
| The topic is too broad to map reliably from the current context | Scope and subdomains must be established before sequencing. |
| Important claims are current, contested, high-stakes, or decision-oriented | Source quality, dates, disagreement, and uncertainty can change the route. |
| Available sources or user materials conflict | The conflict must be surfaced and audited. |
| No reliable curriculum, reference map, or authoritative material is available | A defensible learning ladder needs an evidence base. |

Normally skip research when all material questions are covered and one of these conditions applies:

- the request is a narrow, stable how-to;
- the user directly requests a module such as a quiz or Feynman loop;
- the user supplies an authoritative syllabus or bounded source and asks to stay within it;
- research would not change the scope, sequence, examples, safety, or resource choices.

When the decision is close, ask: “What learning decision would new evidence change?” If there is no concrete answer, skip research.

When research is triggered, state the exact reason and let the user choose the mode. Do not silently browse or delegate.

## Research Modes

### 1. Online Search

Use current, primary, and authoritative sources where possible. For technical claims, prefer official documentation and original research. For disputed claims, actively seek credible counterevidence rather than merely collecting supporting links.

If the environment supports subagents and at least one slot is available, dispatch at least 1 subagent before the main agent completes the search. Do not replace delegation with a parent-only search merely because the main agent could do the work. Decide how many genuinely separable investigations exist:

- **1 subagent:** a bounded topic with one dominant evidence base;
- **2 subagents:** two distinct lenses, such as conceptual map and practical ecosystem, or supporting and opposing evidence;
- **3 subagents:** a broad or contested topic with at least three independent workstreams, such as foundations, current practice, and disputes/risks.

Use no more than 3 and never exceed available concurrency. Do not create artificial roles merely to fill slots. Give each subagent a bounded question, source expectations, and the return contract below. The main agent must independently inspect important sources, test whether sources are genuinely independent, reconcile conflicts, and write the synthesis. Agent agreement is never evidence. Briefly record the workstream split in the research scope so the user can see how coverage was divided; do not present the split itself as evidence.

If subagents are unavailable, the main agent performs the searches and the same audit.

### 2. User-Provided Materials

State the material boundary before analyzing. Make claims only to the extent covered by those materials and label any outside background knowledge separately. Identify:

- what the material covers well;
- conflicts or unsupported claims inside it;
- gaps that prevent a reliable learning route;
- questions that require sources outside the provided material.

Do not imply that the material is comprehensive merely because it is internally consistent.

### 3. External Agent Research

Produce the reusable prompt below, customized to the topic, goal, scope, constraints, and known disputes. Then pause. Do not continue to orientation or planning until the user returns the research result.

When results return, audit their sources and claims before using them. A polished response without inspectable evidence is not verified research.

## External Agent Prompt Template

```text
Research [TOPIC] to support a learning journey for a person whose goal is [GOAL OR USE], current level is [CURRENT LEVEL], and constraints are [CONSTRAINTS].

Define a practical research scope before collecting information. Derive the relevant perspectives from the topic rather than using a fixed panel. Include competing perspectives when the domain is disputed and an incentives perspective only when incentives materially affect the evidence or practice.

Prefer primary and authoritative sources. For important claims, trace the evidence to an identifiable source, check dates and source independence, seek credible counterevidence, and distinguish clearly among:
- fact;
- convergence of genuinely independent sources;
- inference from stated evidence;
- hypothesis that remains unverified.

Do not use the agreement of agents, personas, experts, or sources as proof by itself. Do not invent quotations, credentials, citations, or consensus.

Return structured Markdown with exactly these sections:
1. Research Scope
2. Dynamic Perspectives
3. Key Claims
4. Supporting Evidence
5. Opposing Evidence
6. Sources
7. Disputes
8. Uncertainties
9. Open Verification Questions
10. Recommended Learning Focus

For every important source include title, author or organization, date when available, and a direct URL or stable identifier. Keep claims linked to the sources that support or challenge them. Explain material gaps instead of filling them with guesses.
```

## Dynamic Perspectives

Derive perspectives from the topic and the learning decision. Useful dimensions include:

- theory versus real-world practice;
- historical development versus current state;
- mainstream view versus credible dissent;
- system builders, users, affected groups, and regulators;
- technical feasibility, human behavior, safety, and incentives.

Use only dimensions that can change the learning route. If topic-derived perspectives remain unclear, the following are optional brainstorming lenses, not authorities: practitioner, scholar, skeptic, historian, and incentives analyst. The incentives lens is relevant only when supported incentives plausibly shape claims or behavior. Missing a lens suggests a possible blind spot; it does not prove one.

## Fixed Research Return Contract

Every research result must contain:

1. **Research Scope** — included questions, boundaries, date sensitivity, exclusions.
2. **Dynamic Perspectives** — why each selected view matters to this topic.
3. **Key Claims** — concise, prioritized, and labeled fact/convergence/inference/hypothesis.
4. **Supporting Evidence** — evidence linked to each claim.
5. **Opposing Evidence** — credible contradictions, failed replications, limitations, or counterexamples.
6. **Sources** — traceable source list with dates and source types.
7. **Disputes** — what informed parties disagree about and why.
8. **Uncertainties** — confidence limits, missing data, and unstable current facts.
9. **Open Verification Questions** — unresolved questions that could change the route.
10. **Recommended Learning Focus** — proposed priorities and what evidence justifies them.

## Evidence and Bias Audit

Before synthesis, check:

- **Traceability:** Can every material factual claim be traced to a source or direct observation?
- **Source quality:** Is the source primary, authoritative, methodologically credible, and current enough for the claim?
- **Independence:** Are apparently separate sources copying the same upstream claim, dataset, press release, or review?
- **Counterevidence:** Was credible contrary evidence actively sought and represented fairly?
- **Perspective bias:** Do selected perspectives omit an affected group or decision-relevant dimension? Record this as a hypothesis until tested.
- **Incentive claims:** Are alleged incentives documented rather than guessed?
- **Inference control:** Are causal claims, hidden links, predictions, and generalizations explicitly labeled and accompanied by alternatives?
- **Uncertainty:** Are unresolved conflicts and missing evidence visible rather than averaged away?

## Research Stop Conditions

Stop research when all are true:

- the scope is bounded enough to build a learning ladder;
- key learning decisions are supported by traceable sources;
- material disputes have both supporting and opposing evidence where available;
- facts, source convergence, inferences, and hypotheses are separated;
- open questions and evidence gaps are stated;
- additional searching is unlikely to change the immediate learning priorities.

Do not stop merely because agents or sources agree. Do not continue searching for completeness after the route is decision-ready.

## Research-to-Learning Handoff

Return a concise domain orientation, claim-and-evidence map, and draft learning ladder. Make disputed or uncertain foundations visible in the ladder. Ask the user to confirm scope and sequence before generating the detailed plan.
