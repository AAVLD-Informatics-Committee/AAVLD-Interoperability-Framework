# FHIR alignment - working approach

**Status:** Required analysis; no FHIR version or conformance profile has been
approved.

The conceptual veterinary model defines the intended meaning and behavior. HL7
FHIR is the first implementation-profile path to be mapped and tested. Use of
FHIR is not mandatory unless AAVLD later approves a specific conformance
requirement or implementation profile.

## Initial candidate mappings

Candidate resources for assessment include Organization, Endpoint, Patient,
Group, ServiceRequest, Task, Specimen, Observation, DiagnosticReport,
Provenance, AuditEvent, and applicable bundle or messaging patterns. Catalog
representation requires a separate evidence-based assessment and must not be
forced into an unsuitable resource.

## Alignment matrix fields

- Framework concept and required behavior
- Candidate resource and element
- Cardinality and terminology binding
- R4, R4B, and R5 implementation considerations
- Direct mapping, profile constraint, extension, or gap
- Veterinary-specific need
- Linked issue and decision status
- Synthetic example and validation result

## Veterinary gap tests

- Individual animal versus herd, flock, population, pool, or environmental
  subject
- Owner, client, submitter, receiving laboratory, performing laboratory, and
  referral relationships
- Original and derived specimens
- Laboratory service catalogs and stable offering identifiers
- Accession identity across organizations
- Interim, final, corrected, amended, cancelled, and replaced results or reports
- Terminology for tests, matrices, species, methods, units, and interpretations

FHIR and HL7 are registered trademarks of Health Level Seven International. Use
of the marks does not imply endorsement by HL7.
