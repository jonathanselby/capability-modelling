# Capability Modelling Skill

## Objective

Propose a candidate three-level business capability model from supplied organisational evidence while keeping capability identity separate from org structure, applications, processes, vendors, locations and temporary change programmes.

The output is a **candidate model for architectural review**, not an authoritative taxonomy.

## Evidence rule

Use supplied material as the evidence basis.

Do not silently fill gaps with generic industry knowledge. When a capability is inferred rather than directly supported, label it `inferred` or `needs evidence`.

## Core definition

A capability is an enduring organisational ability required to produce a business outcome or fulfil a business responsibility.

It describes **what must be possible**, not who performs it or how it is currently implemented.

## Hierarchy

Use:

```text
LANDSCAPE GROUPING       navigation only
└── L1 capability        broad enterprise ability
    └── L2 capability    major enduring decomposition
        └── L3 capability elemental enduring ability
```

Do not create L4 by default. Below L3, switch viewpoint when the material is better represented as process, task, information, organisation, application or control detail.

## Depth rule

### Large / complex enterprise

Target a complete L1–L3 model unless the evidence is insufficient. If evidence is missing, show the gap rather than stopping silently.

### Medium organisation

Complete L1–L2 and propose L3 where complexity or the decision requires it.

### Small / simple organisation

Do not force enterprise-wide L3. Use it only where the distinction is materially useful.

## Workflow

### 1. Establish scope

Identify:

- organisation/business area in scope;
- business purpose and outcomes;
- products/services;
- customer/stakeholder responsibilities;
- regulatory and operating obligations supplied;
- material uncertainties.

### 2. Extract evidence without modelling yet

Separate evidence into:

- outcomes/responsibilities;
- business objects/information concepts;
- organisation/team names;
- applications/platforms;
- vendors/products;
- processes/activities;
- locations;
- programmes/change initiatives.

Implementation-shaped nouns may reveal underlying capabilities but must not be copied by default.

### 3. Propose landscape groupings

Use a small number of visual/navigation groupings if they make the model easier to read.

Do not treat groupings as capabilities.

### 4. Propose L1 capabilities

Derive broad enduring enterprise abilities required by the evidence.

For each provide:

- identifier;
- name;
- short definition;
- evidence basis;
- confidence: `supported`, `inferred`, or `needs evidence`.

### 5. Decompose every L1 to L2

For each L1:

- identify distinct enduring child abilities;
- test whether the children collectively explain the parent;
- remove process steps, teams, systems and programmes;
- check sibling granularity.

### 6. Decompose to L3

For large/complex enterprise scope, decompose each material L2 to L3.

An L3 is justified when it reveals a distinction likely to matter to one or more of:

- accountability;
- systems;
- information;
- regulation/control;
- risk;
- supplier dependency;
- investment/change;
- performance measurement.

Do not create L3 solely for visual symmetry.

### 7. Run anti-pattern review

Test every candidate for:

- team/org-chart leakage;
- application/platform leakage;
- vendor/product leakage;
- process-step leakage;
- programme/change leakage;
- location leakage;
- outcome-as-capability;
- object-without-ability;
- excessive breadth;
- inconsistent granularity;
- tautological definition.

### 8. Run horizontal and vertical granularity review

For each sibling set:

- are the children peers in semantic scale?
- does each child genuinely decompose the same parent?
- has one branch drifted into task/process detail while another remains a capability?

### 9. Run stability tests

For every material L1/L2/L3 candidate ask whether it should survive:

1. organisational restructuring;
2. replacement of current systems;
3. process redesign;
4. completion of current programmes.

Flag failures.

### 10. Produce visual views

Produce:

- an enterprise landscape showing groupings, L1 and L2;
- detailed hierarchy views expanding every L1 through L2 to L3.

ASCII nested boxes or tree diagrams are acceptable when diagram tooling is unavailable.

### 11. Report uncertainty

List:

- capabilities requiring business validation;
- overlaps/boundary questions;
- likely missing evidence;
- branches that could not be responsibly decomposed to L3;
- candidates removed/renamed/re-levelled and why.

## Required output

```markdown
# Candidate Capability Model

## Scope and evidence basis

## Organisation complexity / depth decision

## Business purpose / outcomes

## Landscape groupings

## Enterprise landscape — L1/L2

## Detailed hierarchy — L1/L2/L3

## Capability definitions
| ID | Level | Capability | Definition | Evidence basis | Confidence |

## Anti-pattern findings
| Candidate | Finding | Action |

## Granularity / boundary issues

## Assumptions and inferred capabilities

## Missing evidence / questions

## Review summary
```

## Review actions

Use:

```text
ACCEPT
REVISE
COMBINE
SPLIT
MOVE LEVEL
REMOVE
NEEDS EVIDENCE
```

## Things not to do

Do not:

- present an AI-generated taxonomy as authoritative;
- stop at L2 for a large enterprise merely because L3 is harder;
- invent L3 where evidence is absent;
- force every branch to have the same number of children;
- turn process activities into L3 capabilities;
- assume common industry capabilities without evidence;
- copy teams, products, systems or vendors into capability identity;
- map applications, teams or processes into capability identity;
- score maturity unless explicitly requested and evidence exists.

## Human acceptance boundary

The architect and business reviewers decide whether to accept, reject, combine, split, rename or re-level proposed capabilities.

The model proposes and critiques. It does not own business truth.
