# Capability Modelling

**A practical method for modelling enduring business capabilities without accidentally modelling the org chart, systems or current process.**

A business capability model should describe **what an organisation must be able to do**, not how it happens to be organised today.

That sounds simple. In practice, capability maps frequently become disguised org charts, application inventories, process diagrams or transformation plans.

This repository contains a lightweight method, quality tests, worked examples and an AI-assisted modelling skill for keeping capability models useful.

## The core test

A capability should survive reasonable change around it.

Ask:

> **If the organisation restructures, changes software, redesigns the process or ends a transformation programme, should this capability still exist?**

If the answer is no, the model is probably describing implementation rather than an enduring business ability.

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

Other warning signs include capabilities that are so broad they mean almost nothing, sibling capabilities at materially different semantic scales, and definitions that simply repeat the capability name.

See [`anti-patterns/README.md`](anti-patterns/README.md).

## The method

```text
BUSINESS PURPOSE / OUTCOMES
           |
           v
 ENDURING ABILITIES
           |
           v
  CAPABILITY MODEL
           |
           v
QUALITY + ANTI-PATTERN TESTS
           |
           v
GRANULARITY CROSS-CHECK
           |
           v
   REVISE / ACCEPT
           |
           v
MAP ORG / PROCESS / SYSTEM / DATA LATER
```

The order matters. Starting from the current org chart or application estate usually bakes today's implementation into the model.

See [`METHOD.md`](METHOD.md).

## Granularity

Granularity is semantic, not a box-count target.

For the worked examples:

- **L1** means an enterprise-scale enduring ability;
- **L2** means a narrower enduring ability that decomposes one L1;
- workflow steps, tasks, screens, teams, systems, facilities and projects stay outside the capability hierarchy.

The example set deliberately holds L1 models to roughly 8–12 capabilities and selected L2 decompositions to 3–5 siblings so the examples can be compared at the same scale. **Those numbers are not a modelling rule.**

See [`examples/granularity-cross-check.md`](examples/granularity-cross-check.md).

## Quality tests

A proposed capability should pass six questions:

1. **Enduring** — should it still exist after normal organisational or technology change?
2. **Implementation-independent** — can teams, systems and processes change without renaming it?
3. **Business-meaningful** — does it describe an ability the organisation actually needs?
4. **Clear boundary** — can a reader tell what belongs inside and outside it?
5. **Comparable granularity** — is it at roughly the same semantic scale as its siblings?
6. **Useful definition** — does the definition explain the ability rather than restating the name?

The full checklist is in [`checklists/capability-quality.md`](checklists/capability-quality.md).

## Capability definition template

```text
Name
Definition
Business outcome / purpose
Scope included
Scope excluded
Parent capability
Child capabilities
Key information concepts
Relevant measures
Notes / uncertainty
```

The template deliberately does **not** require owner, team, application, process or vendor. Those are mapping dimensions, not capability identity.

See [`templates/capability-definition.md`](templates/capability-definition.md).

## Worked examples

V0.2 uses the same evidence principle as [`codebase-to-edd`](https://github.com/jonathanselby/codebase-to-edd): do not publish only the polished answer; make the evidence basis, rejected interpretations, uncertainty and review recoverable.

Three examples are included:

| Example | Evidence basis | Purpose |
|---|---|---|
| [`Northstar Equipment Hire`](examples/fictional-company/) | fictional source brief | show the method without external evidence dependencies |
| [`Australia Post`](examples/australia-post/) | dated official public sources | large national logistics, retail-access and service network |
| [`Sydney Water`](examples/sydney-water/) | dated official public sources | regulated infrastructure utility |

Every worked example contains:

```text
README
  -> evidence
  -> bad first draft
  -> corrected model
  -> scoped capability definitions
  -> review
```

The public-source models are architectural inference, **not official capability models** of those organisations.

See [`examples/README.md`](examples/README.md).

## AI-assisted modelling

[`SKILL.md`](SKILL.md) defines a constrained AI workflow for proposing a capability model from supplied business evidence.

The important boundary is:

> **The model proposes. The architect accepts, rejects, combines, splits and renames.**

The skill requires the model to expose evidence, assumptions, anti-pattern leakage, granularity problems, missing evidence and boundary questions before anything is accepted.

## Tests

[`tests/quality-cases.md`](tests/quality-cases.md) contains semantic pass/fail/ambiguous cases.

The tests are not automated because terminology alone cannot establish business meaning. A label such as `Customer Account Management` may be a sound capability, a team name or a process label depending on context.

## What comes after the capability model

A capability model becomes more useful when other views are mapped **to it** rather than embedded **inside it**.

```text
CAPABILITY
   +--> business owner / organisational units
   +--> processes
   +--> applications
   +--> data / information concepts
   +--> risks / controls
   +--> suppliers
   +--> investment / change initiatives
   +--> measures / maturity
```

This separation lets the capability remain comparatively stable while the implementation around it changes.

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

The aim is smaller: **make capability models structurally honest enough to be useful.**

## Repository structure

```text
capability-modelling/
├── README.md
├── METHOD.md
├── SKILL.md
├── VERSION
├── CHANGELOG.md
├── LICENSE
├── templates/
├── checklists/
├── anti-patterns/
├── tests/
└── examples/
    ├── README.md
    ├── granularity-cross-check.md
    ├── fictional-company/
    ├── australia-post/
    └── sydney-water/
```

## Licence

MIT. See [`LICENSE`](LICENSE).
