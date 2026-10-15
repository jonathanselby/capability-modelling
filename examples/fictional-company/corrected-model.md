# Corrected Capability Model

Starting from Northstar Equipment Hire's purpose and responsibilities rather than its current structure produces a more stable model.

Northstar is deliberately small enough that **full L3 across the entire enterprise would not normally be necessary in practice**. This example nevertheless expands selected branches to L3 to demonstrate how the method scales.

## Landscape groupings

```text
CUSTOMER & COMMERCIAL
OPERATIONS & ASSETS
ENTERPRISE SUPPORT
```

## Enterprise landscape — L1 / L2

```text
+-----------------------------------------------------------------------+
| CUSTOMER & COMMERCIAL                                                 |
|                                                                       |
|  Customer Management                                                  |
|   ├─ Customer Acquisition Management                                  |
|   ├─ Customer Relationship Management                                 |
|   └─ Customer Service Management                                      |
|                                                                       |
|  Rental Agreement Management                                          |
|   ├─ Rental Quotation Management                                      |
|   ├─ Rental Contract Management                                       |
|   ├─ Rental Extension Management                                      |
|   └─ Rental Closure Management                                        |
|                                                                       |
|  Revenue Management                                                   |
|   ├─ Pricing Management                                               |
|   ├─ Billing Management                                               |
|   ├─ Payment Management                                               |
|   └─ Revenue Assurance                                                |
+-----------------------------------------------------------------------+
| OPERATIONS & ASSETS                                                   |
|                                                                       |
|  Fleet Management                                                     |
|   ├─ Fleet Planning                                                   |
|   ├─ Fleet Acquisition                                                |
|   ├─ Fleet Disposition                                                |
|   └─ Fleet Performance Management                                     |
|                                                                       |
|  Equipment Availability Management                                    |
|   ├─ Availability Determination                                       |
|   ├─ Capacity Reservation                                             |
|   ├─ Commitment Management                                            |
|   └─ Availability Exception Management                                |
|                                                                       |
|  Fulfilment Management                                                |
|   ├─ Collection Management                                            |
|   ├─ Delivery Management                                              |
|   ├─ Return Management                                                |
|   └─ Fulfilment Exception Management                                  |
|                                                                       |
|  Maintenance Management                                               |
|   ├─ Maintenance Planning                                             |
|   ├─ Maintenance Execution                                            |
|   ├─ Serviceability Management                                        |
|   └─ Maintenance Parts Management                                     |
+-----------------------------------------------------------------------+
| ENTERPRISE SUPPORT                                                    |
|                                                                       |
|  Supplier Management                                                  |
|   ├─ Supplier Selection                                               |
|   ├─ Supplier Contract Management                                     |
|   └─ Supplier Performance Management                                  |
|                                                                       |
|  Workforce Management                                                 |
|   ├─ Workforce Planning                                               |
|   ├─ Workforce Administration                                         |
|   └─ Workforce Capability Management                                  |
|                                                                       |
|  Enterprise Management                                                |
|   ├─ Strategy Management                                              |
|   ├─ Risk & Compliance Management                                     |
|   ├─ Financial Management                                             |
|   └─ Technology Management                                            |
+-----------------------------------------------------------------------+
```

## Detailed hierarchy — selected L3

### Maintenance Management

```text
Maintenance Management
├── Maintenance Planning
│   ├── Preventive Maintenance Planning
│   ├── Corrective Maintenance Planning
│   └── Maintenance Scheduling
├── Maintenance Execution
│   ├── Work Order Management
│   ├── Maintenance Work Coordination
│   └── Maintenance Completion Management
├── Serviceability Management
│   ├── Serviceability Assessment
│   ├── Defect Management
│   └── Return-to-Service Management
└── Maintenance Parts Management
    ├── Parts Demand Management
    ├── Parts Availability Management
    └── Parts Consumption Management
```

### Rental Agreement Management

```text
Rental Agreement Management
├── Rental Quotation Management
│   ├── Quote Preparation
│   ├── Quote Approval Management
│   └── Quote Validity Management
├── Rental Contract Management
│   ├── Contract Establishment
│   ├── Contract Terms Management
│   └── Contract Variation Management
├── Rental Extension Management
│   ├── Extension Eligibility Management
│   ├── Extension Pricing Management
│   └── Extension Confirmation Management
└── Rental Closure Management
    ├── Return Condition Assessment
    ├── Closure Charge Management
    └── Contract Completion Management
```

### Fleet Management

```text
Fleet Management
├── Fleet Planning
│   ├── Fleet Demand Planning
│   ├── Fleet Mix Planning
│   └── Fleet Capacity Planning
├── Fleet Acquisition
│   ├── Acquisition Requirement Management
│   ├── Acquisition Evaluation
│   └── Fleet Onboarding Management
├── Fleet Disposition
│   ├── Disposal Candidate Management
│   ├── Disposal Channel Management
│   └── Fleet Retirement Management
└── Fleet Performance Management
    ├── Utilisation Management
    ├── Lifecycle Cost Management
    └── Fleet Reliability Management
```

The L3 labels remain abilities. If decomposition continued into steps such as `inspect machine`, `send quote` or `approve invoice`, that would be process/activity modelling rather than capability modelling.

## Why this is stronger

- `Sydney Sales` becomes evidence for `Customer Management`, not a capability.
- `Online Booking Portal` is mapped to capabilities later.
- `Workshop` becomes an implementation location supporting `Maintenance Management`.
- `Invoice Processing` sits below broader `Revenue Management` and would normally be represented in process detail.
- `Digital Transformation` and `ERP Replacement` remain change initiatives mapped to affected capabilities.

The model is illustrative, not an industry reference taxonomy.
