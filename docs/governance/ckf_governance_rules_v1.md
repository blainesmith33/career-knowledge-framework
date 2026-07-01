# CKF Governance Rules v1

**Framework:** Career Knowledge Framework (CKF)  
**Version:** 1.0  
**Status:** Draft - Governance Specification

---

## Purpose

The CKF Governance Rules define how authority, derivation, interpretation, presentation, revision, and traceability are managed across the Career Knowledge Framework.

Governance exists to preserve the core CKF principle that a career should have an authoritative knowledge representation before it has a presentation. Resumes, profiles, summaries, and other audience-facing artifacts should be derived from governed career knowledge rather than maintained as disconnected sources of truth.

These rules establish how CKF artifacts may consume, transform, interpret, and present information while preserving authority boundaries and preventing unsupported claims.

---

## Governance Scope

Governance applies across all CKF artifacts, including core artifacts, downstream career artifacts, supporting documentation, and future framework extensions.

The core governed artifact chain is:

```text
MEL -> CPIL -> CCA -> RGF
```

Governance applies whenever information is:

- Recorded as experience.
- Derived into capability patterns or insights.
- Interpreted or assessed.
- Transformed into presentation artifacts.
- Revised, corrected, retired, or reintroduced.
- Used by downstream artifacts or future CKF components.

Downstream artifacts are derivative. They may consume, transform, interpret, or present upstream material only within their authority boundary.

---

## Authority Model

Authority flows downstream through the Career Knowledge Framework.

```text
Individual
      |
      v
Master Experience Ledger (MEL)
      |
      v
Capability Pattern & Insight Ledger (CPIL)
      |
      v
Career Capability Assessment (CCA)
      |
      v
Resume Generation Framework (RGF)
      |
      v
Career Artifacts
```

Upstream artifacts control downstream artifacts.

Downstream artifacts may not override, replace, reinterpret, or backfill upstream authority. When downstream work reveals missing, ambiguous, or incorrect upstream information, that information must be reconciled into the appropriate upstream artifact before being used authoritatively.

The authority distinctions are:

- MEL = experience authority.
- CPIL = capability pattern and insight authority.
- CCA = interpretation and assessment authority.
- RGF = presentation transformation authority.

---

## Artifact Authority Boundaries

Each CKF artifact has a defined authority boundary.

The Master Experience Ledger (MEL) is authoritative for experience records, including recorded facts, chronology, roles, responsibilities, projects, activities, outcomes, and experience context.

The Capability Pattern & Insight Ledger (CPIL) is authoritative for capability patterns, insights, and supporting capability records derived from MEL experience records.

The Career Capability Assessment (CCA) is authoritative for interpretation and assessment of capability patterns and insights, including strength, limits, transferability, alignment, confidence, and career meaning.

The Resume Generation Framework (RGF) is authoritative for presentation transformation only, including emphasis, organization, wording, formatting, and audience-specific adaptation.

RGF outputs are not authoritative records. They are downstream presentations of upstream-authorized information.

---

## Source Authority and Individual Authority

The individual is the primary authority regarding their own experience.

The MEL records the individual's experience in a governed, structured, and traceable form. Experiences do not require external evidence to be represented in the MEL when the individual can reasonably attest to them.

Source authority begins with the individual and is represented through the MEL. Downstream artifacts may not treat generated language, inferred patterns, assessments, or presentation artifacts as replacements for the individual's recorded experience.

When a downstream artifact identifies a possible new experience, correction, role, project, outcome, or contextual detail, that information must be reconciled into the MEL before it is used authoritatively.

---

## Evidence Governance

Evidence strengthens transparency, specificity, and confidence, but it does not create experience authority.

Evidence may include documents, certificates, licenses, publications, repositories, work samples, presentations, portfolios, employment records, images, videos, or other supporting materials.

Evidence supports records but does not determine whether an experience may be represented. The absence of external evidence does not automatically invalidate an experience recorded in the MEL.

Evidence must not be used to bypass the MEL. If evidence reveals a new experience or correction, the experience record must be reconciled into the MEL before downstream artifacts treat it as authoritative.

