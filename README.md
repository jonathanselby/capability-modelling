# Capability Modelling

**A practical method for modelling enduring business capabilities without accidentally modelling the org chart, systems or current process.**

A business capability model should describe **what an organisation must be able to do**, not how it happens to be organised today.

That sounds simple. In practice, capability maps frequently become disguised org charts, application inventories, process diagrams or transformation plans.

This repository contains a lightweight method, quality tests, worked examples, visual modelling guidance and an AI-assisted modelling skill for keeping capability models useful.

## The core test

A capability should survive reasonable change around it.

> **If the organisation restructures, changes software, redesigns the process or ends a transformation programme, should this capability still exist?**

If the answer is no, the model is probably describing implementation rather than an enduring business ability.

## Enterprise depth

For a large or complex enterprise, this method treats **three capability levels as the robust default**:

```text
LANDSCAPE GROUPING       visual/navigation only
└── L1 capability        broad enterprise ability
    └── L2 capability    major enduring decomposition
        └── L3 capability elemental enduring ability
```

This is consistent with mature reference-model practice. BIAN deliberately reduced its Business Capability Model to three levels and decomposed most areas to L3; APQC demonstrates disciplined multi-level decomposition for processes; ArchiMate separates capability from process, organisation, application and technology views.

See [`BENCHMARKS.md`](BENCHMARKS.md).

### But depth must earn its cost

**Large / complex enterprise** — complete L1–L3 is normally justified because L3 often exposes materially different ownership, systems, controls, information, investment, suppliers, risk and performance.

**Medium organisation** — complete L1–L2, then use L3 where complexity or the decision requires it.

**Small / simple organisation** — L1–L2 are usually sufficient. There is little value maintaining enterprise-wide L3 detail if the lower-level distinctions do not change a decision.

> **Decompose only while the next level reveals a distinction that matters.**

## What a capability is

For this method, a capability is:

> **An enduring organisational ability required to produce a business outcome or fulfil a business responsibility.**

A capability describes **what must be possible**. It should not prescribe:

- which team performs it;
- which application enables it;
- which vendor supplies it;
- which workflow implements it;
- where it is performed;
- which current programme is changing it.

Those things matter, but they are separate views that can be mapped to capabilities later.

## Common mistakes

A proposed capability is suspect when it is primarily:

- a team name;
- an application;
- a current programme;
- a location;
- a vendor product;
- a workflow step;
- a temporary transformation activity.

See [`anti-patterns/README.md`](anti-patterns/README.md).

## Visual modelling

A serious capability model should be readable as a model, not merely as a list.

This repository uses ASCII nested boxes and hierarchy diagrams so the hierarchy remains visible without requiring proprietary tooling.

Example:

```text
+-----------------------------------------------------------------------+
| CUSTOMER & MARKET                                                     |
|                                                                       |
|  +---------------------------+                                        |
|  | L1 Customer Management    |                                        |
|  |                           |                                        |
|  | +-----------------------+ |                                        |
|  | | L2 Relationship Mgmt  | |                                        |
|  | |                       | |                                        |
|  | | +-------------------+ | |                                        |
|  | | | L3 Preference Mgmt| | |                                        |
|  | | +-------------------+ | |                                        |
|  | +-----------------------+ |                                        |
|  +---------------------------+                                        |
+-----------------------------------------------------------------------+
```

For large models, use two complementary views:

1. **enterprise landscape** — groupings, all L1 and L2 capabilities;
2. **domain detail maps** — each L1 expanded through L2 to L3.

See [`VISUAL-MODELLING.md`](VISUAL-MODELLING.md).

## The method

```text
BUSINESS PURPOSE / OUTCOMES
           |
           v
 ENDURING ABILITIES
           |
           v
  L1 -> L2 -> L3 MODEL
           |
           v
QUALITY + GRANULARITY TESTS
           |
           v
   REVISE / ACCEPT
           |
           v
MAP ORG / PROCESS / SYSTEM / DATA LATER
```

See [`METHOD.md`](METHOD.md).

## Quality tests

A proposed capability should be:

1. **Enduring** — it survives normal organisational and technology change.
2. **Implementation-independent** — teams, systems and processes can change without renaming it.
3. **Business-meaningful** — it describes an ability the organisation genuinely needs.
4. **Clearly bounded** — reviewers can distinguish what is inside and outside it.
5. **Correctly levelled** — siblings operate at comparable semantic scale.
6. **Usefully defined** — the definition adds meaning beyond the name.
7. **Worth decomposing** — L3 exists because the distinction changes a decision, not because the diagram looks neater.

See [`checklists/capability-quality.md`](checklists/capability-quality.md).

## Worked examples

The example standard mirrors the evidence discipline used in [`codebase-to-edd`](https://github.com/jonathanselby/codebase-to-edd): show the source basis, plausible bad interpretation, correction logic, definitions and unresolved uncertainty.

Current examples:

- **Northstar Equipment Hire** — fictional; demonstrates a small organisation where L3 should be selective rather than universal.
- **Australia Post** — public-source example of a large national logistics/service enterprise.
- **Sydney Water** — public-source example of a large, regulated, asset-intensive utility.

Each uses the same package:

```text
README
EVIDENCE
BAD FIRST DRAFT
CORRECTED MODEL
CAPABILITY DEFINITIONS
REVIEW
LANDSCAPE
```

See [`examples/README.md`](examples/README.md) and [`examples/granularity-cross-check.md`](examples/granularity-cross-check.md).

### Evidence caveat

The method can support a complete enterprise L1–L3 model. A public-source example cannot responsibly pretend to know internal capability boundaries, ownership or lower-level detail that public material does not expose.

Therefore:

> **Worked examples decompose to L3 where the evidence supports the distinction and record gaps where it does not. They are architectural inference, not official capability models.**

This is deliberate. Completeness is not permission to invent.

## Capability definition template

```text
Identifier
Name
Level
Definition
Business outcome / purpose
Scope included
Scope excluded
Parent capability
Child capabilities
Key information concepts
Relevant measures
Evidence / uncertainty
```

See [`templates/capability-definition.md`](templates/capability-definition.md).

## AI-assisted modelling

[`SKILL.md`](SKILL.md) defines a constrained workflow for proposing a three-level model.

> **The model proposes. The architect accepts, rejects, combines, splits and renames.**

For large-enterprise scope, the skill must not stop at L2 simply because L3 is harder. It must either propose responsible L3 decomposition or identify where evidence is insufficient.

## What comes after the capability model

A capability becomes more useful when implementation views are mapped **to it** rather than embedded **inside it**.

```text
CAPABILITY
   +--> organisation / ownership
   +--> process / value stream
   +--> applications / technology
   +--> information / data
   +--> risks / controls
   +--> suppliers
   +--> investment / change
   +--> measures / maturity
```

Below L3, switch viewpoint when the detail is better represented as process, activity, information, organisation, application or control—not L4 capability by default.

## What this is not

This repository is not:

- a universal capability taxonomy;
- an industry reference model;
- an org-design method;
- a process-modelling notation;
- an application portfolio method;
- an automated capability classifier;
- a maturity-scoring framework;
- a substitute for business subject-matter expertise.

The aim is: **make capability models structurally honest, deep enough for the organisation, and useful for decisions.**

## Licence

MIT. See [`LICENSE`](LICENSE).
