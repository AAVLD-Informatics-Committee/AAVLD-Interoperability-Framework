# Decision log

This log summarizes decisions without replacing the evidence and discussion in
the linked GitHub issue.

## IF-001 - Initial repository license

| Field | Value |
| --- | --- |
| Status | Project setup decision; pending confirmation by the appropriate committee or AAVLD authority |
| Date | 2026-08-26 |
| Decision | License original repository framework text, schemas, examples, and code under Apache License 2.0. |
| Rationale | Apache-2.0 is a widely used permissive license for open, implementable specification projects and includes an express patent grant. A single license reduces ambiguity across prose and computable artifacts. |
| Boundary | External material retains its original license, attribution, copyright, and trademark requirements. |
| Source issue | [#2 Approve governance, licensing, contribution, and release rules](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/2) |
| Affected artifacts | `LICENSE`, `README.md`, `CONTRIBUTING.md`, and future original repository content. |
| Decision authority | Project setup approved; committee/AAVLD ratification to be recorded if required. |

## IF-002 - Proposed drafting and source policy

| Field | Value |
| --- | --- |
| Status | Proposed in draft pull request #9; committee disposition required |
| Date | 2026-08-26 |
| Proposed decision | Use ISO/IEC Directives Part 2, RFC 8874, and OASIS Document Life Cycle Best Practices as bounded, informative development-process references; use ISO-style verbal forms in framework prose and map FHIR-native constraints explicitly. |
| Rationale | A common drafting model makes authority, normative intent, traceability, verification, and the framework-to-FHIR relationship reviewable. |
| Boundary | The proposal does not import ISO, IETF, OASIS, or HL7 governance; make a cited technology mandatory; or establish ISO/IEC 17025 as an AAVLD requirement. |
| Source issue | [#10 Approve drafting conventions and source-classification policy](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/10) |
| Related decision | [AAVLD-IT-Guidance #18](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance/issues/18) controls the committee disposition applied to ISO/IEC 17025. |
| Affected artifacts | `framework/drafting-conventions.md`, `references/source-classification.md`, source register, governance, contribution, templates, and release gates. |
| Decision authority | Repository maintainers may integrate the proposal; committee approval is required before Working Draft 0.1. |
