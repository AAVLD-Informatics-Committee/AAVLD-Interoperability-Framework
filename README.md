# AAVLD Interoperability Framework

This repository is the working home for development of the proposed AAVLD
Interoperability Framework for veterinary diagnostic laboratories.

> **Project status:** Pre-symposium working material. Content in this repository
> has not been approved as an AAVLD standard, accreditation requirement, or
> implementation mandate unless a release explicitly states otherwise.

## Purpose

The framework will define the common meaning, identifiers, workflows, exchange
behavior, and governance needed for laboratories and their partners to publish
services, submit diagnostic requests, acknowledge and accession work, return
results, manage corrections, and preserve traceability across organizational
boundaries.

The framework defines veterinary semantics before prescribing a transport or
product. HL7 FHIR is the first implementation-profile path to be mapped and
tested. It is not a mandatory implementation technology unless AAVLD later
approves a specific profile or conformance requirement.

## Initial deliverable

Before the October 15, 2026 symposium, the project will develop three practical
use cases and one synthetic, machine-validatable vertical slice:

`catalog -> order -> acknowledgement -> validation or rejection -> accession -> specimen -> interim result -> final report -> correction or amendment`

The work will include visible failure states, terminology alignment, FHIR
mapping, and documented veterinary gaps.

## Repository map

- `framework/` - integrated prose framework and status.
- `model/` - conceptual model and FHIR alignment.
- `decisions/` - accepted and tentative decision summaries.
- `examples/` - synthetic examples and validation artifacts.
- `meetings/` - public-safe agendas, working questions, and outcomes.
- `references/` - source classification and provenance.

## Governance and participation

Issues record work and decision requests. Pull requests contain proposed
changes. Repository merge approval, committee disposition, and formal AAVLD
publication approval are separate actions. See [GOVERNANCE.md](GOVERNANCE.md)
and [CONTRIBUTING.md](CONTRIBUTING.md).

External contributions will not be merged until contribution authority and
terms are confirmed. Do not submit real operational, client, owner, animal,
herd, accession, submitter, or production-system data. See
[DATA-SAFETY.md](DATA-SAFETY.md).

## Related AAVLD work

Accreditation-oriented guidance for validation, records, security, change
control, continuity, LIMS, and interfaces is developed separately in the
[AAVLD IT Guidance repository](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance).

## License

Original work in this repository is licensed under the
[Apache License 2.0](LICENSE), subject to confirmation by the appropriate AAVLD
authority. External material retains its own license, copyright, attribution,
and trademark requirements.
