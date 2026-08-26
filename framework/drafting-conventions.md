# Framework drafting conventions - proposed

**Status:** Provisional working policy pending disposition of
[#10](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/10).

These conventions apply to human-readable framework text and its relationship
to computable implementation-profile artifacts. They do not import ISO, IETF,
OASIS, or HL7 governance into AAVLD and do not make a source or technology
mandatory merely by citation.

## Statement classes and verbal forms

The proposed framework prose uses one verbal form for each statement class.
The committee must approve or revise this model before Working Draft 0.1.

| Statement class | Form | Meaning |
| --- | --- | --- |
| Framework requirement | `shall` | Necessary for conformance to the identified framework scope. |
| Recommendation | `should` | Preferred approach with documented reasons permitting an alternative. |
| Permission | `may` | Permitted course of action. |
| Possibility or capability | `can` | Describes capability or possibility; it does not grant permission or impose a requirement. |
| Implementation-profile constraint | Formal profile rule plus explanatory prose | A testable restriction for a named technology and version, traceable to framework requirements or an explicit profile decision. |
| Example | Clearly labeled `Example` | Informative illustration that does not establish conformance. |
| Note or rationale | Clearly labeled `Note` or `Rationale` | Informative explanation that does not contain hidden requirements. |
| Open issue | Linked issue identifier | Unresolved content that must not be presented as an accepted requirement. |

Do not use uppercase RFC keywords and ISO-style verbal forms interchangeably.
Quoted or referenced external text retains its original meaning within that
external source; AAVLD meaning is established only by this framework and its
recorded decisions.

## Conformance statement structure

Each framework requirement, recommendation, permission, or
implementation-profile constraint must identify:

1. **Identifier:** a stable reference once the statement enters a published
   Working Draft;
2. **Conformance subject:** the organization, system, sender, receiver,
   repository role, profile, or other actor to which it applies;
3. **Behavior:** one clear action or property;
4. **Conditions:** the event, state, scope, or exception under which it applies;
5. **Traceability:** source IDs and the governing issue or decision; and
6. **Verification:** automated test, inspection, document review,
   demonstration, or a stated reason that verification is deferred.

Use one principal requirement per statement. Avoid passive constructions that
hide the responsible subject and avoid subjective terms unless their evaluation
criteria are defined.

## Requirement identifiers

- Published framework statements use `AAVLD-IF-<AREA>-<NNN>`.
- Identifiers are assigned when a statement first enters Working Draft 0.1.
- An assigned identifier is not reused after removal; the disposition is
  retained in traceability records.
- Pre-symposium illustrations use `EXAMPLE-...` identifiers so they cannot be
  mistaken for adopted requirements.

## FHIR conformance bridge

- Framework requirements remain technology-neutral unless a recorded decision
  explicitly makes an implementation profile part of the conformance scope.
- Every FHIR artifact must state its FHIR version and package or profile
  dependency versions.
- Cardinalities, bindings, invariants, slicing, capability expectations, and
  other FHIR constraints must trace to one or more framework statements or an
  explicit implementation-profile decision.
- A FHIR `mustSupport` flag is incomplete unless the implementation guide also
  defines the behavior that support requires for the relevant producer,
  consumer, or other actor.
- A FHIR example illustrates intent but is not a conformance resource.
- Unresolved veterinary gaps remain linked issues; they must not be concealed
  through a forced FHIR mapping.
- The project must not claim conformance to a FHIR implementation guide until
  the named artifacts have passed the applicable validator and review gates.

The FHIR version baseline remains open under
[#6](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/6).

## Verification methods

| Method | Appropriate use |
| --- | --- |
| Automated test | Schema, profile, invariant, terminology, identifier, state-transition, or example validation. |
| Inspection | Presence, structure, linkage, version metadata, or other directly observable evidence. |
| Document review | Semantic, governance, authority, safety, licensing, or traceability requirements. |
| Demonstration | End-to-end behavior across representative independent implementations. |
| Deferred | Pre-symposium question with an owner, issue, reason, and target stage. |

## AAVLD working stages and gates

The names below are AAVLD working stages. OASIS lifecycle material informs the
idea of stable artifacts and controlled progression but does not supply AAVLD
votes, stage names, intellectual-property rules, or approval authority.

| Stage | Minimum gate |
| --- | --- |
| Pre-symposium working material | Clearly marked provisional; sources and open decisions are linked. |
| Symposium working package | Stable dated package; agenda, use cases, reviewers, and decision questions identified. |
| Working Draft 0.1 | Committee disposition recorded; statement classes, traceability, versions, and known gaps are visible. |
| Pilot draft | Pilot scope, participants, validation method, results, deviations, and compatibility findings recorded. |
| Candidate framework | Material comments resolved or explicitly deferred; conformance and release evidence complete. |
| Approved Framework 1.0 | Formal AAVLD publication authority and approval record identified. |

Progression never implies a higher approval than the authority recorded for
that stage.

## Classification examples

The following statements test the conventions. They are illustrations, not
adopted requirements.

| ID | Class | Illustrative statement | Conformance subject | Verification |
| --- | --- | --- | --- | --- |
| EXAMPLE-REQ-001 | Framework requirement | A receiving laboratory shall return an acknowledgement for each submitted request, identifying acceptance, rejection, or the need for clarification. | Receiving laboratory exchange function | Demonstrate each outcome in a synthetic request sequence. |
| EXAMPLE-FHIR-001 | Implementation-profile constraint | An AAVLD FHIR request profile shall define how the originating request identifier is represented and validated. | Named AAVLD FHIR request profile | Inspect the profile and validate a positive and negative synthetic example; exact mapping remains subject to #6. |
| EXAMPLE-REC-001 | Recommendation | An implementation should retain a reviewable mapping between external identifiers and its local identifiers. | Implementing organization or system | Inspect mapping evidence or record the justified alternative. |

Reviewers should be able to classify the statement, identify its subject, and
apply the verification method without additional verbal explanation. Failure
to do so means the convention or statement requires revision.
