# Product Development Lifecycle

## How To Use This Reference

Use this file to identify the current stage, plan the next stage, or explain what “complete” means. Do not treat the lifecycle as a reason to generate every possible document.

Each stage should answer:

- What decision is this stage meant to enable?
- What evidence is needed?
- What is the minimum useful output?
- What must be confirmed before the next stage?

## S1 Opportunity Identification

### Purpose

Determine whether a meaningful and addressable product opportunity exists.

### Core Work

- Clarify the observed problem and its context.
- Separate user, customer, buyer, operator, and maintainer roles.
- State user value and business or organizational value.
- Identify company advantages and capability boundaries.
- Record initial constraints, assumptions, non-goals, and irreversible risks.
- Compare “build a product” with simpler alternatives.

### Typical Outputs

- opportunity brief;
- stakeholder map;
- problem statement;
- value hypothesis;
- initial scope and non-goals;
- proceed / pause / stop recommendation.

### Exit Evidence

- a specific problem and target context;
- a credible reason the product should exist;
- explicit decision owner;
- agreement on the questions research must answer.

## S2 Research

### Purpose

Replace assumptions with enough evidence to define the right product.

### Research Tracks

- users and observed behavior;
- usage environment and journey;
- customer, operator, maintenance, and procurement needs;
- competitors and adjacent product methods;
- enabling technology and engineering feasibility;
- supplier and component landscape;
- commercial model and cost boundaries;
- standards, safety, accessibility, privacy, and compliance.

### Typical Outputs

- research plan and question list;
- evidence library with source dates;
- user or stakeholder findings;
- scenario and journey findings;
- competitor method synthesis;
- technical opportunity and constraint summary;
- unresolved assumptions.

### Exit Evidence

- priority research questions are answered or explicitly left open;
- facts, inferences, and assumptions are separated;
- the opportunity statement has been confirmed or revised;
- research points toward product decisions rather than only collecting cases.

## S3 Product Definition

### Purpose

Convert evidence into a product boundary and a coherent product system.

### Core Work

- define what the product is and is not;
- define primary users, customers, operators, and maintainers;
- map scenarios, journey, storyboard, experience flow, states, and timing;
- establish value, capability, function, experience, and product layers when useful;
- build product-family and module hypotheses;
- prioritize requirements and define the first representative product;
- define standard versus configurable parameters;
- define Must / Should / Could / Won’t scope;
- set initial engineering target ranges and operating boundaries;
- define success criteria and validation plan.

### Visual Definition Outputs

Use visual artifacts when they clarify decisions:

- storyboard;
- user journey;
- service or experience flow;
- state and timing diagram;
- system framework;
- hierarchy or layer diagram;
- spatial relationship drawing;
- low-fidelity layout;
- product-family map.

Do not create diagrams without a decision purpose.

### Exit Evidence

- primary scenario and representative product are confirmed;
- value and critical user journey are understandable;
- scope and non-goals are frozen for the next stage;
- major requirements trace to evidence;
- initial performance, reliability, maintenance, cost, and compliance targets exist;
- a design brief and validation strategy are ready.

## S4 Product Design

### Purpose

Turn the product definition into an integrated, buildable product concept.

### Track A: Engineering Module

Define the reusable internal core:

- function boundary;
- mechanical envelope;
- mounting and service access;
- electrical power and connectors;
- data and control interfaces;
- firmware and software boundary;
- thermal path;
- sensor, actuator, and display compatibility;
- test points and diagnostics;
- variant compatibility and change impact.

### Track B: Standard Product

Define a specific product built around the module:

- target scenario and user relationship;
- product configuration;
- industrial design and structure;
- interaction and UI;
- installation and maintenance;
- material and process direction;
- accessibility and safety;
- product-family visual language.

### Working Rule

Select a representative standard product first. Co-design the product and module until real constraints are known. Freeze the reusable module interfaces before expanding additional variants.

### Exit Evidence

