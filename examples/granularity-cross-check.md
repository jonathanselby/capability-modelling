# Granularity Cross-Check

The examples use different industries but should demonstrate the method at comparable architectural scales.

## Cross-example control

| Level | Northstar Equipment Hire | Australia Post | Sydney Water |
|---|---|---|---|
| L1 scale | enterprise-wide enduring ability | enterprise-wide enduring ability | enterprise-wide enduring ability |
| L1 count | 10 | 12 | 12 |
| selected L2 pattern | 3 parents × 4 children | 3 parents × 4 children | 3 parents × 4 children |
| L2 scale | enduring decomposition of one L1 | enduring decomposition of one L1 | enduring decomposition of one L1 |
| process steps at L1/L2? | no | no | no |
| systems/vendors at L1/L2? | no | no | no |
| teams/locations at L1/L2? | no | no | no |

The counts are an **example-design control**, not a modelling rule. A real organisation may legitimately require a different number of capabilities.

## Comparable L1 examples

```text
Northstar          Australia Post            Sydney Water
---------          --------------            ------------
Customer Mgmt      Customer Mgmt             Customer Mgmt
Fleet Mgmt         Transport Network Mgmt    Network & Asset Mgmt
Fulfilment Mgmt    Delivery & Collection     Water Supply Mgmt
Revenue Mgmt       Revenue Mgmt              Revenue Mgmt
Supplier Mgmt      Partner & Supplier Mgmt   Supplier & Partner Mgmt
Enterprise Mgmt    Enterprise Mgmt           Enterprise Mgmt
```

The names are not intended to align one-for-one. The comparison tests **scale**, not taxonomy reuse.

## L2 test

Good L2 candidates answer:

> What narrower enduring abilities make this L1 capability possible?

They should not answer:

> What steps do people perform today?

For example:

```text
Network & Asset Management
├── Asset Planning
├── Asset Maintenance Management
├── Asset Renewal Management
└── Asset Performance Management
```

is at a different semantic level from:

```text
Network & Asset Management
├── Inspect Pump
├── Raise Work Order
├── Approve Contractor
└── Close Job
```

The second structure is a process/task decomposition and belongs in a different model.

## When to move a candidate between levels

Move a capability when comparison with siblings exposes a material scale mismatch.

Examples:

- `Customer Management` beside `Send Invoice` -> move/recast `Send Invoice` beneath Revenue Management or process modelling;
- `Enterprise Management` beside `Parcel Locker Management` -> map the locker as implementation and remove it from the capability hierarchy;
- `Water Supply Management` beside `Reservoir Inspection` -> treat inspection as process/maintenance activity, not L1/L2 capability.

## Conclusion

Granularity is not proved by box count. It is established by the semantic scale of siblings, explicit definitions and resistance to implementation leakage.
