# Worked examples

The worked examples are evidence artefacts, not decorative illustrations.

This follows the same principle used in [`codebase-to-edd`](https://github.com/jonathanselby/codebase-to-edd): a method is more credible when another reader can inspect what went in, what was inferred, what was rejected and what remains uncertain.

`codebase-to-edd` pins real repository analyses to an exact source commit. Capability modelling rarely has an immutable codebase, so public-source examples use a dated source set instead: named public pages/reports, report year where relevant, and retrieval date.

## Example set

| Example | Basis | Organisation type | Depth demonstrated |
|---|---|---|---|
| [Northstar Equipment Hire](fictional-company/) | fictional source brief | small/simple | complete L1/L2; selected L3 to show how to deepen only where useful |
| [Australia Post](australia-post/) | official public sources | large national enterprise | enterprise landscape plus L3 domain detail where public evidence supports inference |
| [Sydney Water](sydney-water/) | official public sources | large regulated utility | enterprise landscape plus L3 domain detail where public evidence supports inference |

The examples are kept at comparable semantic granularity. They are **not** forced to identical capability counts.

See [`granularity-cross-check.md`](granularity-cross-check.md).

## Standard example package

Every worked example contains:

1. `README.md` — scope, source basis and modelling question;
2. `evidence.md` — what the supplied/public material actually supports, plus gaps;
3. `bad-first-draft.md` — plausible implementation-shaped labels and why they fail;
4. `corrected-model.md` — candidate hierarchy and depth decision;
5. `capability-definitions.md` — scoped definitions for selected capabilities;
6. `review.md` — anti-pattern, granularity, evidence and uncertainty review;
7. `landscape.txt` — a visual ASCII capability landscape.

## Evidence rule

For public-source examples:

- source facts are **observed** from named public material;
- capability hierarchy is **architectural inference**, not an official model;
- absent internal detail is recorded as unknown rather than guessed;
- public product, programme, location, team or channel names may be evidence but are not automatically capabilities;
- source pages may change, so retrieval date/report year are recorded.

## Depth rule

### Large/complex organisations

The target method is complete L1–L3.

Public examples may not expose enough evidence to responsibly populate every branch at L3. In that case the example must identify the evidence gap rather than manufacture apparent completeness.

### Small/simple organisations

Full enterprise L3 is not expected. L3 should be used only where it reveals a distinction that materially changes ownership, systems, controls, information, risk, investment or another decision.

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
VISUAL LANDSCAPE + L3 DETAIL
   |
   v
SCOPED DEFINITIONS + OPEN QUESTIONS
```

The goal is not to prove one taxonomy uniquely correct. It is to make the modelling judgement inspectable.
