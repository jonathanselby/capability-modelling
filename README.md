# Capability Modelling

**A practical method for modelling enduring business capabilities without accidentally modelling the org chart, systems or current process.**

A business capability model should describe **what an organisation must be able to do**, not how it happens to be organised today.

That sounds simple. In practice, capability maps frequently become disguised org charts, application inventories, process diagrams or transformation plans.

This repository contains a lightweight method, quality tests, fictional examples and an AI-assisted modelling skill for keeping capability models useful.

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

Other warning signs include capabilities that are so broad they mean almost nothing, sibling capabilities at wildly different levels of granularity, and definitions that simply repeat the capability name.

See [`anti-patterns/README.md`](anti-patterns/README.md).

## The method

The method is deliberately small:

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
   REVISE / ACCEPT
           |
           v
MAP ORG / PROCESS / SYSTEM / DATA LATER
```

The order matters. Starting from the current org chart or application estate usually bakes today's implementation into the model.

See [`METHOD.md`](METHOD.md).

## Quality tests

A proposed capability should pass six questions:

1. **Enduring** — should it still exist after normal organisational or technology change?
2. **Implementation-independent** — can teams, systems and processes change without renaming it?
3. **Business-meaningful** — does it describe an ability the organisation actually needs?
4. **Clear boundary** — can a reader tell what belongs inside and outside it?
5. **Comparable granularity** — is it at roughly the same level as its siblings?
6. **Useful definition** — does the definition explain the ability rather than restating the name?

The full checklist is in [`checklists/capability-quality.md`](checklists/capability-quality.md).

## Capability definition template

A capability definition should be short enough to review but rich enough to stop the name carrying all of the meaning.

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

## Worked example

The fictional **Northstar Equipment Hire** example begins with a plausible but poor first draft containing team names, systems, processes and programmes.

It then rebuilds the model around enduring abilities such as:

```text
Customer Management
Fleet Management
Equipment Availability Management
Rental Agreement Management
Fulfilment Management
Maintenance Management
Revenue Management
Supplier Management
Workforce Management
Enterprise Management
```

The point is not that these names form a universal equipment-hire taxonomy. They demonstrate the method and make the corrections inspectable.

Start with:

- [`examples/fictional-company/bad-first-draft.md`](examples/fictional-company/bad-first-draft.md)
- [`examples/fictional-company/corrected-model.md`](examples/fictional-company/corrected-model.md)
- [`examples/fictional-company/capability-definitions.md`](examples/fictional-company/capability-definitions.md)

## AI-assisted modelling

[`SKILL.md`](SKILL.md) defines a constrained AI workflow for proposing a capability model from supplied business evidence.

The important boundary is:

> **The model proposes. The architect accepts, rejects, combines, splits and renames.**

The skill requires the model to:

- derive candidate capabilities from business purpose and responsibilities rather than copying nouns blindly;
- flag unsupported assumptions;
- run its own proposal through the anti-pattern tests;
- identify likely org-chart, system, process, programme and vendor leakage;
- identify inconsistent granularity;
- state what evidence is missing;
- avoid presenting a generated taxonomy as authoritative.

## Tests

[`tests/quality-cases.md`](tests/quality-cases.md) contains small pass/fail cases for the method.

The tests are semantic, not automated. That is deliberate. A capability called `Customer Account Management` may be sound in one context and badly scoped in another. A deterministic name checker cannot establish business meaning.

## What comes after the capability model

A capability model becomes more useful when other views are mapped **to it** rather than embedded **inside it**.

Useful mappings can include:

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
│   └── capability-definition.md
├── checklists/
│   └── capability-quality.md
├── anti-patterns/
│   └── README.md
├── tests/
│   └── quality-cases.md
└── examples/
    └── fictional-company/
        ├── README.md
        ├── bad-first-draft.md
        ├── corrected-model.md
        └── capability-definitions.md
```

## Licence

MIT. See [`LICENSE`](LICENSE).
