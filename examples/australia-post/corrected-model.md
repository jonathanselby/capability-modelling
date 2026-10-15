# Corrected Candidate Capability Model — Australia Post

This is an architectural inference from the dated public source set, not an official Australia Post taxonomy.

## Level 1

```text
Customer Management
Service Portfolio Management
Item Acceptance Management
Transport Network Management
Delivery & Collection Management
Retail Access Management
Address & Delivery Point Management
International Service Management
Revenue Management
Partner & Supplier Management
Workforce Management
Enterprise Management
```

## Selected Level 2 decompositions

```text
Transport Network Management
├── Network Planning
├── Capacity Management
├── Transport Execution Management
└── Network Performance Management

Delivery & Collection Management
├── Delivery Planning
├── Delivery Execution Management
├── Collection Management
└── Delivery Exception Management

Retail Access Management
├── Access Network Planning
├── Service Point Management
├── Assisted Service Management
└── Self-Service Access Management
```

## Why these are at the chosen level

`Post Offices` and `Parcel Lockers` do not become sibling capabilities. They are implementation forms within the broader enduring ability to provide service access.

Likewise, `Delivery Vehicles` are assets used by Transport Network Management and Delivery & Collection Management rather than a business ability.

`Letters` and `Parcels` may be useful portfolio/product segment mappings, but the public evidence does not require separate enterprise L1 capability trees for each.

`Community Service Obligations` are obligations that constrain and measure multiple capabilities rather than a capability identity.
