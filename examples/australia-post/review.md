# Review — Australia Post

## Evidence review

The model is constrained to abilities supported by Australia Post's public description of its service, national networks, access obligations and operating scale.

It does not claim knowledge of internal capability ownership, systems, maturity or process decomposition.

## Anti-pattern corrections

- `Post Offices` -> implementation mapped to Retail Access Management.
- `Parcel Lockers` -> implementation mapped to Retail Access Management and Delivery Management.
- `Delivery Vehicles` -> assets mapped to Transport Management and Delivery Management.
- `MyPost Business` -> product/channel mapped to Customer Management, Channel Management and Product & Service Management.
- `Network Modernisation` -> change initiative mapped to affected capabilities.
- `Community Service Obligations` -> obligations mapped across relevant capabilities.

## Granularity review

The 12 L1 capabilities are enterprise-scale abilities.

The selected L2s decompose L1 capabilities into enduring management abilities. They do not descend to tasks such as `Scan Parcel`, `Load Vehicle` or `Open Post Office`.

## Boundary questions

Needs internal validation:

- Product & Service Management vs Commercial Management;
- Network Management vs Transport Management vs Delivery Management;
- Consignment Management vs Delivery Management;
- Retail Access Management vs Customer Management;
- whether processing/sortation merits an explicit L1 or sits within Network Management.

## Review outcome

**ACCEPT as a public-source worked candidate with explicit boundary questions.**

The taxonomy is not asserted as uniquely correct or official.
