# Bad First Draft

This is deliberately wrong.

A workshop at fictional Northstar Equipment Hire produces the following list:

```text
Sydney Sales
Online Booking Portal
Fleet Operations Team
Workshop
Invoice Processing
Customer Service
Digital Transformation
Microsoft 365
Equipment Delivery
Supplier Contracts
Branch Operations
ERP Replacement
```

The list feels plausible because every item is real to the organisation. But it mixes several architectural views.

| Candidate | What it actually describes | Problem |
|---|---|---|
| Sydney Sales | organisation + location | would change with structure/location |
| Online Booking Portal | application/channel | technology implementation |
| Fleet Operations Team | organisation | team, not enduring ability |
| Workshop | location/function shorthand | unclear capability boundary |
| Invoice Processing | process/activity | too implementation/process specific |
| Customer Service | potentially valid but ambiguous | needs definition and scope |
| Digital Transformation | programme | temporary change activity |
| Microsoft 365 | vendor/product | technology implementation |
| Equipment Delivery | potentially process or capability | needs level/boundary test |
| Supplier Contracts | business object/process shorthand | does not yet define an ability |
| Branch Operations | organisational/operating structure | likely too structure-dependent |
| ERP Replacement | programme | temporary change activity |

## What to do next

Do not simply rename each row until it sounds more architectural.

Return to Northstar's purpose and responsibilities and ask what enduring abilities must exist regardless of teams, locations, products and programmes.
