# Capability Modelling Anti-Patterns

A capability model usually goes wrong by importing another architectural view into the capability layer.

## 1. Org-chart leakage

Examples:

- Sales Team
- Finance Department
- APAC Operations
- Sydney Service Desk

Why it fails: organisational structure changes while the underlying business ability may remain.

Ask instead: what enduring ability does this organisational unit provide?

## 2. Application leakage

Examples:

- Salesforce
- SAP
- ServiceNow
- CRM Platform

Why it fails: software enables capabilities but is not itself a business capability.

Ask instead: what business ability would still be required if the application were replaced?

## 3. Vendor leakage

Examples:

- Microsoft 365 Management
- AWS Operations
- Workday Administration

Why it fails: it ties capability identity to a supplier or product decision.

## 4. Process-step leakage

Examples:

- Send Invoice
- Approve Refund
- Create Purchase Order
- Schedule Technician

Why it fails: these are activities inside an ability rather than enduring abilities at the same modelling level.

## 5. Programme leakage

Examples:

- Digital Transformation
- ERP Replacement
- Cloud Migration
- Customer 360 Programme

Why it fails: programmes are temporary change vehicles. The capability should remain after the programme closes.

## 6. Location leakage

Examples:

- Sydney Distribution
- Melbourne Support
- Offshore Processing

Why it fails: location is a deployment/organisation attribute, not capability identity.

## 7. Outcome-as-capability

Examples:

- Customer Satisfaction
- Revenue Growth
- Operational Excellence

Why it fails: these are outcomes or aspirations, not abilities.

Ask what abilities contribute to the outcome.

## 8. Object-without-ability

Examples:

- Customers
- Suppliers
- Contracts
- Assets

Why it fails: an information/business object is not automatically a capability.

`Customer Management` may be meaningful; `Customer` usually is not.

## 9. Category-without-boundary

Examples:

- Operations
- Management
- Digital
- Corporate

Why it fails: the label is too broad to support analysis without a strong definition and decomposition.

## 10. Mixed granularity

Example sibling list:

```text
Customer Management
Send Renewal Email
Enterprise Operations
Revenue Management
```

Why it fails: the items cannot be compared meaningfully because they occupy different conceptual levels.

## 11. Definition tautology

Weak:

> Contract Management is the capability to manage contracts.

A definition should clarify purpose and boundary, not repeat the label.

## 12. Generated-authority failure

An AI-generated capability map is a candidate model, not discovered truth.

Red flags:

- capability names appear without evidence;
- missing business context is silently filled with generic industry knowledge;
- familiar reference-model terms are presented as mandatory;
- the model does not identify uncertainty or assumptions.

The correct response is review, not confidence.