- representative product concept is accepted;
- module envelope and interfaces are sufficiently stable;
- interaction, UI, structure, electronics, and software agree on states and interfaces;
- key technical risks have proof-of-concept plans;
- engineering inputs and change-sensitive assumptions are documented;
- relevant experience targets have been converted into an initial measurable engineering baseline, including operating conditions, tolerances, planned test methods, and acceptance criteria.

## S5 Engineering Development

### Purpose

Produce detailed, testable engineering outputs.

### Core Work

- detailed mechanical, electrical, embedded, software, and backend design;
- component and mainboard selection;
- interface control;
- power, thermal, signal, and connectivity design;
- connection and power-on tests;
- firmware loading and configuration;
- state-machine and control integration;
- design for manufacture, assembly, service, and test;
- BOM, supplier alternatives, and lifecycle review;
- change-controlled refinement of measurable requirements and acceptance criteria;
- verification execution planning and traceability;
- final engineering release baseline for prototype build.

### Exit Evidence

- design files and interface definitions are released;
- critical components and alternatives are known;
- measurable requirements have test methods;
- prototype BOM and build package are ready;
- known high-risk technical questions have test plans.

## S6 Prototype Validation

### Purpose

Verify that the product works as an experience and as an engineered object.

### Core Work

- prototype build and bring-up;
- hardware-software integration;
- usability and comprehension testing;
- functional, performance, thermal, noise, stability, safety, and service tests;
- defect logging, root cause, correction, and retest;
- cost and manufacturability learning;
- requirements traceability update.

### Exit Evidence

- critical user journey works;
- blocking defects are closed or formally accepted;
- failures have evidence and ownership;
- the design revision for pilot is identified;
- test results update the current baseline.

## S7 Pilot Production Validation

### Purpose

Verify repeatability, process capability, quality, supply, and delivery readiness.

### Core Work

- small-batch procurement and build;
- work instructions and fixtures;
- incoming, in-process, and final inspection;
- assembly time and yield tracking;
- firmware and configuration control;
- packaging, installation, and service rehearsal;
- cost ledger and supplier confirmation;
- pilot issue closure.

### Exit Evidence

- product can be repeatedly built to the acceptance standard;
- BOM, process, firmware, and inspection versions are controlled;
- critical quality and supply risks are acceptable;
- manuals have verified source material.

## S8 Product Manuals and Whitepapers

### Purpose

Turn verified development knowledge into reusable product knowledge.

### Outputs

- product manual;
- configuration and compatibility guide;
- installation, operation, maintenance, and troubleshooting guidance;
- internal R&D whitepaper;
- external product whitepaper;
- product-family and module rules;
- known limits and support boundaries.

### Source Rule

Compile from confirmed stage baselines and verified evidence. Do not reconstruct facts from memory or marketing language.

### Exit Evidence

- every claim traces to the current baseline;
- internal and external documents are consistent;
- confidential information is filtered from external materials;
- owners and update rules are defined.

## S9 Closeout and Asset Preservation

### Purpose

Close the project responsibly and preserve reusable value.

### Core Work

- compare outcomes with original goals;
- summarize decisions, deviations, costs, defects, and lessons;
- identify patents, reusable modules, templates, suppliers, and test assets;
- mark current, archived, and cleanup-candidate files;
- produce a handoff reading order;
- record follow-up roadmap and ownership.

### Exit Evidence

- project status is unambiguous;
- current baselines and historical assets are separated;
- unresolved risks have owners or are formally accepted;
- cleanup actions are proposed and explicitly approved before execution;
- a new colleague or agent can restart from the preserved context.

## Intensity Adaptation

### Concept Exploration

- emphasize S1-S4;
- use the smallest evidence set that can validate the opportunity;
- stop when the concept decision is made;
- perform a lightweight S9 closeout;
- do not invent engineering maturity.

### Standard Product Development

- use all stages;
- maintain requirements traceability from S3 onward;
- freeze measurable requirements before detailed engineering;
- require test evidence before progression;
- preserve module and product-family compatibility across variants.
