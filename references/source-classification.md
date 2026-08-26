# Source classification policy - proposed

**Status:** Provisional working policy pending disposition of
[#10](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/10).

## Rule

A source must be described along several dimensions. A label or citation does
not transfer the source's authority into the AAVLD Interoperability Framework
and does not make a technology, terminology, process, or laboratory control
mandatory.

| Attribute | Question answered |
| --- | --- |
| Source role | What kind of evidence or practice does the source provide? |
| Authority domain | For which claims, and under whose authority, is the source controlling? |
| Adoption status | Has AAVLD approved, proposed, excluded, or only considered its use? |
| Version and date | Which exact edition, release, or dated record was evaluated? |
| Use boundary | What may and may not be derived from the source? |

## Source roles

| Role | Permitted use |
| --- | --- |
| AAVLD accreditation source | Supports statements about existing AAVLD accreditation requirements within the cited clause and version. It does not automatically establish an interoperability requirement. |
| AAVLD governance or committee record | Records authority, direction, decisions, dissent, and unresolved work. A working record is not formal approval by itself. |
| Development-process reference | Informs drafting, review, repository, or lifecycle practice only. It is not a source of veterinary laboratory controls or interoperability requirements. |
| Interoperability standard or alignment target | Supplies external semantics, exchange patterns, or conformance mechanisms for evaluation or an approved implementation profile. Citation alone does not make it mandatory. |
| Terminology reference | Supplies codes, value sets, units, or mappings subject to version, licensing, veterinary fit, and an adoption decision. |
| Related contextual reference | Provides relevant context outside the framework's direct authority. Its relationship must be stated and approved before normative use. |
| Operational evidence | Grounds use cases and tests in actual practice. Restricted data must be replaced with synthetic examples before publication. |
| Example only | Illustrates a possible implementation without creating a requirement or preferred product design. |

## Adoption states

- **Proposed:** use is recommended but awaiting the identified decision authority.
- **Informative:** the source may guide work within a stated boundary but is not
  an AAVLD requirement or implementation mandate.
- **Approved:** the identified authority has approved the stated use, version,
  and boundary; the decision record must be linked.
- **Excluded:** the source was considered and intentionally not used, with the
  rationale recorded.
- **Superseded:** a later version or decision replaced the recorded use.

## Authority domains

Authority is specific to the claim being made. Examples include AAVLD
accreditation requirements, AAVLD committee governance, AAVLD publication,
HL7 FHIR semantics for a selected FHIR version, and an external standards
body's own publication. No source is universally authoritative for all of
these domains.

## Drafting and traceability test

Before a substantive statement enters Working Draft 0.1, its record must
identify:

1. the statement class defined in
   [the drafting conventions](../framework/drafting-conventions.md);
2. supporting source IDs and exact versions;
3. the authority domain and adoption status;
4. the governing issue or recorded decision; and
5. the applicable verification approach.

If these cannot be identified, the statement remains an open issue or
informative working note.

## Cross-repository and copyright rules

- Source IDs are repository-local and must not be renumbered merely to match
  another repository. Record explicit cross-references instead.
- A decision owned by another AAVLD project must have one controlling record;
  this repository records the dependency and resulting application.
- Link to external standards and record bibliographic facts. Do not copy
  protected text, terminology, schemas, or examples unless redistribution is
  permitted.
- ISO/IEC 17025 remains a related contextual reference unless the disposition
  of [AAVLD-IT-Guidance #18](https://github.com/AAVLD-Informatics-Committee/AAVLD-IT-Guidance/issues/18)
  establishes a different AAVLD relationship.
