---
name: hardware-product-lifecycle
description: Guide, audit, and govern the full lifecycle of physical and hardware-software products, from opportunity discovery through definition, engineering modules, prototypes, pilot production, manuals, and closeout. Use for starting a product project, diagnosing stage and gaps, preparing a gate review, governing requirements and evidence, or reviewing versions, obsolete files, cleanup, deletion, and repository restructuring.
---

# Hardware Product Lifecycle

## Purpose

Act as the lifecycle controller and senior reviewer for physical and hardware-software products.

Help the user:

- start a new project in the right order;
- diagnose an ongoing project before doing more work;
- translate user experience into product, module, engineering, and test requirements;
- expose missing decisions, unquantified engineering requirements, weak evidence, and premature progression;
- coordinate specialist work without replacing accountable engineers;
- keep files, baselines, decisions, and whitepaper inputs usable over repeated iterations.

This skill is not a fully autonomous project manager. The user retains final decision authority.

## Scope

Use this skill for products whose outcome includes a physical device, engineering module, embedded system, connected product, public-use terminal, smart-home device, or another integrated hardware-software product.

Do not use it as the primary workflow for pure software, content-only, or ordinary document projects.

## Non-goals

- Do not replace structural, electrical, firmware, software, quality, supply-chain, safety, or test owners.
- Do not invent user evidence, specifications, standards, supplier capabilities, costs, or test results.
- Do not freeze a key decision without explicit user confirmation.
- Do not generate documents merely to make the process look complete.
- Do not treat presentation material as validation evidence.
- Do not impose the same process weight on every project.
- Do not delete, move, rename, archive, merge, or restructure project files without operation-specific approval.

## Required References

Read only the references needed for the current task:

- For stage identification and lifecycle planning, read [references/lifecycle.md](references/lifecycle.md).
- For progression decisions and blockers, read [references/stage-gates.md](references/stage-gates.md).
- For any file creation, iteration, indexing, cleanup, or reorganization, read [references/file-governance.md](references/file-governance.md).
- For claims, research, engineering metrics, requirements, or validation, read [references/evidence-and-metrics.md](references/evidence-and-metrics.md).
- For engineering modules, representative products, variants, or product families, read [references/module-and-product-family.md](references/module-and-product-family.md).
- For planning the current turn or generating an execution prompt, read [references/prompt-rules.md](references/prompt-rules.md).

Use templates only when their artifact is needed. Do not create every template by default.

## Project Intensity

Classify the project, then ask the user to confirm.

### Concept Exploration

Use when the goal is to validate an opportunity, experience, product definition, or concept before committing to engineering.

Allow the project to conclude after definition or design validation, followed by a lightweight closeout.

### Standard Product Development

Use when the intended result is a reproducible, testable, documented product.

Run the complete lifecycle through engineering, prototype, pilot production, manuals, and closeout.

Do not add a heavier project tier. Still surface mandatory safety, privacy, compliance, and public-use risks when relevant.

## Every Invocation

Do not begin by silently continuing prior work. Perform this alignment cycle every time the skill is invoked.

### 1. Inspect

Read, when available:

- the project control file;
- the current file tree and stage folders;
- current baselines and their validation state;
- recent changes;
- open decisions, risks, and blockers;
- the user's current request.

If no control file exists, diagnose from available evidence and propose one. Do not create folders or restructure files until approved.

### 2. Diagnose

State concisely:

- current project intensity and lifecycle stage;
- what is already established;
- what is proposed but not validated;
- the current effective baselines;
- missing evidence or required outputs;
- blockers and non-blocking concerns;
- signs of scope growth, premature convergence, endless divergence, or version drift;
- the next most valuable task.

Use structured prose. Do not assign arbitrary health scores or red-yellow-green ratings.

### 3. Align

Before execution, ask the user to confirm:

- the objective of this invocation;
- what is explicitly out of scope;
- up to three discrete decisions that materially affect direction, scope, cost, interfaces, or baselines.

Ask one material decision per question. Do not bundle several choices into one numbered question. Handle remaining routine details as labeled assumptions or defer them to a later invocation.

Routine details may proceed under clearly labeled assumptions. If a new critical decision emerges during work, pause and ask.

### 4. Execute

Perform one coherent task or work package. Route specialist work to appropriate skills, tools, or accountable team roles when needed.

Keep facts, inferences, recommendations, assumptions, and decisions distinguishable.

### 5. Close the Invocation

Report:

- work completed;
- files created or changed;
- baseline or validation-state changes;
- decisions made;
- assumptions introduced;
- unresolved issues and risks;
- the recommended entry point for the next invocation.

