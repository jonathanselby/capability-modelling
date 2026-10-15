# Capability Modelling Skill

## Objective

Propose a candidate business capability model from supplied organisational evidence while keeping capability identity separate from org structure, applications, processes, vendors, locations, assets/facilities and temporary change programmes.

The output is a **candidate model for architectural review**, not an authoritative taxonomy.

## Evidence rule

Use the supplied material as the basis for the model.

Do not silently fill gaps with generic industry knowledge. When a capability is inferred rather than directly supported, label it as inferred or needs evidence.

## Core definition

A capability is an enduring organisational ability required to produce a business outcome or fulfil a business responsibility.

It describes **what must be possible**, not who performs it or how it is currently implemented.

## Modelling levels

Use levels semantically:

- **L1** — enterprise-scale enduring ability;
- **L2** — narrower enduring ability that decomposes one L1;
- **process/task** — activities/workflow detail; do not place these in the capability hierarchy.

Do not infer that L1 must contain a fixed number of capabilities or every L1 must have the same number of L2s.

## Workflow

### 1. Establish scope

Identify from the supplied evidence:

- organisation/business area in scope;
- business purpose and outcomes;
- products/services;
- customer or stakeholder responsibilities;
- regulatory/operating obligations where supplied;
- material uncertainties.

### 2. Extract evidence without modelling yet

Separate relevant evidence into:

- outcomes/responsibilities;
- business objects/information concepts;
- organisation/team names;
- applications/platforms;
- vendors/products;
- processes/activities;
- locations;
- assets/facilities;
- programmes/change initiatives.

Implementation categories may reveal underlying abilities but must not be copied into the capability model by default.

### 3. Propose L1 candidate capabilities

Derive enterprise-scale enduring abilities needed to deliver evidenced outcomes and responsibilities.

For each candidate provide:

- name;
- short definition;
- evidence basis;
- confidence: `supported`, `inferred`, or `needs evidence`.

### 4. Add L2 only where it improves meaning

Decompose an L1 only into narrower enduring abilities.

Do not use process steps as L2s. Do not create L2 merely for visual symmetry.

### 5. Run anti-pattern review

Explicitly test every candidate for:

- team/org-chart leakage;
- application/platform leakage;
- vendor/product leakage;
- process-step leakage;
- programme/change leakage;
- location leakage;
- asset/facility leakage;
- outcome-as-capability;
- object-without-ability;
- excessive breadth;
- inconsistent granularity;
- tautological definition.

### 6. Run sibling granularity review

For each sibling set test:

- would one candidate naturally contain another?
- is one candidate a single task while peers are broad abilities?
- is one candidate primarily implementation rather than business ability?
- is one candidate materially broader or narrower without evidence-based reason?

Use review actions: `ACCEPT`, `REVISE`, `COMBINE`, `SPLIT`, `MOVE LEVEL`, `REMOVE`, `NEEDS EVIDENCE`.

### 7. Run stability tests

For each material candidate ask whether it should survive:

1. organisational restructuring;
2. replacement of current systems;
3. process redesign;
4. completion of current programmes.

Flag candidates that fail.

### 8. Report uncertainty

List:

- capabilities that need business validation;
- overlaps/boundary questions;
- likely missing evidence;
- candidates that were removed or renamed and why.

## Required output

```markdown
# Candidate Capability Model

## Scope and evidence basis

## Business purpose / outcomes

## Proposed L1 capability hierarchy

## Selected L2 decompositions

## Capability definitions
| Capability | Definition | Evidence basis | Confidence |

## Anti-pattern findings
| Candidate | Finding | Action |

## Granularity cross-check

## Boundary issues

## Assumptions and inferred capabilities

## Missing evidence / questions

## Review summary
```

## Things not to do

Do not:

- present an AI-generated taxonomy as authoritative;
- assume common industry capabilities are present without evidence;
- copy team, system, site, product or asset names into the model merely because they appear frequently;
- optimise for a fixed number of capability boxes;
- force every business object into a `... Management` capability;
- create symmetry by invention;
- hide ambiguity behind confident wording;
- use process steps as L2 capabilities;
- score maturity unless explicitly asked and evidence exists;
- map applications, teams or processes into capability identity.

## Human acceptance boundary

The architect or business reviewers decide whether to accept, reject, combine, split, rename or re-level proposed capabilities.

The model proposes and critiques. It does not own business truth.
