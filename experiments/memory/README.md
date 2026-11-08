# Memory Reliability Research

## Initial research question
Why can a memory retrieval system find expected records while also returning candidates that fail one or more mandatory conditions?

## Working distinction
- **Candidate retrieval:** find records that may be relevant.
- **Constraint validation:** verify that each candidate satisfies every mandatory condition.
- **Relationship resolution:** identify links, corrections, and superseded records.
- **Evidence presentation:** provide provenance or report insufficient evidence.

High recall alone does not establish answer quality. Precision and the causes of false positives matter too.

## Proposed synthetic test dimensions
- required attributes combined with AND logic;
- synonyms within a single attribute;
- time ranges and event dates;
- context/property scope;
- insufficient or ambiguous information;
- correction chains and superseded records;
- source references and traceability.

## Status
This is a research brief. It does not claim that a specific component or architecture has been approved for production. Results should include test conditions and evidence.
