# Contributing

This repository is in its pre-symposium initialization stage.

## Current contribution status

External contributions may be discussed in issues, but they will not be merged
until AAVLD confirms contribution authority and terms. Participation does not
by itself confer decision or publication authority.

## Working method

- Search existing issues before proposing new work.
- Use a work-item issue for a bounded deliverable and a decision-request issue
  when committee direction is needed.
- Link substantive pull requests to an issue.
- Classify each substantive statement and identify its conformance subject,
  source IDs, governing decision, and verification approach.
- Identify affected framework, model, FHIR, terminology, example, and
  compatibility concerns.
- Keep editorial review, repository merge approval, committee disposition, and
  formal AAVLD approval distinct.

## Drafting and conformance checklist

- Apply the proposed
  [drafting conventions](framework/drafting-conventions.md), including one
  principal requirement per statement and consistent `shall`, `should`, `may`,
  and `can` usage.
- Keep framework requirements technology-neutral unless a recorded decision
  defines an implementation-profile constraint.
- State FHIR and dependency versions for computable artifacts.
- Define the actor behavior represented by FHIR `mustSupport`; the flag alone is
  not a complete conformance statement.
- Mark examples, notes, rationales, and unresolved issues as informative.
- Use `EXAMPLE-...` identifiers for pre-symposium illustrations; stable
  `AAVLD-IF-...` identifiers begin with Working Draft 0.1.

## Data and source rules

- Use synthetic examples only.
- Do not submit private calendar details or personal contact information.
- Do not copy external standards, terminologies, schemas, or vendor material
  unless redistribution is permitted.
- Identify the source and applicable license for contributed material.
- Do not imply endorsement by AAVLD, HL7, a laboratory, or a vendor.

See [DATA-SAFETY.md](DATA-SAFETY.md), the
[source register](references/source-register.md), and the
[source classification policy](references/source-classification.md).
