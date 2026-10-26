# Stage Gates and Progression Rules

## Purpose

Use stage gates to make decisions, not to reward document volume. A gate passes only when the decision can be made with adequate evidence.

## Finding Types

### Blocking Finding

The next stage would create material cost, architecture, schedule, quality, or rework risk. Pause and obtain resolution. A reversible, non-regulatory residual risk may proceed only through the controlled exception defined below.

Legal, mandatory compliance, unresolved safety, and unresolved privacy blockers are non-waivable. They require evidence of resolution or an approved control by the accountable specialist before progression.

### Advisory Finding

The issue is reversible, low cost, optional, or outside the current minimum scope. Work may continue after the issue is recorded.

## Universal Gate Questions

At every gate ask:

1. What decision is being requested?
2. Which current baseline supports it?
3. What evidence was reviewed?
4. What remains an assumption?
5. Which requirements or interfaces change?
6. What new cost or irreversible commitment begins next?
7. Who owns unresolved items?
8. Which files become current, archived, or cleanup candidates?

## G1 Opportunity Gate

### Pass When

- the problem, context, user, customer, and decision owner are identifiable;
- value is plausible for both user and organization;
- alternatives to building have been considered;
- research questions and constraints are explicit.

### Block When

- the solution is fixed before the problem is understood;
- user and buyer are conflated without analysis;
- the project exists only because a technology or component is available.

## G2 Research Gate

### Pass When

- priority questions have evidence;
- research sources and dates are recorded;
- findings have been synthesized into implications;
- critical unknowns are visible.

### Block When

- case collection is mistaken for insight;
- claims rely on secondary summaries where primary sources are available;
- no real user, customer, operator, or environment evidence exists for a standard product project.

## G3 Definition Freeze

### Pass When

- product definition and non-goals are clear;
- primary scenario, journey, and representative product are confirmed;
- scope priority and validation plan exist;
- standard and configurable parameters are separated;
- initial engineering, reliability, maintenance, cost, and compliance targets exist;
- requirements trace to evidence.

### Block When

- the project is still expanding core functions;
- multiple product directions compete without a selection rule;
- the team is designing appearance without a confirmed use relationship;
- “fast,” “stable,” or “industrial grade” remain unbounded claims.

## G4 Design Freeze

### Pass When

- representative product and engineering module have been co-designed;
- module envelope and interfaces are documented;
- interaction, UI, structure, hardware, and software share the same state logic;
- major proof-of-concept tests are complete or planned;
- compatibility and change-sensitive assumptions are visible;
- relevant requirements are measurable and include operating conditions, tolerances, planned test methods, and acceptance criteria suitable for entering detailed engineering.

### Block When

- a universal module is designed without a representative product;
- appearance hides unresolved service, thermal, interface, or mounting problems;
- product variants are expanded before module interfaces stabilize;
- detailed engineering is expected to discover requirements that should already be quantified.

## G5 Engineering Release

### Pass When

- requirements are measurable;
- test methods and acceptance thresholds exist;
- drawings, BOM, interfaces, firmware, and configuration are versioned;
- safety and compliance risks have owners;
- prototype build inputs are complete.

### Block When

- the prototype is being used to discover basic requirements that should already be defined;
- critical components lack lifecycle or alternative-supply review;
- there is no trace from requirement to planned test.

## G6 Prototype Gate

### Pass When

- the critical journey works;
- required tests have results;
- critical defects are closed, accepted, or assigned with a dated correction plan;
- the pilot revision is identified;
- user and engineering findings changed the baseline where necessary.

### Block When

- a presentation demo is treated as a validated prototype;
- known safety, thermal, stability, or usability failures are hidden by scope wording;
- failed tests are not repeated after correction.

## G7 Pilot Gate

### Pass When

- repeatable manufacturing and inspection are demonstrated;
- yield, assembly, configuration, and quality issues are known;
- BOM and firmware are controlled;
- supply and cost fit the business boundary;
- installation, maintenance, and recovery procedures have been rehearsed.

### Block When

- pilot units differ without configuration records;
- critical parts have no viable supply plan;
- quality depends on individual craftsmanship rather than a controlled process.

## G8 Documentation Gate

### Pass When

- manuals and whitepapers use verified current baselines;
- internal and external claims agree;
- known limits, compatibility, maintenance, and ownership are documented;
- confidential details are correctly separated.

### Block When

- marketing claims exceed test evidence;
- manuals refer to superseded hardware, firmware, or installation methods.

## G9 Closeout Gate

### Pass When

- final status and incomplete work are explicit;
- assets, baselines, decisions, and lessons are indexed;
- current and historical files are separated;
- deletion or restructuring proposals have user approval before execution;
- restart ownership and reading order are clear.

## Overriding a Gate

Use `Conditional` only when every unresolved item is advisory or a reversible, non-regulatory residual risk, and the next work is explicitly bounded. A conditional result must not authorize an irreversible purchase, engineering release, prototype build, pilot run, or market claim that depends on the unresolved item.

Risk acceptance requires a named decision-maker with authority over the affected scope and a named technical owner. It cannot waive law, mandatory compliance, unresolved safety, or unresolved privacy requirements.

When an authorized decision-maker elects to proceed conditionally, record:

- the skipped condition;
- why proceeding is justified;
- expected consequence;
- responsible owner;
- latest recovery date or stage;
- affected files and baselines.

Do not allow an accepted risk to disappear from later reviews.
