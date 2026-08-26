# Source register - working inventory

The attributes below define how a source may be used. Citation does not by
itself make a source an AAVLD requirement, an interoperability mandate, or a
mandatory implementation technology. See the proposed
[source classification policy](source-classification.md).

Source IDs are local to this repository and remain stable. The Guidance
cross-reference column records related identifiers without renumbering either
register.

| ID | Source | Role | Authority domain | Adoption status | Version or date evaluated | Intended use and boundary | Guidance cross-reference |
| --- | --- | --- | --- | --- | --- | --- | --- |
| SRC-001 | [AAVLD Requirements for an Accredited Veterinary Medical Diagnostic Laboratory, Version 1](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance/blob/00683d0/references/aavld/AAVLD%20Requirements%20for%20an%20Accredited%20Veterinary%20Medical%20Diagnostic%20Laboratory-1137-1.pdf) | AAVLD accreditation source | AAVLD accreditation claims within cited clauses | Authoritative for those claims; not automatically a framework requirement | 1137 Version 1; accessed 2026-08-26 | Trace accreditation-related controls for records, validation, security, reporting, and interfaces. Do not derive interoperability semantics without a framework decision. | Guidance SRC-001 |
| SRC-002 | [AAVLD IT Guidance modernization](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance) | Related AAVLD project | Committee coordination for guidance scope and decisions | Related; controlling only for decisions explicitly owned there | Active repository; accessed 2026-08-26 | Coordinate validation, security, records, change-control, and cross-project decisions without duplicating authority. | Repository-level relationship |
| SRC-003 | [August 26, 2026 pre-meeting agenda](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance/blob/00683d0/meetings/AAVLD%202026/2026-08-26%20Informatics%20Committee%20Pre-Meeting%20Agenda.md) | AAVLD committee working record | Evidence of proposed agenda items only | Working record; not approval | 2026-08-26 agenda at commit `00683d0` | Track symposium and repository recommendations. Require a separate disposition record for any decision. | Meeting record |
| SRC-004 | [HL7 FHIR specification](https://hl7.org/fhir/) | Interoperability standard and alignment target | HL7 FHIR semantics and conformance for the selected version | Proposed first implementation-profile path; version and mandate undecided | R4, R4B, and R5 baseline evaluation pending #6; accessed 2026-08-26 | Map and test veterinary semantics without forcing unsuitable mappings. FHIR is not mandatory unless AAVLD approves a defined profile or conformance scope. | None |
| SRC-005 | Laboratory catalogs, forms, reports, and interface experience | Operational evidence | Participating organizations' own practices | Candidate evidence | Version and provenance recorded per contribution | Derive realistic synthetic use cases. Do not publish real, restricted, personal, client, owner, animal, accession, or production-system data. | None |
| SRC-006 | NAHLN, LOINC, SNOMED CT, UCUM, and other relevant sources | Candidate technical or terminology references | Each source's own technical or terminology domain | Candidate umbrella entry; each adopted source requires its own versioned record | To be determined during #6 | Evaluate veterinary fit, licensing, redistribution, mapping, version, and gaps before adoption. | None |
| SRC-007 | [ISO/IEC Directives Part 2](https://www.iso.org/directives-and-policies.html) | Development-process reference | ISO and IEC document structure and drafting | Proposed informative use pending #10 | Ninth edition, 2021, with Amendment 1:2026; accessed 2026-08-26 | Inform structure and verbal-form discipline only. Do not reproduce protected text or imply ISO process, certification, or endorsement. | Guidance SRC-004 |
| SRC-008 | [RFC 8874, Working Group GitHub Usage Guidance](https://www.rfc-editor.org/info/rfc8874/) | Development-process reference | IETF working-group use of GitHub | Proposed informative use pending #10 | Informational RFC, August 2020; accessed 2026-08-26 | Inform transparent issue, pull-request, and policy practices. Do not import IETF roles, mailing-list rules, consensus process, or authority. | Guidance SRC-005 |
| SRC-009 | [OASIS Document Life Cycle Best Practices](https://www.oasis-open.org/policies-guidelines/document-life-cycle-best-practices/) | Development-process reference | OASIS Technical Committee work-product lifecycle | Proposed informative use pending #10 | Version 2024.08.22; accessed 2026-08-26 | Inform stable artifacts and controlled progression. Retain AAVLD stage names, approvals, contribution terms, and intellectual-property rules. | Guidance SRC-006 |
| SRC-010 | [ISO/IEC 17025:2017](https://www.iso.org/standard/66912.html) | Related contextual reference | ISO/IEC laboratory competence requirements | Provisional; controlled by the disposition of AAVLD-IT-Guidance #18 | Edition 3, 2017-11; confirmed current in 2023; accessed 2026-08-26 | Potential contextual alignment only. Do not present it as an AAVLD accreditation or interoperability requirement without an explicit AAVLD decision. | Guidance SRC-007 and [Guidance #18](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance/issues/18) |

## Source rules

- Preserve authoritative source versions and dates.
- Link to external standards rather than copying them unless redistribution is
  permitted.
- Separate AAVLD accreditation requirements, framework requirements,
  recommendations, examples, and implementation-profile constraints.
- Record provisional interpretations as issues until the required authority
  resolves them.
- Replace umbrella candidate entries with individually versioned records before
  normative or computable use.
- Record superseded versions and decisions rather than silently replacing them.