Evidence may affect confidence, limits, specificity, and traceability. It must not be treated as a substitute for source authority.

---

## Traceability Requirements

CKF artifacts must preserve traceability across the authority chain.

Experience claims should trace to MEL records.

Capability patterns and insights should trace to MEL records through CPIL entries.

Interpretations and assessments should trace to CPIL records and, where relevant, MEL context.

Presentation claims should trace to MEL, CPIL, and CCA support as appropriate.

Traceability may be explicit or implicit depending on artifact type, but governance requires that substantive claims remain explainable in terms of upstream authority.

When traceability is missing, the claim must be treated as unsupported until reconciled with the appropriate upstream artifact.

---

## Derivation Rules

Derivation is the process of transforming MEL experience records into CPIL capability patterns and insights.

Derivation must be conservative, explainable, and traceable.

The CPIL may derive capability patterns and insights from recorded experience, responsibilities, activities, outcomes, tools, methods, domains, repeated patterns, and reasonable implications of MEL entries.

The CPIL must not invent capabilities without MEL support.

If a new capability is discovered downstream, it must be reconciled into the CPIL before being used authoritatively.

If the capability requires new experience support that is not present in the MEL, the experience must first be reconciled into the MEL.

---

## Interpretation Rules

Interpretation is the process of assessing what CPIL capability patterns and insights indicate about strength, depth, breadth, transferability, specialization, progression, relevance, confidence, and limits.

The CCA may interpret CPIL records and relevant MEL context. It must not create experience authority or capability pattern authority.

Interpretation must remain proportional to upstream support. The CCA must not convert weak, narrow, indirect, or ambiguous support into broad claims about mastery, seniority, scope, fit, or transferability.

If a new interpretation is discovered during presentation or other downstream work, it must be reconciled into the CCA before being treated as authoritative.

If that interpretation depends on a new capability, the capability must first be reconciled into the CPIL. If it depends on a new experience, the experience must first be reconciled into the MEL.

---

## Presentation Rules

Presentation is the process of transforming upstream-authorized information into audience-specific artifacts.

The RGF may adapt emphasis, organization, wording, formatting, density, sequencing, and tone for a target artifact or audience.

Presentation must preserve upstream authority. It must not add unsupported experience, capabilities, assessments, achievements, credentials, metrics, responsibilities, or outcomes.

Presentation context may guide what to emphasize, omit, qualify, or reorder. It must not create new source authority.

RGF outputs are not authoritative records. They are presentation artifacts derived from MEL, CPIL, CCA, and presentation-specific context.

---

## Revision Governance

Revisions must occur at the artifact layer that holds authority for the information being revised.

Experience revisions belong in the MEL.

Capability pattern and insight revisions belong in the CPIL.

Interpretation and assessment revisions belong in the CCA.

Presentation revisions belong in the RGF or downstream presentation artifact.

When downstream work reveals upstream gaps or errors, the downstream artifact should not silently absorb the change. The information must be reconciled into the appropriate upstream artifact before downstream artifacts rely on it authoritatively.

When an upstream artifact changes, downstream artifacts should be reviewed for consistency and revised where needed.

---

## Versioning Expectations

Meaningful artifact changes should be versioned so revisions remain reviewable and explainable.

Versioning should preserve:

- What changed.
- Why it changed.
- Which artifact held authority for the change.
- Which downstream artifacts may be affected.
- Whether confidence, limits, or traceability changed.

Versioning does not require any specific schema, tool, or implementation mechanism. It is a governance expectation that supports accountability and long-term maintainability.

---

## Unsupported Claim Handling

Unsupported claims must not be promoted into authoritative artifacts.

When a claim lacks traceable support, the framework should handle it by:

- Reconciling it into the MEL if it is an experience claim.
- Reconciling it into the CPIL if it is a capability pattern or insight claim supported by MEL records.
- Reconciling it into the CCA if it is an interpretation or assessment supported by CPIL and MEL records.
- Omitting, qualifying, or flagging it if it cannot be reconciled.

