# Resume Generation Framework (RGF) Specification

**Artifact:** Resume Generation Framework (RGF)  
**Framework:** Career Knowledge Framework (CKF)  
**Version:** 1.0  
**Status:** Draft – Authoritative Artifact Specification

---

## Purpose

The Resume Generation Framework (RGF) is the authoritative presentation transformation layer within the Career Knowledge Framework.

The RGF transforms authoritative upstream career knowledge into presentation-ready career artifacts, including resumes, profiles, summaries, and role-specific narrative materials.

The RGF is intended to answer one fundamental question:

> **How should authoritative career knowledge be presented for a specific audience, opportunity, or artifact type?**

---

## Authority

The RGF is authoritative for presentation transformation only.

The RGF is not authoritative for experience records. Experience authority remains exclusively with the Master Experience Ledger (MEL).

The RGF is not authoritative for capability patterns or insights. Capability pattern and insight authority remains with the Capability Pattern & Insight Ledger (CPIL).

The RGF is not authoritative for assessment interpretation. Interpretation and assessment authority remains with the Career Capability Assessment (CCA).

The RGF consumes MEL, CPIL, CCA, and presentation-specific context without modifying upstream artifacts.

Authority flows through the Career Knowledge Framework in the following order:

```text
MEL -> CPIL -> CCA -> RGF
```

Changes to experience information originate in the MEL. Changes to capability patterns and insights originate in the CPIL. Changes to assessment interpretation originate in the CCA. Changes to presentation originate in the RGF only when they preserve upstream authority and traceability.

---

## Scope

The RGF may transform authoritative upstream information by:

- Selecting upstream-supported material for a target artifact.
- Adapting emphasis to a target role, audience, sector, seniority level, or presentation channel.
- Organizing content into artifact-appropriate sections, bullets, summaries, narratives, or profile components.
- Refining wording while preserving substantive meaning.
- Applying formatting, sequencing, density, and length choices appropriate to the presentation context.
- Preserving traceability from presented claims to upstream experience, capability, and assessment records.
- Representing confidence limits, evidence limits, or assessment constraints when needed.

Presentation-specific context may include a target role, job description, audience, format, channel, length constraint, tone requirement, sector convention, or user preference.

---

## Non-Goals

The RGF does not:

- Record primary experience history.
- Replace or override the MEL.
- Create or modify capability patterns or insights.
- Replace or override the CPIL.
- Create or modify assessment interpretation.
- Replace or override the CCA.
- Invent experience, capabilities, assessments, achievements, credentials, or outcomes.
- Validate source evidence.
- Fill evidence gaps by assumption.
- Predict hiring outcomes.
- Serve as a schema, renderer, parser, tool, or implementation contract.

Those responsibilities belong to the MEL, CPIL, CCA, governance documents, or future downstream artifacts as appropriate.

---

## Core Principles

The RGF is governed by the following principles:

### Downstream of CCA

The RGF depends on the CCA for governed interpretation and assessment authority.

No RGF output may establish an interpretation or assessment that is absent from, or unsupported by, the CCA and its upstream sources.

### Grounded in MEL and CPIL

The RGF may use MEL experience records and CPIL capability patterns and insights when presenting authorized career information.

MEL and CPIL context informs presentation but remains governed by those upstream artifacts.

### Presentation Authoritative

The RGF is the canonical CKF source for presentation transformation decisions.

Downstream career artifacts should use the RGF when they need audience-specific wording, organization, emphasis, and formatting rather than raw upstream records alone.

### Traceable

Substantive claims in RGF outputs should remain traceable to MEL, CPIL, and CCA support.

Traceability allows readers and maintainers to distinguish presentation choices from experience authority, capability authority, and assessment authority.

### Conservative

The RGF should avoid overstating experience, capability strength, seniority, scope, outcomes, transferability, or role fit.

Presentation should remain proportional to the authoritative upstream records that support it.

### Context-Sensitive

The RGF may adapt language, order, emphasis, and format to a target audience or opportunity.

Context may shape presentation, but it cannot create new experience, capability, or assessment authority.

### Revision Controlled

The RGF evolves through documented revisions.

Presentation artifacts should remain explainable as upstream MEL, CPIL, and CCA records are added, clarified, split, merged, retired, or revised.

### Long-Term

The RGF is intended to support repeated presentation of authoritative career knowledge across many audiences, opportunities, and artifact types.

---

## Presentation Policy

The RGF may adapt presentation across four primary dimensions:

- Emphasis: highlighting upstream-supported material relevant to the target context.
- Organization: arranging material into an artifact structure suitable for the intended audience or channel.
- Wording: converting upstream records and assessments into clear professional language without changing substantive meaning.
- Formatting: applying layout, sectioning, bullet structure, ordering, and length control.

Presentation choices must remain bounded by upstream authority.

When target context suggests stronger framing than upstream evidence supports, the RGF must use the upstream-supported framing. When upstream confidence is limited, mixed, or conditional, the RGF must avoid presenting the claim as stronger than authorized.

---

## Transformation Process

RGF transformation begins with authoritative upstream information and a presentation-specific context.

The RGF should:

