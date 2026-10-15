# Visual Modelling

A capability model is both a semantic model and a communication artefact. A list alone is not enough for serious enterprise use.

## Visual rule

Use nested boxes to make hierarchy visible while keeping layout independent of organisation structure.

Example:

```text
+-----------------------------------------------------------------------+
| CUSTOMER & MARKET                                                     |
|                                                                       |
|  +---------------------------+   +---------------------------------+  |
|  | L1 Customer Management    |   | L1 Channel Management           |  |
|  |                           |   |                                 |  |
|  | +-----------------------+ |   | +-----------------------------+ |  |
|  | | L2 Relationship Mgmt  | |   | | L2 Channel Portfolio Mgmt | |  |
|  | |                       | |   | |                             | |  |
|  | | +-------------------+ | |   | | +-------------------------+ | |  |
|  | | | L3 Contact Mgmt   | | |   | | | L3 Channel Design      | | |  |
|  | | +-------------------+ | |   | | +-------------------------+ | |  |
|  | | +-------------------+ | |   | | +-------------------------+ | |  |
|  | | | L3 Preference Mgmt| | |   | | | L3 Channel Performance | | |  |
|  | | +-------------------+ | |   | | +-------------------------+ | |  |
|  | +-----------------------+ |   | +-----------------------------+ |  |
|  +---------------------------+   +---------------------------------+  |
+-----------------------------------------------------------------------+
```

The outermost box is a landscape grouping, not an additional capability level.

## What belongs on the landscape

A high-level landscape should normally show:

- landscape groupings;
- all L1 capabilities;
- enough L2/L3 detail to make decomposition visible;
- identifiers where the model is large enough to require stable references.

For a large model, do not force every L3 box onto one unreadable page. Use two complementary views:

1. **enterprise landscape** — groupings, L1 and L2;
2. **domain detail maps** — one L1 capability expanded through L2 to L3.

Together these form the complete model.

## Identifier convention

Use hierarchical identifiers when the model becomes substantial:

```text
C1       Customer Management
C1.1     Customer Relationship Management
C1.1.1   Customer Contact Management
C1.1.2   Customer Preference Management
```

Identifiers stabilise cross-references even when names improve later.

Do not encode org ownership, product, location or system into the identifier.

## Large-enterprise expectation

For a large enterprise, the deliverable should be recoverable as a complete tree:

```text
GROUPING
  L1
    L2
      L3
      L3
    L2
      L3
      L3
```

A polished diagram may show only a slice at once, but the underlying model should not have hidden gaps simply because the visual became crowded.

## Small-enterprise simplification

A small or simple organisation should not manufacture L3 detail merely to resemble a reference framework.

Stop at L2 when:

- the L2 capability already maps cleanly to one coherent business responsibility;
- systems, controls, data and investment do not differ materially below it;
- further decomposition would mostly restate process steps;
- no current decision needs the extra distinction.

The model should be as deep as the decisions require, not as deep as the modelling tool permits.
