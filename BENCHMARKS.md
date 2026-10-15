# Comparator Benchmark

This method is intentionally lightweight, but it should be capable of reaching the depth expected of serious enterprise capability modelling.

The benchmark is not to copy another framework. It is to understand what mature reference models demonstrate about hierarchy, completeness, notation and usable granularity.

## BIAN

BIAN is the strongest direct comparator because it maintains a banking Business Capability Model alongside its Service Landscape.

BIAN Release 9 deliberately limited its Business Capability Model to **three capability levels** and reported:

- 5 high-level groupings;
- 40 Level 1 capabilities;
- 183 Level 2 capabilities;
- 345 Level 3 capabilities.

BIAN also stated that the model had been decomposed to Level 3 in most cases. Later BIAN material distinguishes the business capability hierarchy from elemental Service Domains and notes that business capabilities often align with service-domain granularity around Level 2 or Level 3.

Sources:

- BIAN Release 9.0 notes: https://bian.org/wp-content/uploads/2020/10/BIAN-v9.0-Release-Notes.pdf
- BIAN Business Capability Model / Service Landscape alignment paper: https://bian.org/wp-content/uploads/2023/08/BIAN-BCM-Relationship-with-BIAN-Service-Landscape-Final.pdf
- current BIAN Service Landscape: https://bian.org/deliverables/service-landscape/

### Lesson for this repository

Three levels is a defensible enterprise default. A high-level grouping may sit above L1 for navigation, but it is not another capability level.

```text
LANDSCAPE GROUPING
└── L1 capability
    └── L2 capability
        └── L3 capability
```

## APQC Process Classification Framework

APQC is not a capability model, so its taxonomy must not be copied into capability identity. It is useful as a comparator for **decomposition discipline**.

APQC's Process Classification Framework decomposes work through five levels: Category, Process Group, Process, Activity and Task. APQC also distinguishes process from capability: a process is a sequence of activities producing an output; a capability is broader and includes the means required to perform work.

Sources:

- https://www.apqc.org/process-frameworks
- https://www.apqc.org/How-Can-Organizations-Classify-and-Organize-Their-Processes-Using-a-Common-Framework

### Lesson for this repository

A robust model should be capable of systematic decomposition without accidentally turning L3 into process steps. Capability modelling stops at an enduring ability; process modelling continues into sequence, activity and task.

## ArchiMate / The Open Group

ArchiMate provides an enterprise-architecture notation that includes capability in its Strategy domain and separates capabilities from business processes, organisational structure, applications and technology.

Source:

- https://www.opengroup.org/archimate-forum/archimate-overview

### Lesson for this repository

The capability map should be visually explicit and should remain separable from implementation views. A capability can later be related to organisation, process, application, information and technology without embedding those concerns in the capability identity.

## Position adopted here

The repository therefore uses:

| Layer | Meaning |
|---|---|
| Landscape grouping | visual/navigation grouping only; not a capability level |
| L1 | broad enterprise capability |
| L2 | major enduring decomposition of an L1 capability |
| L3 | more elemental enduring business ability; still not a process step |

### Depth by organisation size

**Large / complex enterprise**  
A complete three-level model is the normal target. L3 is where materially different ownership, systems, controls, information, investment and risk often become visible.

**Medium organisation**  
Complete L1 and L2, then use L3 where the business question requires it. Full L3 may still be appropriate for regulated, asset-intensive or operationally complex areas.

**Small / simple organisation**  
L1 and L2 are usually sufficient. Decomposing the whole enterprise to L3 can create taxonomy maintenance without a corresponding decision benefit.

The test is not organisational headcount alone. It is whether the additional decomposition reveals distinctions that change a decision.
