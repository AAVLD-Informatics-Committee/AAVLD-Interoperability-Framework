# AAVLD Interoperability Framework

**Status:** Pre-symposium working structure - 2026-08-26

> This material is not an approved AAVLD standard or accreditation requirement.

## Purpose

Define shared veterinary diagnostic laboratory semantics and exchange behavior
that can be implemented across different organizations, LIMS products, vendors,
and technical transports.

## Initial scope

- Publishing laboratory tests and services.
- Moving from test request through validation, acknowledgement, and accession.
- Preserving subject, specimen, organization, request, accession, result, and
  report identity.
- Returning interim and final results.
- Managing rejections, cancellations, corrections, amendments, and referrals.
- Aligning identifiers, terminology, error handling, governance, and change.
- Mapping and testing the model through a FHIR implementation-profile path.

## Pre-symposium exclusions

Unless explicitly brought into scope by a recorded decision, the initial work
does not define production transport selection, authentication architecture,
billing, complete practice-management workflows, formal FHIR Implementation
Guide publication, or full deployment requirements.

## Initial use-case sequence

1. Publish and discover a test or service offering.
2. Submit a request and determine whether it is accepted, rejected, or requires
   clarification.
3. Create an accession while preserving original identifiers.
4. Return interim and final results with authorization and traceability.
5. Correct, amend, cancel, or replace information without losing history.

Detailed requirements and conformance language will be developed through linked
issues and recorded decisions.
