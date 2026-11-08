# Memory Retrieval Evaluation — 8 November 2026

## Why we ran this evaluation

Tuti is an assistant being developed around practical hospitality workflows. A useful assistant must not merely find records that look related; it must select records that satisfy all mandatory conditions in the user's question, preserve context boundaries, and make uncertainty visible.

This note shares a sanitized summary of an internal evaluation so other developers can critique our approach.

## Observed result

In the OS-013 evaluation:

- 14 cases were evaluated.
- 1 case fully conformed to the test contract.
- The retrieval process recovered all expected record IDs.
- Candidate precision was reported as 37.3%.
- The run reported no results outside the requested scope or time period.

These figures describe one project-specific test run. They are not a public benchmark, and they should not be generalized to other systems or datasets. The detailed private test fixtures and operational implementation are not published here.

## What this suggests — and what it does not

The result suggests a gap between candidate retrieval and candidate validation: expected records can be found while additional candidates are also returned.

It does **not**, by itself, prove which subsystem caused each false positive or establish that a particular architecture is the solution. Further inspection and controlled experiments are needed.

## Questions for the community

1. Should candidate generation and strict constraint validation be separate stages?
2. How do you enforce AND logic across mandatory attributes while allowing synonyms within one attribute?
3. Which constraints should be applied in structured storage queries rather than semantic ranking?
4. How do you model corrections and superseded memories without erasing history?
5. What is a practical way to measure precision, recall, and contract-level correctness on small datasets?
6. How should a system report insufficient evidence rather than guessing?

## Our current working direction

We are evaluating an incremental approach: preserve existing components, audit what is actually active, and validate one capability at a time before integrating further functionality. No production architecture change is implied by this note.

## Invitation

If you have built memory, search, retrieval, RAG, or agent systems, we would value concrete examples, papers, design patterns, and critical feedback. Please join the discussion in [GitHub Issue #1](https://github.com/osiasfjunior-crypto/tuti-lab-community/issues/1).

Portuguese contributions are welcome too.
