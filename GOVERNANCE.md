# Proposed governance

This is a working governance model pending committee and AAVLD confirmation.

## Authority layers

| Authority | Responsibility |
| --- | --- |
| Repository maintainer | Maintains repository settings and may merge an eligible pull request. |
| Committee decision authority | Resolves substantive scope, semantic, technical, and governance questions. |
| AAVLD publication authority | Approves an official AAVLD release or implementation mandate. |

An approval or merge at one layer does not imply approval at another layer.

## Project records

- Issues record work, questions, evidence, and decision requests.
- The decision log summarizes accepted or tentative dispositions.
- The source register and classification policy record provenance, authority,
  adoption status, and permitted use.
- Pull requests record proposed repository changes.
- Merged content is the integrated working source.
- Tagged releases identify stable review or approved artifacts.
- The GitHub Project is an operational dashboard and does not override the
  records above.

## Change workflow

1. Open or identify the governing issue.
2. Gather source evidence, use cases, and implementation impact.
3. Classify proposed statements and identify their conformance subjects,
   traceability, and verification approach.
4. Record required committee or AAVLD disposition.
5. Propose text or computable changes through a pull request.
6. Review drafting, authority, mapping, terminology, compatibility, validation,
   licensing, and data-safety effects.
7. Merge only within the authority granted to repository maintainers.
8. Update the decision log and changelog when applicable.

## Drafting and conformance authority

The proposed [drafting conventions](framework/drafting-conventions.md) and
[source classification policy](references/source-classification.md) apply to
working material pending committee disposition of
[#10](https://github.com/AAVLD-Informatics-Committee/AAVLD-Interoperability-Framework/issues/10).

- Repository maintainers may integrate clearly marked provisional material.
- The committee resolves framework statement classes, normative language,
  semantic requirements, and implementation-profile scope.
- Formal AAVLD publication authority approves an official framework release or
  implementation mandate.
- An external source controls only its stated authority domain. Referencing ISO,
  IETF, OASIS, or HL7 material does not transfer their governance or approval to
  AAVLD.
- A computable FHIR constraint must trace to framework text or a recorded
  implementation-profile decision, identify its FHIR version, and state its
  verification evidence.

## Working states

1. Pre-symposium working material.
2. Symposium working package.
3. Working Draft 0.1.
4. Pilot draft.
5. Candidate framework.
6. Approved Framework 1.0.

The symposium output does not automatically become Working Draft 0.1. Outcomes
must be reconciled and approved by the required authority. Minimum entry gates
for each stage are defined in the
[drafting conventions](framework/drafting-conventions.md).

## Decisions still required

- Name repository maintainers and reviewers.
- Identify committee decision and AAVLD publication authorities.
- Confirm licensing and external contribution terms.
- Define quorum, decision recording, dissent, and reconsideration rules.
- Decide whether stakeholder or public review is required.
- Approve or revise the drafting conventions and source-classification policy
  in #10.
- Apply the controlling disposition from AAVLD-IT-Guidance #18 to any
  ISO/IEC 17025 relationship stated by this framework.