Unsupported claims must not be hidden inside presentation language.

Claims discovered during resume generation, profile writing, career analysis, or other downstream work remain non-authoritative until reconciled into the appropriate upstream artifact.

---

## Confidence, Limits, and Uncertainty

CKF governance requires confidence, limits, and uncertainty to remain visible where they materially affect interpretation or presentation.

Confidence may be shaped by specificity, recency, duration, repetition, directness of support, quality of evidence, and degree of inference required.

Limits should be preserved when support is narrow, dated, indirect, incomplete, ambiguous, or context-specific.

Uncertainty must not be resolved through invention. When the record supports more than one reasonable interpretation, the framework should preserve that ambiguity or route it to the appropriate artifact for clarification.

Downstream artifacts may simplify presentation, but they must not remove important limits in a way that misleads the audience.

---

## Downstream Artifact Governance

Downstream artifacts include resumes, profiles, biographies, portfolios, interview preparation materials, career summaries, job application materials, and future presentation or analysis artifacts.

Downstream artifacts are derivative. They do not hold authority over experience, capability patterns, insights, interpretations, or assessments unless a future CKF specification explicitly assigns a bounded authority role.

Downstream artifacts may consume governed upstream information and adapt it for a defined purpose. They may not redefine upstream facts, create unsupported claims, or override the authority chain.

If downstream work reveals new authoritative material, it must be reconciled upstream before being used authoritatively.

---

## Prohibited Behavior

CKF artifacts must not:

- Override the authority flow: MEL -> CPIL -> CCA -> RGF.
- Treat downstream artifacts as upstream authority.
- Invent experience, capabilities, interpretations, assessments, achievements, credentials, metrics, responsibilities, titles, dates, employers, tools, domains, awards, or outcomes.
- Treat evidence as a replacement for MEL authority.
- Treat absence of external evidence as proof that an experience did not occur.
- Convert presentation needs into source claims.
- Convert aspirational goals into demonstrated experience or capability claims.
- Present inferred material as directly evidenced material.
- Strengthen weak support beyond upstream confidence.
- Remove material limits when doing so would mislead the audience.
- Allow resume or profile wording to become the authoritative record.
- Modify an upstream artifact through a downstream artifact's authority.

---

## Governance Review

Governance review should occur when:

- A core artifact specification changes.
- A new artifact type is introduced.
- Authority boundaries become unclear.
- Downstream artifacts reveal unsupported claims or missing upstream records.
- Terminology changes affect multiple artifacts.
- Revision practices become inconsistent.
- Traceability is weakened or lost.

Governance review should verify that the authority model remains intact, terminology remains consistent, and downstream artifacts continue to respect upstream authority.

---

## Long-Term Governance Role

The long-term role of CKF governance is to keep career knowledge stable, traceable, and reusable as the framework evolves.

Governance separates experience authority, capability pattern and insight authority, interpretation and assessment authority, and presentation transformation authority. This separation allows CKF to support many career artifacts without collapsing all career knowledge into resumes or profiles.

Governance should remain durable as new artifact types, presentation channels, evidence sources, and career analysis methods are added. New extensions should integrate into the existing authority model unless governance explicitly defines a new bounded authority role.

---

## Summary

CKF governance applies across all framework artifacts.

The authority flow is:

```text
MEL -> CPIL -> CCA -> RGF
```

The MEL governs experience. The CPIL governs capability patterns and insights. The CCA governs interpretation and assessment. The RGF governs presentation transformation.

Upstream artifacts control downstream artifacts. Downstream artifacts may consume, transform, interpret, or present upstream material only within their authority boundary.

The individual is the primary authority regarding their own experience. Evidence strengthens transparency and confidence, but it does not create experience authority or determine whether an experience may be represented.

Any new experience, capability, or interpretation discovered downstream must be reconciled into the appropriate upstream artifact before being used authoritatively.

RGF outputs and other downstream career artifacts are not authoritative records. They are governed presentations of upstream-authorized career knowledge.
