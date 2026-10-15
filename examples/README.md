# Worked examples

The worked examples are evidence artefacts, not decorative illustrations.

This follows the same principle used in [`codebase-to-edd`](https://github.com/jonathanselby/codebase-to-edd): a method is more credible when another reader can inspect what went in, what was inferred, what was rejected and what remains uncertain.

`codebase-to-edd` pins real repository analyses to an exact source commit. Capability modelling rarely has an immutable codebase, so public-source examples use a dated source set instead: named public pages/reports, the report year where relevant, and a retrieval date.

## Example set

| Example | Basis | L1 capabilities | Selected L2 decompositions | Purpose |
|---|---|---:|---|---|
| [Northstar Equipment Hire](fictional-company/) | fictional source brief | 10 | 3 × 4 | demonstrate the method without external evidence dependencies |
| [Australia Post](australia-post/) | public corporate/service sources | 12 | 3 × 4 | test the method against a large logistics, retail-access and service network |
| [Sydney Water](sydney-water/) | public statutory/service sources | 12 | 3 × 4 | test the method against an infrastructure, utility and regulatory context |

The counts are **not** targets for real capability models. They are held within a deliberately narrow range here so the worked examples can be compared without one example operating at enterprise-domain scale and another at process-step scale.

See [`granularity-cross-check.md`](granularity-cross-check.md).

## Standard example package

Every worked example should contain the same six artefacts:

1. `README.md` — scope, source basis and modelling question;
2. `evidence.md` — what the supplied/public material actually supports, plus gaps;
3. `bad-first-draft.md` — plausible implementation-shaped labels and why they fail;
4. `corrected-model.md` — candidate L1 model plus selected L2 decompositions;
5. `capability-definitions.md` — scoped definitions for selected capabilities;
6. `review.md` — anti-pattern, granularity, evidence and uncertainty review.

This prevents a thin example from appearing equivalent to a fully worked one.

## Evidence rule

For public-source examples:

- source facts are **observed** from the named public material;
- the capability hierarchy is **architectural inference**, not an official capability model;
- absent internal detail is recorded as unknown rather than guessed;
- public product, programme, location, team or channel names may be used as evidence but are not automatically accepted as capabilities;
- source pages may change, so retrieval date and report year are recorded.

## Reproducibility rule

A reader should be able to recover:

```text
SOURCE SET
   |
   v
EVIDENCE EXTRACT
   |
   v
BAD / PLAUSIBLE FIRST DRAFT
   |
   v
ANTI-PATTERN + GRANULARITY REVIEW
   |
   v
CORRECTED CANDIDATE MODEL
   |
   v
SCOPED DEFINITIONS + OPEN QUESTIONS
```

The goal is not to prove that one taxonomy is uniquely correct. It is to make the modelling judgement inspectable.
