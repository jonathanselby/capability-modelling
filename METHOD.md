# Capability Modelling Method

## 1. Start from purpose, not structure

Begin with what the organisation exists to achieve, the outcomes it must produce and the responsibilities it must fulfil.

Useful inputs include strategy, products/services, customer commitments, regulatory obligations and operating responsibilities.

Do not start with the org chart, application inventory or current process catalogue.

## 2. Derive candidate enduring abilities

Ask what the organisation must be able to do for those outcomes to remain possible.

A capability is an enduring organisational ability required to produce a business outcome or fulfil a business responsibility.

It describes **what must be possible**, not who performs it or how it is implemented.

## 3. Build the hierarchy deliberately

This method uses three capability levels.

### Landscape grouping — not a capability level

A visual grouping makes a large model readable. Examples might be `Customer & Market`, `Operations`, `Assets` or `Enterprise Support`.

A grouping is navigation. Do not count it as L0 and do not score or map it as if it were an executable business ability.

### Level 1 — broad enterprise capability

L1 represents a major enduring ability of the enterprise.

It should be broad enough to remain stable across major organisational and technology change, but specific enough to have a clear business meaning.

Examples:

- Customer Management
- Asset Management
- Revenue Management
- Risk Management

### Level 2 — major enduring decomposition

L2 decomposes one L1 capability into distinct enduring abilities.

L2 siblings should collectively explain the meaningful scope of their parent without becoming process steps.

Example:

```text
Asset Management
├── Asset Strategy Management
├── Asset Lifecycle Management
├── Asset Performance Management
└── Asset Information Management
```

### Level 3 — elemental business ability

L3 is the lowest capability layer used by default in this method.

It exists to expose distinctions that matter to ownership, systems, controls, information, investment, risk or performance.

Example:

```text
Asset Lifecycle Management
├── Asset Acquisition Management
├── Asset Maintenance Strategy Management
├── Asset Renewal Management
└── Asset Disposal Management
```

L3 is still a capability. It is **not** an activity, task or workflow step.

## 4. Depth policy

### Large or complex enterprise

A complete L1–L3 model is the normal target.

Large enterprises need L3 because L2 often still hides materially different:

- ownership;
- applications and technology;
- data/information concepts;
- regulatory controls;
- suppliers;
- investment/change portfolios;
- risk and performance characteristics.

A model that stops at L2 can look complete while remaining too coarse to support portfolio, operating-model or transformation decisions.

### Medium organisation

Complete L1 and L2 first. Decompose to L3 where the decision requires it or where complexity, regulation or asset intensity makes the distinction material.

### Small or simple organisation

L1 and L2 are usually enough. There is little value in maintaining an enterprise-wide L3 taxonomy if the lower-level distinctions do not change ownership, controls, systems, investment or decisions.

**The stopping rule:** decompose only while the next level reveals a distinction that matters.

## 5. Define boundaries at every level

For each material capability, record:

- name;
- definition;
- business outcome / purpose;
- scope included;
- scope excluded;
- parent;
- children where applicable;
- key information concepts;
- relevant measures;
- evidence / uncertainty where the model is inferred.

If two sibling capabilities cannot be distinguished without naming teams or systems, the boundaries are probably not yet clear.

## 6. Apply the MECE test pragmatically

The children of a capability should aim to be:

- **mutually distinguishable** — avoid deliberate overlap;
- **collectively sufficient** — explain the parent well enough for the model's purpose.

Do not force false mathematical purity. Real enterprises contain cross-cutting concerns. Record boundary decisions rather than hiding them.

## 7. Test for implementation leakage

Challenge every candidate:

- Is this a team or business unit?
- Is this an application or platform?
- Is this a vendor/product?
- Is this a location?
- Is this a workflow step?
- Is this a programme or temporary initiative?
- Is this only a business object with no ability attached?

If yes, identify the enduring ability underneath it or move the item to the appropriate mapping view.

## 8. Test granularity horizontally and vertically

### Horizontal test

Sibling capabilities should operate at comparable semantic scale.

Bad:

```text
Customer Management
Send Renewal Email
Enterprise Operations
```

### Vertical test

Each child should be a genuine decomposition of its parent.

Bad:

```text
Customer Management
└── Finance Management
```

### L3 stopping test

If the next decomposition naturally becomes verbs such as `validate`, `approve`, `send`, `receive`, `route`, `inspect` or `reconcile`, you may be crossing into process/activity modelling.

## 9. Test stability under change

Run four thought experiments:

1. the organisation restructures;
2. major applications are replaced;
3. processes are redesigned;
4. current transformation programmes end.

The capability should still make sense.

## 10. Map implementation separately

Only after the capability model is stable should implementation views be mapped to it.

```text
CAPABILITY
   +--> organisation / owner
   +--> processes / value streams
   +--> applications / technology
   +--> information / data
   +--> risks / controls
   +--> suppliers
   +--> investment / initiatives
   +--> measures / maturity
```

This separation allows the capability hierarchy to remain comparatively stable while the operating model changes.

## 11. Make the model visual

A serious capability model should have at least two views:

1. **enterprise landscape** — landscape groupings plus all L1 and L2 capabilities;
2. **domain detail** — each L1 expanded through L2 to L3.

See [`VISUAL-MODELLING.md`](VISUAL-MODELLING.md).

## 12. Review completeness without chasing symmetry

Ask whether every major enterprise responsibility is represented and whether every L1 can be decomposed far enough for the intended decisions.

Do not invent capabilities merely to make each branch have the same number of children.

## 13. Keep it useful

A capability model earns its cost when it helps answer questions such as:

- Where are multiple systems supporting the same business ability?
- Which capabilities carry the most investment, risk or change?
- Which capabilities are weak, fragmented or strategically important?
- Which capabilities have unclear ownership?
- Where do controls, data or suppliers create concentration risk?
- Which transformation initiatives affect the same underlying business ability?

If deeper decomposition does not improve a decision, stop.
