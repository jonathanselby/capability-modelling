# Corrected Candidate Capability Model — Australia Post

This is an **independent architectural inference from public sources**, not Australia Post's official capability model.

Because Australia Post is a large, complex national enterprise, this example uses a full three-level structure.

## Landscape groupings

```text
CUSTOMER & MARKET
PRODUCT & COMMERCIAL
NETWORK & FULFILMENT
ENTERPRISE ENABLEMENT
```

## Enterprise landscape — L1 / L2

```text
+-----------------------------------------------------------------------+
| CUSTOMER & MARKET                                                     |
|                                                                       |
| Customer Management                                                   |
|  ├─ Customer Acquisition Management                                   |
|  ├─ Customer Relationship Management                                  |
|  ├─ Customer Service Management                                       |
|  └─ Customer Insight Management                                       |
|                                                                       |
| Channel Management                                                    |
|  ├─ Retail Access Management                                          |
|  ├─ Digital Channel Management                                        |
|  ├─ Business Channel Management                                       |
|  └─ Channel Performance Management                                    |
+-----------------------------------------------------------------------+
| PRODUCT & COMMERCIAL                                                  |
|                                                                       |
| Product & Service Management                                          |
|  ├─ Parcel Service Management                                         |
|  ├─ Letter Service Management                                         |
|  ├─ Retail Service Management                                         |
|  └─ International Service Management                                  |
|                                                                       |
| Commercial Management                                                 |
|  ├─ Pricing Management                                                |
|  ├─ Contract Management                                               |
|  ├─ Revenue Management                                                |
|  └─ Commercial Performance Management                                 |
+-----------------------------------------------------------------------+
| NETWORK & FULFILMENT                                                  |
|                                                                       |
| Network Management                                                    |
|  ├─ Network Planning                                                  |
|  ├─ Network Capacity Management                                       |
|  ├─ Network Operations Management                                     |
|  └─ Network Performance Management                                    |
|                                                                       |
| Consignment Management                                                |
|  ├─ Lodgement Management                                              |
|  ├─ Item Identification Management                                    |
|  ├─ Consignment Status Management                                     |
|  └─ Delivery Commitment Management                                    |
|                                                                       |
| Transport Management                                                  |
|  ├─ Transport Planning                                                |
|  ├─ Linehaul Management                                               |
|  ├─ Local Transport Management                                        |
|  └─ Transport Exception Management                                    |
|                                                                       |
| Delivery Management                                                   |
|  ├─ Delivery Planning                                                 |
|  ├─ Delivery Execution Management                                     |
|  ├─ Delivery Exception Management                                     |
|  └─ Delivery Confirmation Management                                  |
+-----------------------------------------------------------------------+
| ENTERPRISE ENABLEMENT                                                 |
|                                                                       |
| Workforce Management                                                  |
| Supplier Management                                                   |
| Asset Management                                                      |
| Risk & Compliance Management                                          |
+-----------------------------------------------------------------------+
```

## Detailed hierarchy — L3 examples

### Consignment Management

```text
Consignment Management
├── Lodgement Management
│   ├── Lodgement Acceptance Management
│   ├── Lodgement Validation Management
│   └── Lodgement Exception Management
├── Item Identification Management
│   ├── Identifier Assignment Management
│   ├── Label/Data Association Management
│   └── Identification Exception Management
├── Consignment Status Management
│   ├── Tracking Event Management
│   ├── Status Visibility Management
│   └── Status Exception Management
└── Delivery Commitment Management
    ├── Service Promise Management
    ├── Delivery Window Management
    └── Commitment Exception Management
```

### Network Management

```text
Network Management
├── Network Planning
│   ├── Network Footprint Planning
│   ├── Route Network Planning
│   └── Facility Role Planning
├── Network Capacity Management
│   ├── Capacity Forecasting
│   ├── Capacity Allocation
│   └── Constraint Management
├── Network Operations Management
│   ├── Facility Operations Management
│   ├── Network Flow Management
│   └── Operational Disruption Management
└── Network Performance Management
    ├── Throughput Performance Management
    ├── Service Performance Management
    └── Network Cost Performance Management
```

### Channel Management

```text
Channel Management
├── Retail Access Management
│   ├── Retail Location Portfolio Management
│   ├── Retail Service Availability Management
│   └── Retail Access Performance Management
├── Digital Channel Management
│   ├── Digital Service Portfolio Management
│   ├── Digital Access Management
│   └── Digital Channel Performance Management
├── Business Channel Management
│   ├── Business Access Management
│   ├── Account Service Channel Management
│   └── Business Channel Performance Management
└── Channel Performance Management
    ├── Channel Demand Management
    ├── Channel Service Performance Management
    └── Channel Economics Management
```

The complete example uses L3 to demonstrate depth, but the hierarchy remains candidate architecture. Public sources do not expose enough internal information to claim authoritative ownership or system alignment.