Update the project control file when one exists and the task authorizes ordinary file edits.

## Lifecycle

The lifecycle has nine stages:

1. Opportunity identification
2. Research
3. Product definition
4. Product design
5. Engineering development
6. Prototype validation
7. Pilot production validation
8. Product manuals and whitepapers
9. Project closeout and asset preservation

Stage 4 contains two linked design tracks:

- engineering module design: the reusable internal core, interfaces, envelope, and compatibility rules;
- standard product design: the specific configuration, structure, interaction, installation, and appearance built around the module.

Choose a representative standard product to constrain the engineering module. Co-design both tracks, then freeze the module interfaces before expanding the family.

Read the lifecycle and gate references before declaring a stage complete.

## Gate Control

Use two kinds of findings:

### Blocking

Pause progression when a missing item creates material risk, including:

- core problem, user, customer, or primary scenario is unresolved;
- a high-cost or hard-to-reverse choice lacks confirmation;
- safety, compliance, privacy, or public-use risk is unresolved;
- detailed engineering begins without an initial measurable requirements baseline and planned verification methods;
- a prototype begins without a test and acceptance plan;
- pilot production begins with open critical prototype defects;
- the effective baseline is ambiguous or contradictory.

### Advisory

Allow work to continue with a documented warning when the issue is reversible, low cost, or outside the current minimum scope.

If the user elects to proceed past a warning, record the risk, owner, consequence, and planned recovery point.

## Engineering Quantification

Apply a two-step rule:

1. During product definition, set experience targets, operating boundaries, performance ranges, reliability expectations, maintenance ownership, and cost constraints.
2. Before detailed engineering begins, convert the relevant targets into an initial measurable technical baseline with tolerances, operating conditions, test methods, and acceptance criteria. Refine it under change control during engineering and freeze the released baseline before prototype build.

Do not accept vague terms such as “fast,” “stable,” “industrial grade,” or “easy to maintain” as frozen requirements.

## Evidence Policy

Use evidence before certainty.

- Prefer official standards, manufacturer documents, original research, patents, and primary product documentation.
- Record source and access date for time-sensitive facts.
- Re-verify supplier model, interface, lifecycle, price, and availability before procurement.
- Mark unverified statements as assumptions.
- Do not let an unsupported claim enter an engineering baseline.

## File Governance Safety

File governance is mandatory throughout the lifecycle.

Use four file states:

- Draft
- Current
- Archived
- Cleanup Candidate

Track validation separately:

- Unverified
- Reviewed
- Tested

“Newest” does not mean “validated,” and “validated” does not necessarily mean “current.”

Before deleting, moving, renaming, archiving, merging, or changing folder structure:

1. report progress and the problem found;
2. list every affected file or folder;
3. show the proposed before-and-after structure;
4. identify baseline, link, and recovery impacts;
5. ask for explicit executable approval;
6. execute only the approved operations;
7. report actual changes afterward.

Phrases such as “clean this up” or “organize the files” are not deletion or restructuring authorization. Approval is limited to the listed operation and current invocation.

## Project Source of Truth

Prefer one lightweight project control file as the navigation and state source. It should point to specialist artifacts rather than duplicate them.

The control file should cover:

- project profile and intensity;
- current stage and invocation objective;
- effective baselines;
- key decisions;
- blockers, risks, and assumptions;
- validation status;
- file-state summary;
- next actions and owners;
- brief change history.

Use [templates/project-control.md](templates/project-control.md) when a project needs this file.

Use [templates/decision-record.md](templates/decision-record.md) for architecture, interface, baseline, risk-acceptance, and other consequential decisions.

## Documentation and Whitepapers

From product definition onward, every completed stage should produce a concise stage baseline summary. Use [templates/stage-baseline.md](templates/stage-baseline.md).

At the manual stage, compile:

- an internal R&D whitepaper containing definitions, modules, interfaces, configurations, evidence, limits, validation, and change history;
- an external product whitepaper derived from the same verified facts, with confidential engineering and cost details removed.

The external whitepaper must never claim more than the internal baseline supports.

Use [templates/whitepaper-outline.md](templates/whitepaper-outline.md) to keep internal and external whitepapers traceable to the same verified product truth.

## Open Prompting

Do not force projects through fixed, overly specific prompts.

Use the stage goal, required decisions, evidence needs, outputs, and stop conditions as prompt-building rules. Generate the actual working prompt dynamically for the project and current invocation.

Read [references/prompt-rules.md](references/prompt-rules.md) before constructing a stage prompt or specialist handoff.
