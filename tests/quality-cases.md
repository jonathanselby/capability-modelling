# Capability Quality Cases

These are semantic review cases, not automated unit tests.

## Case 1 — application name

Candidate: `Salesforce`

**Expected:** REMOVE as capability. Map the application later to capabilities it enables.

## Case 2 — team name

Candidate: `Sydney Sales`

**Expected:** REMOVE or REVISE. Geography and current organisation structure should not define the capability.

## Case 3 — broad enduring ability

Candidate: `Customer Management`

**Expected:** plausible L1 where the scope is enterprise-wide customer capability.

## Case 4 — meaningful L2

Parent: `Customer Management`  
Candidate child: `Customer Relationship Management`

**Expected:** plausible L2 if it describes an enduring subset of the parent and is distinct from sibling abilities such as Customer Service Management.

## Case 5 — elemental L3

Parent: `Customer Relationship Management`  
Candidate child: `Customer Preference Management`

**Expected:** plausible L3 if customer preferences are a materially distinct business responsibility with separate information, controls or system support.

## Case 6 — process step masquerading as L3

Parent: `Rental Agreement Management`  
Candidate child: `Send Contract Email`

**Expected:** REMOVE from capability hierarchy. This is activity/task detail.

## Case 7 — programme

Candidate: `ERP Replacement`

**Expected:** REMOVE as capability. Map the programme to impacted capabilities.

## Case 8 — sibling mismatch

```text
Customer Management
Send Renewal Email
Enterprise Management
```

**Expected:** FAIL granularity review. These labels operate at materially different scales.

## Case 9 — parent/child mismatch

```text
Customer Management
└── Finance Management
```

**Expected:** FAIL vertical review. The child does not decompose the parent.

## Case 10 — ambiguous terminology

Candidate: `Customer Account Management`

**Expected:** NEEDS EVIDENCE. The label could describe an enduring capability, a team or a process depending on context.

## Case 11 — small organisation stopping at L2

A ten-person professional-services firm has `Client Management -> Client Relationship Management`, with one owner, one CRM, one policy set and no material lower-level distinctions.

**Expected:** ACCEPT stopping at L2. L3 would likely add maintenance without decision value.

## Case 12 — large enterprise needs L3

A national utility has `Asset Management -> Asset Lifecycle Management`, but acquisition, maintenance strategy, renewal and disposal have different systems, governance, investment pools and controls.

**Expected:** SPLIT to L3. The L2 label hides distinctions that matter architecturally.
