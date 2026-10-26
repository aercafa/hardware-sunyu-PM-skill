# Evidence, Requirements, and Engineering Metrics

## Purpose

Prevent attractive concepts, supplier claims, or vague experience goals from entering engineering as untested facts.

## Claim Types

Label important statements as one of:

- **Fact:** directly supported by a cited source or observation.
- **Inference:** reasoned interpretation of facts.
- **Recommendation:** proposed action based on evidence and trade-offs.
- **Assumption:** necessary but unverified premise.
- **Decision:** explicitly accepted direction.

Do not convert an assumption into a decision without user confirmation.

## Evidence Hierarchy

Prefer, in order:

1. applicable laws, regulations, and official standards;
2. original manufacturer data, drawings, lifecycle notices, and test reports;
3. direct user, customer, operator, maintenance, or environment observation;
4. original research, patents, or developer documentation;
5. verified project tests and measurements;
6. reputable secondary analysis;
7. internal expert judgment;
8. unverified market or promotional claims.

Use the strongest evidence reasonably available. Record access date for information that can change.

## Research Evidence Record

For important findings record:

| Field | Content |
| --- | --- |
| Question | What decision this research supports |
| Finding | What was observed |
| Claim type | Fact / Inference / Recommendation / Assumption |
| Source | Primary link, file, interview, observation, or test |
| Date | Source or access date |
| Confidence | High / Medium / Low with reason |
| Product implication | What changes because of this finding |

## Two-Step Quantification

### During Product Definition

Set target ranges and boundaries without pretending engineering is complete.

Cover as relevant:

- response and feedback expectation;
- user distance, posture, duration, and concurrency;
- content and data scale;
- operating hours and environment;
- reliability and recovery expectation;
- safety, accessibility, privacy, and compliance boundary;
- installation and maintenance responsibility;
- service time and replaceable units;
- target cost and price boundary;
- intended product lifetime and supply horizon.

### Before Detailed Engineering

Convert each relevant target into:

- measurable parameter;
- nominal value or range;
- tolerance;
- operating condition;
- test method;
- sample size or duration;
- pass / fail threshold;
- responsible owner;
- evidence location.

Treat this as the initial engineering-entry baseline. Detailed engineering may refine values only through documented change control; the released requirements baseline is frozen before prototype build.

## Non-functional Requirement Categories

### Performance

- boot and wake time;
- input and feedback latency;
- frame rate and media capability;
- sensor recognition time and accuracy;
- network and update time;
- simultaneous-user or device load.

### Reliability and Recovery

- operating hours;
- restart and watchdog behavior;
- offline behavior;
- failure recovery;
- endurance and cycle life;
- environmental range;
- data and configuration recovery.

### Safety and Compliance

- electrical and fire safety;
- structural stability and glass safety;
- pinch, crush, edge, and child-access risks;
- EMC and radio compliance;
- accessibility;
- privacy, data minimization, and consent;
- content and intellectual-property rights.

### Maintainability

- access and disassembly time;
- module replacement time;
- diagnostics and logs;
- remote update and rollback;
- spare parts and service ownership;
- cleaning and public-use durability.

### Cost and Supply

- target BOM and manufacturing cost;
- tooling and one-time engineering cost;
- installation and support cost;
- supplier lead time;
- minimum order quantity;
- alternative parts;
- component lifecycle and obsolescence.

## Requirement Quality Check

A frozen requirement should be:

- necessary;
- unambiguous;
- feasible;
- measurable;
- traceable to a need or risk;
- owned;
- testable under stated conditions.

Rewrite:

- “fast response” into a measurable response-time threshold;
- “industrial grade” into operating, endurance, environment, and lifecycle requirements;
- “easy maintenance” into access, diagnosis, replacement, and recovery targets;
- “high quality” into defined visual, mechanical, functional, and reliability acceptance criteria.

## Traceability

From product definition onward, link:

`User or business need -> Product requirement -> Engineering requirement -> Design output -> Test case -> Result`

Use [templates/requirements-traceability.md](../templates/requirements-traceability.md) when the project enters standard product development.

## Evidence Rules at Gates

- Research conclusions need sources.
- Definition decisions need evidence and explicit confirmation.
- Engineering release needs measurable requirements and planned tests.
- Prototype claims need results.
- Pilot claims need repeatability and process evidence.
- Manual and whitepaper claims need a current verified baseline.

If evidence is missing, state the uncertainty and define how it will be resolved. Do not hide the gap with polished language.
