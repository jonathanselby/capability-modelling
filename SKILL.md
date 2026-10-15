# Capability Modelling Skill

## Objective

Propose a candidate business capability model from supplied organisational evidence while keeping capability identity separate from org structure, applications, processes, vendors, locations and temporary change programmes.

The output is a **candidate model for architectural review**, not an authoritative taxonomy.

## Evidence rule

Use the supplied material as the basis for the model.

Do not silently fill gaps with generic industry knowledge. When a capability is inferred rather than directly supported, label it as inferred or needs evidence.

## Core definition

A capability is an enduring organisational ability required to produce a business outcome or fulfil a business responsibility.

It describes **what must be possible**, not who performs it or how it is currently implemented.

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
- programmes/change initiatives.

The latter categories may help reveal underlying abilities, but must not be copied into the capability model by default.

### 3. Propose candidate capabilities

Derive enduring abilities needed to deliver the evidenced outcomes and responsibilities.

For each candidate provide:

- name;
- short definition;
- evidence basis;
- confidence: `supported`, `inferred`, or `needs evidence`.

### 4. Build a simple hierarchy

Group capabilities only where hierarchy adds clarity.

Do not create levels merely to make the diagram symmetrical.

Keep sibling granularity reasonably comparable.

### 5. Run anti-pattern review

Explicitly test every candidate for:

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

### 6. Run stability tests

For each material candidate ask whether it should survive:

1. organisational restructuring;
2. replacement of current systems;
3. process redesign;
4. completion of current programmes.

Flag candidates that fail.

### 7. Report uncertainty

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

## Proposed capability hierarchy

## Capability definitions
| Capability | Definition | Evidence basis | Confidence |

## Anti-pattern findings
| Candidate | Finding | Action |

## Granularity / boundary issues

## Assumptions and inferred capabilities

## Missing evidence / questions

## Review summary
```

## Review actions

Use only these review actions where practical:

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
- assume common industry capabilities are present without evidence;
- copy team or system names into the model merely because they appear frequently;
- optimise for a fixed number of capability boxes;
- force every business object into a `... Management` capability;
- create symmetry by invention;
- hide ambiguity behind confident wording;
- score maturity unless explicitly asked and evidence exists;
- map applications, teams or processes into capability identity.

## Human acceptance boundary

The architect or business reviewers decide whether to accept, reject, combine, split, rename or re-level proposed capabilities.

The model proposes and critiques. It does not own business truth.
