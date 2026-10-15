# Review — Australia Post

## Evidence review

The model is constrained to abilities supported by Australia Post's public description of its service, national networks, access obligations and operating scale.

It does not claim knowledge of internal capability ownership, systems, maturity or process decomposition.

## Anti-pattern corrections

- `Post Offices` -> implementation mapped to Retail Access Management.
- `Parcel Lockers` -> implementation mapped to Retail Access / Delivery & Collection capabilities.
- `Delivery Vehicles` -> assets mapped to transport/delivery capabilities.
- `MyPost Business` -> product/channel mapped to Customer Management and Service Portfolio Management.
- `Network Modernisation` -> change initiative mapped to affected capabilities.
- `Community Service Obligations` -> obligations mapped across relevant capabilities.

## Granularity review

The 12 L1 capabilities are enterprise-scale abilities.

The selected L2s decompose one L1 into four enduring management abilities. They do not descend to tasks such as `Scan Parcel`, `Load Vehicle` or `Open Post Office`.

## Boundary questions

Needs internal validation:

- Service Portfolio Management vs International Service Management;
- Transport Network Management vs Delivery & Collection Management;
- Retail Access Management vs Customer Management;
- whether processing/sortation merits an explicit L1 or sits within transport/network operation.

## Review outcome

**ACCEPT as a public-source worked candidate with explicit boundary questions.**

The taxonomy is not asserted as uniquely correct or official.