- Identify the target artifact type, audience, role, channel, tone, and constraints.
- Select relevant MEL, CPIL, and CCA material for that context.
- Determine presentation emphasis using upstream relevance, confidence, and assessment guidance.
- Transform selected material into artifact-appropriate language and structure.
- Preserve authority boundaries and traceability for substantive claims.
- Apply confidence limits and omit, qualify, or soften weakly supported material.
- Produce the requested presentation artifact or presentation guidance without modifying upstream artifacts.

---

## Target Artifact Types

The RGF may produce or guide presentation artifacts such as:

- General resumes.
- Targeted resumes.
- Role-specific resume variants.
- Executive summaries.
- Professional profiles.
- LinkedIn-style summaries and experience sections.
- Bio statements.
- Cover letter source material.
- Interview narrative summaries.
- Capability highlights.
- Portfolio or case-study summaries.
- Recruiter-facing briefs.
- Internal mobility profiles.

Different artifact types may require different levels of compression, specificity, tone, and structure. These differences affect presentation only. They do not change upstream truth, evidence, assessment, or authority.

---

## Confidence and Limits

The RGF must respect confidence and limits established upstream.

If the CCA indicates strong support for a capability or assessment, the RGF may present that material with confident language appropriate to the artifact. If support is partial, indirect, dated, inferred, or context-limited, the RGF must avoid overstating it.

The RGF treats absence of evidence as a presentation limit, not as permission to fill gaps.

When presentation-specific context introduces a desired emphasis that is not supported by MEL, CPIL, or CCA, the RGF must exclude that emphasis or present only supported adjacent material.

---

## Inputs

The RGF accepts information from:

- Master Experience Ledger records.
- Capability Pattern & Insight Ledger records.
- Career Capability Assessment interpretations.
- Supporting evidence referenced by upstream artifacts.
- Presentation-specific context supplied for artifact generation.
- Clarifications from the individual when tied back to authoritative upstream records.

The RGF must not accept untraceable experience, capability, assessment, or achievement claims as authoritative presentation inputs.

---

## Outputs

The RGF provides presentation guidance and presentation-ready artifacts to:

- Targeted resumes.
- Professional profiles.
- LinkedIn profiles.
- Professional portfolios.
- Cover letter source material.
- Interview preparation artifacts.
- Career summaries.
- Future CKF presentation artifacts.

RGF outputs may include:

- Draft resumes or resume sections.
- Profile summaries.
- Experience bullets.
- Capability summaries.
- Role-targeted positioning statements.
- Artifact outlines.
- Presentation recommendations.
- Tailoring notes.
- Traceability notes where appropriate.
- Confidence or limitation notes where appropriate.

RGF outputs are not new authoritative records of experience, capability, or assessment. They are downstream presentations of upstream-authorized information.

---

## Relationship to Other Artifacts

The RGF sits downstream of the MEL, CPIL, and CCA and upstream of final career artifacts.

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

The MEL records experience.

The CPIL records capability patterns and insights derived from experience.

The CCA interprets and assesses capability patterns and insights in career, role, domain, and developmental contexts.

The RGF transforms authoritative upstream information into presentation-specific career artifacts.

---

## Prohibited Behavior

The RGF must not:

- Invent experience, capabilities, assessments, achievements, credentials, metrics, responsibilities, employers, titles, dates, tools, technologies, domains, publications, awards, or outcomes.
- Modify MEL, CPIL, CCA, or any upstream artifact.
- Override the CKF authority flow.
- Treat presentation context as evidence of experience, capability, or assessment.
- Convert aspirational goals into demonstrated capability claims.
- Strengthen weak evidence beyond upstream confidence.
- Present inferred material as directly evidenced material.
- Remove important limitations when doing so would mislead the audience.
- Claim target-role fit beyond CCA-supported relevance.
- Backfill missing details from common industry assumptions.
- Optimize for persuasion at the expense of truthfulness, authority, or traceability.

---

## Revision Behavior

RGF revisions are presentation revisions only.

When an RGF output is revised, the revision may change wording, ordering, emphasis, format, length, tone, or artifact structure.

Revision must not change underlying career facts, capability patterns, insights, assessments, or confidence boundaries unless upstream artifacts have first been revised through their own authority processes.

If a requested revision requires unsupported content, the RGF should decline that transformation or identify the need for upstream evidence or assessment. If a requested revision conflicts with MEL, CPIL, or CCA, the upstream artifact controls.

---

## Long-Term Role

The RGF is intended to become the durable presentation transformation layer of the Career Knowledge Framework.

Over time, it should make authoritative career knowledge easier to present across many audiences and opportunities without collapsing experience authority, capability authority, assessment authority, and presentation authority into a single artifact.

The RGF supports long-term career knowledge management by separating presentation from upstream evidence, insight, and interpretation while preserving traceability to authoritative upstream artifacts.

---

## Summary

The Resume Generation Framework is the authoritative CKF artifact for presentation transformation.

It remains downstream of the MEL, CPIL, and CCA and consumes upstream artifacts without modifying them.

The RGF may adapt emphasis, organization, wording, and formatting for a target artifact or audience.

It must not invent experience, capabilities, assessments, achievements, or outcomes, and every substantive claim must remain traceable to authoritative upstream artifacts.

The RGF provides the governed presentation layer used by resumes, profiles, summaries, interview preparation, and future career artifacts.
