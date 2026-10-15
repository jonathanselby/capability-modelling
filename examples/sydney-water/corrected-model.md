# Corrected Candidate Capability Model — Sydney Water

This is an **independent architectural inference from public sources**, not Sydney Water's official capability model.

Sydney Water is a large, regulated and asset-intensive utility, so a three-level model is appropriate.

## Landscape groupings

```text
CUSTOMER & SERVICE
WATER & RESOURCE OPERATIONS
ASSETS & INFRASTRUCTURE
ENTERPRISE & REGULATION
```

## Enterprise landscape — L1 / L2

```text
+-----------------------------------------------------------------------+
| CUSTOMER & SERVICE                                                    |
|                                                                       |
| Customer Management                                                   |
|  ├─ Customer Account Management                                       |
|  ├─ Customer Service Management                                       |
|  ├─ Customer Billing Management                                       |
|  └─ Customer Communication Management                                 |
|                                                                       |
| Service Commitment Management                                         |
|  ├─ Service Standard Management                                       |
|  ├─ Service Interruption Management                                   |
|  ├─ Customer Impact Management                                        |
|  └─ Service Performance Management                                    |
+-----------------------------------------------------------------------+
| WATER & RESOURCE OPERATIONS                                           |
|                                                                       |
| Water Supply Management                                               |
|  ├─ Water Source Interface Management                                 |
|  ├─ Water Treatment Management                                        |
|  ├─ Water Distribution Management                                     |
|  └─ Water Quality Management                                          |
|                                                                       |
| Wastewater Management                                                 |
|  ├─ Wastewater Collection Management                                  |
|  ├─ Wastewater Treatment Management                                   |
|  ├─ Recycled Water Management                                         |
|  └─ Wastewater Quality Management                                     |
|                                                                       |
| Stormwater Management                                                 |
|  ├─ Stormwater Network Management                                     |
|  ├─ Stormwater Flow Management                                        |
|  ├─ Stormwater Quality Management                                     |
|  └─ Stormwater Incident Management                                    |
|                                                                       |
| Resource & Environment Management                                     |
|  ├─ Water Conservation Management                                     |
|  ├─ Environmental Impact Management                                   |
|  ├─ Resource Recovery Management                                      |
|  └─ Catchment Interface Management                                    |
+-----------------------------------------------------------------------+
| ASSETS & INFRASTRUCTURE                                               |
|                                                                       |
| Asset Management                                                      |
|  ├─ Asset Strategy Management                                         |
|  ├─ Asset Lifecycle Management                                        |
|  ├─ Asset Performance Management                                      |
|  └─ Asset Information Management                                      |
|                                                                       |
| Infrastructure Delivery Management                                    |
|  ├─ Infrastructure Planning                                           |
|  ├─ Capital Delivery Management                                       |
|  ├─ Commissioning Management                                          |
|  └─ Delivery Assurance                                                |
|                                                                       |
| Operational Resilience Management                                     |
|  ├─ Continuity Planning                                               |
|  ├─ Incident Management                                               |
|  ├─ Emergency Response Management                                     |
|  └─ Recovery Management                                               |
+-----------------------------------------------------------------------+
| ENTERPRISE & REGULATION                                               |
|                                                                       |
| Regulatory & Compliance Management                                    |
| Risk Management                                                       |
| Workforce Management                                                  |
| Supplier Management                                                   |
| Enterprise Management                                                 |
+-----------------------------------------------------------------------+
```

## Detailed hierarchy — L3 examples

### Asset Management

```text
Asset Management
├── Asset Strategy Management
│   ├── Asset Portfolio Strategy Management
│   ├── Asset Service Strategy Management
│   └── Asset Investment Strategy Management
├── Asset Lifecycle Management
│   ├── Asset Acquisition Management
│   ├── Asset Maintenance Strategy Management
│   ├── Asset Renewal Management
│   └── Asset Disposal Management
├── Asset Performance Management
│   ├── Asset Condition Management
│   ├── Asset Reliability Management
│   └── Asset Criticality Management
└── Asset Information Management
    ├── Asset Register Management
    ├── Asset Configuration Information Management
    └── Asset History Management
```

### Water Supply Management

```text
Water Supply Management
├── Water Source Interface Management
│   ├── Source Availability Management
│   ├── Source Supply Coordination
│   └── Source Constraint Management
├── Water Treatment Management
│   ├── Treatment Capacity Management
│   ├── Treatment Performance Management
│   └── Treatment Exception Management
├── Water Distribution Management
│   ├── Distribution Capacity Management
│   ├── Distribution Pressure Management
│   └── Distribution Flow Management
└── Water Quality Management
    ├── Water Quality Monitoring Management
    ├── Water Quality Compliance Management
    └── Water Quality Incident Management
```

### Operational Resilience Management

```text
Operational Resilience Management
├── Continuity Planning
│   ├── Critical Service Identification
│   ├── Continuity Strategy Management
│   └── Continuity Readiness Management
├── Incident Management
│   ├── Incident Detection Management
│   ├── Incident Coordination Management
│   └── Incident Escalation Management
├── Emergency Response Management
│   ├── Emergency Mobilisation Management
│   ├── Emergency Stakeholder Coordination
│   └── Emergency Resource Management
└── Recovery Management
    ├── Service Restoration Management
    ├── Recovery Prioritisation Management
    └── Post-Incident Recovery Management
```

L3 is warranted here because asset classes, service obligations, controls, operational systems and investment decisions differ materially below L2.
