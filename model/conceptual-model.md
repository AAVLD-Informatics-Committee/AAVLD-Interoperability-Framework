# Conceptual model - working inventory

**Status:** Proposed pre-symposium inventory; cardinality and conformance are not
yet approved.

## Core entities

- Organization and laboratory
- Client or requesting party
- Animal, herd, flock, population, environment, or other testing subject
- Test or service offering
- Request and requested service
- Specimen and derived specimen
- Receipt, acknowledgement, and validation outcome
- Accession
- Performing and referral laboratory
- Observation, result, and report
- Correction, amendment, cancellation, or replacement
- Error, warning, and retry event

## Required relationship tests

The vertical slice must demonstrate that an implementer can determine:

- Who requested, received, and performed the work.
- Which offering and version were requested.
- Which subject and specimen the work concerns.
- How external request and specimen identifiers map to local accessions.
- Whether the exchange was received, accepted, rejected, or accepted with a
  warning.
- Which results are interim or final and who authorized them.
- What changed in a correction or amendment and what it replaces.
- Whether referral or subcontracted testing occurred.

## Computable representation

At least one pre-symposium representation will be machine-validatable. The
project will decide whether the first artifact is JSON Schema, FHIR Shorthand,
FHIR StructureDefinitions, or another bounded representation appropriate to the
vertical slice.
