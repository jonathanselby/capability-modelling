# Corrected Capability Model

Starting from Northstar Equipment Hire's purpose and responsibilities rather than its current structure produces a more stable model.

## Level 1

```text
Customer Management
Fleet Management
Equipment Availability Management
Rental Agreement Management
Fulfilment Management
Maintenance Management
Revenue Management
Supplier Management
Workforce Management
Enterprise Management
```

These are illustrative, not authoritative.

## Why this is stronger

### `Sydney Sales` -> `Customer Management`

The location and team structure disappear. Customer acquisition, relationship and account needs remain even if sales is reorganised or moved.

### `Online Booking Portal` -> mapped later

The portal is not renamed into a capability. It would map to one or more capabilities such as Customer Management, Equipment Availability Management and Rental Agreement Management.

### `Fleet Operations Team` -> `Fleet Management`

The enduring ability survives team restructuring.

### `Workshop` -> `Maintenance Management`

The physical workshop is one implementation location. The enduring need is to maintain equipment in serviceable condition.

### `Invoice Processing` -> `Revenue Management`

Invoice processing is one process within the broader ability to calculate, collect and account for revenue.

### `Digital Transformation` -> mapped as change

The programme changes capabilities but is not a capability itself.

### `Microsoft 365` -> mapped as technology

A product can enable Workforce Management or Enterprise Management without defining either capability.

### `Equipment Delivery` -> `Fulfilment Management`

Delivery is part of fulfilling a rental commitment. A different operating model could use customer collection without removing the need for fulfilment.

### `Supplier Contracts` -> `Supplier Management`

Contracts are important artefacts within the broader ability to establish and govern supplier relationships.

### `ERP Replacement` -> mapped as change

The programme should map to the capabilities it affects, not sit inside the capability hierarchy.

## Example second level

A selected decomposition might be:

```text
Fleet Management
├── Fleet Planning
├── Fleet Acquisition
├── Fleet Disposition
└── Fleet Performance Management

Maintenance Management
├── Maintenance Planning
├── Maintenance Execution
├── Serviceability Management
└── Maintenance Parts Management

Rental Agreement Management
├── Rental Quotation Management
├── Rental Contract Management
├── Rental Extension Management
└── Rental Closure Management
```

This decomposition should be driven by useful distinctions, not by a target number of boxes.

## Separate mappings

Once the capability model is stable, Northstar can map today's implementation around it:

```text
Maintenance Management
    +--> Fleet Operations Team
    +--> Sydney Workshop
    +--> maintenance module in ERP
    +--> maintenance processes
    +--> parts suppliers
    +--> ERP Replacement programme
```

The capability remains stable while these mappings can change independently.
