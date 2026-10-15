# Granularity Cross-Check

This file exists to stop the worked examples drifting to different semantic scales.

## Common hierarchy

```text
LANDSCAPE GROUPING   navigation only
└── L1               broad enterprise ability
    └── L2           major enduring decomposition
        └── L3       elemental enduring business ability
```

## Cross-example comparison

| Level | Northstar Equipment Hire | Australia Post | Sydney Water |
|---|---|---|---|
| grouping | Operations & Assets | Network & Fulfilment | Assets & Infrastructure |
| L1 | Maintenance Management | Network Management | Asset Management |
| L2 | Maintenance Planning | Network Capacity Management | Asset Lifecycle Management |
| L3 | Preventive Maintenance Planning | Capacity Forecasting | Asset Renewal Management |

These labels are domain-specific, but the semantic scale is intended to be comparable.

## Horizontal test

At any one parent, siblings should be peers.

Good:

```text
Asset Management
├── Asset Strategy Management
├── Asset Lifecycle Management
├── Asset Performance Management
└── Asset Information Management
```

Bad:

```text
Asset Management
├── Asset Strategy Management
├── Replace Pump
├── SAP EAM
└── Western Sydney Team
```

The bad version mixes capability, task, application and organisation.

## Vertical test

Each child must be a narrower enduring ability of its parent.

Good:

```text
Asset Lifecycle Management
├── Asset Acquisition Management
├── Asset Maintenance Strategy Management
├── Asset Renewal Management
└── Asset Disposal Management
```

Bad:

```text
Asset Lifecycle Management
└── Customer Billing Management
```

## L3 stopping test

A candidate L3 is useful when the distinction is likely to change one or more of:

- accountability;
- application/system support;
- information concepts;
- controls/regulation;
- risk;
- supplier dependency;
- investment/change;
- performance measures.

If none change, the L3 split may be taxonomy for its own sake.

## Capability/process boundary

If the next decomposition naturally becomes a sequence of actions—`receive`, `validate`, `approve`, `route`, `send`, `inspect`, `reconcile`—the model is probably crossing into process/activity detail.

Do not create L4 merely to keep decomposing.

## Organisation-size caveat

Northstar is intentionally small. A complete L3 model would add little operating value, so L3 is demonstrated selectively.

Australia Post and Sydney Water are examples of organisational scale and complexity where a real internal enterprise capability model would normally be expected to reach L3 broadly. Public material, however, cannot support authoritative internal detail across every branch, so the examples show responsible L3 inference where evidence is strongest and retain explicit gaps elsewhere.
