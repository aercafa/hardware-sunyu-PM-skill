# Open Prompting and Invocation Rules

## Purpose

Generate prompts that guide decisions without forcing every product through fixed wording or predetermined solutions.

Do not maintain a large library of rigid task prompts. Build the prompt from current project state.

## Prompt Construction

For the current stage and invocation, include only relevant elements:

1. **Role:** the expert perspective needed now.
2. **Project context:** current product, stage, intensity, and baselines.
3. **Decision objective:** what decision this work must enable.
4. **Inputs:** files, evidence, constraints, and prior decisions.
5. **Unknowns:** assumptions and questions still open.
6. **Task:** the analysis or artifact needed.
7. **Evaluation criteria:** how alternatives will be compared.
8. **Evidence rules:** required sources and verification.
9. **Output:** a useful structure, not a predetermined conclusion.
10. **Stop conditions:** when to pause for user or specialist confirmation.
11. **File rules:** intended source file, version effect, and derived outputs.

## Stage Reminders

### Opportunity

Prompt for problem, actors, value, alternatives, constraints, and research questions. Do not request a product solution too early.

### Research

Prompt around decisions and evidence gaps. Require implications, not only collected examples.

### Product Definition

Prompt for journeys, storyboards, flows, frameworks, product boundaries, requirements, representative product, non-goals, and validation strategy. Keep multiple concepts open until selection criteria exist.

### Product Design

Prompt for engineering module and representative product together. Require interface, service, installation, experience, and variant implications.

### Engineering

Prompt for measurable requirements, architecture alternatives, component evidence, interfaces, risks, test methods, and release inputs.

### Prototype

Prompt for hypotheses, test setup, acceptance criteria, results, defects, corrective action, and retest.

### Pilot Production

Prompt for repeatability, process, yield, configuration, quality, supply, cost, installation, and service readiness.

### Manuals and Whitepapers

Prompt for synthesis from current verified baselines. Separate internal technical truth from external communication.

### Closeout

Prompt for objective comparison, decisions, unresolved risks, reusable assets, file state, reading order, and restart path.

## Decision Frequency

Every invocation must begin with alignment.

Ask the user to confirm no more than three discrete material decisions before execution. Ask one decision per question; do not hide multiple choices inside one numbered item. Avoid asking about routine details that can be handled as labeled assumptions, and defer lower-priority decisions to a later invocation.

Pause again only when new information changes:

- product direction;
- scope or non-goals;
- major cost;
- architecture or interface;
- baseline;
- safety, compliance, or privacy;
- file deletion or structure.

## Specialist Handoff

When another agent, skill, or team role is needed, prepare a handoff containing:

- the decision to support;
- minimum project context;
- current baselines;
- exact inputs;
- constraints and non-goals;
- evidence standard;
- required output;
- questions to answer;
- actions requiring user approval.

Do not provide the intended conclusion to an independent reviewer.

## Exploration Versus Convergence

### During Exploration

- allow multiple approaches;
- avoid premature dimensions, components, or appearance locks;
- expose assumptions;
- define selection criteria before ranking.

### During Convergence

- compare against confirmed criteria;
- limit scope;
- identify one current baseline;
- quantify requirements;
- document rejected alternatives and why;
- control changes after freeze.

The skill should explicitly warn when the project remains in endless exploration or converges without evidence.

## Output Quality

Prefer:

- conclusions before background;
- clear separation of facts and recommendations;
- tables only when they improve comparison;
- direct language;
- links to source artifacts;
- explicit current status and next decision.

Avoid:

- generic innovation language;
- long taxonomies without a use decision;
- unverified precision;
- repeated summaries across files;
- producing HTML, slides, and images before the source content is stable.

## End-of-invocation Summary

Close with:

- objective completed or not;
- artifacts affected;
- decisions and assumptions;
- validation and baseline changes;
- blockers and risks;
- file-governance actions proposed or executed;
- next recommended invocation.
