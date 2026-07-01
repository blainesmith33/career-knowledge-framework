# Master Experience Ledger (MEL) Specification

**Artifact:** Master Experience Ledger (MEL)  
**Framework:** Career Knowledge Framework (CKF)  
**Version:** 1.0  
**Status:** Draft – Authoritative Artifact Specification

---

## Purpose

The Master Experience Ledger (MEL) is the authoritative record of an individual's experiences that contribute to their professional capabilities.

The MEL establishes a single canonical representation of those experiences from which downstream career artifacts are derived.

The MEL is intended to answer one fundamental question:

> **What experiences has this individual had throughout their lifetime?**

---

## Authority

The MEL is the authoritative source for all experience-related information within the Career Knowledge Framework.

All downstream artifacts derive their experience information from the MEL.

No downstream artifact may modify, reinterpret, or replace information contained within the MEL.

Changes to professional experience originate in the MEL and propagate through derivative artifacts.

Authority flows through the Career Knowledge Framework in the following order:

```text
MEL -> CPIL -> CCA -> RGF
```

---

## Scope

The MEL may include, but is not limited to:

- Professional employment
- Self-employment
- Independent consulting
- Volunteer experience
- Formal education
- Professional development
- Apprenticeships
- Independent research
- Open-source contributions
- Personal projects
- Supplemental long-term experience
- Publications
- Creative work
- Other meaningful experience contributing to professional capability

---

## Non-Goals

The MEL does not:

- Evaluate capability.
- Rank proficiency.
- Recommend careers.
- Optimize resumes.
- Predict hiring outcomes.
- Interpret strengths or weaknesses.

Those responsibilities belong to downstream artifacts.

---

## Core Principles

The MEL is governed by the following principles:

### Experience Authoritative

The MEL is the canonical source of experience information.

### Owner Maintained

The individual is the primary authority regarding their own experiences.

Experiences do not require external documentation to be recorded.

### Evidence Supported

Supporting materials may be attached to experiences whenever available.

Evidence strengthens transparency and traceability but is not required for inclusion.

### Revision Controlled

The MEL evolves through documented revisions.

Historical changes should remain traceable.

### Long-Term

The MEL is intended to represent an individual's lifetime of experience rather than a single job search.

---

## Internal Structure

Each MEL entry should describe an experience.

An experience may contain:

- Title
- Organization
- Dates
- Category
- Description
- Responsibilities
- Outcomes
- Skills Demonstrated
- Notes
- Supporting Evidence (optional)
- Revision History

Individual implementations may extend these fields provided they preserve the authoritative nature of the artifact.

---

## Supporting Evidence

Supporting evidence is optional.

Evidence may include:

- Employment records
- Historical applications
- Tax records
- Certificates
- Licenses
- Publications
- Git repositories
- Videos
- Images
- Documentation
- Presentations
- Portfolios
- Other supporting materials

Supporting evidence increases confidence and transparency but does not determine whether an experience may be represented.

---

## Inputs

The MEL accepts information from:

- The individual.
- Historical records.
- Supporting documents.
- Public professional artifacts.
- Other trustworthy sources identified by the individual.

---

## Outputs

The MEL provides authoritative experience information to:

- Capability Pattern & Insight Ledger (CPIL)
- Career Capability Assessment (CCA)
- Resume Generation Framework (RGF)
- Position-specific resumes
- LinkedIn profiles
- Professional portfolios
- Career analyses
- Future CKF artifacts

---

## Relationship to Other Artifacts

The MEL serves as the foundation of the Career Knowledge Framework.

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

The MEL must not:

- Evaluate capability strength.
- Rank proficiency.
- Recommend careers.
- Optimize resumes.
- Predict hiring outcomes.
- Treat downstream interpretation as primary experience evidence.
- Allow downstream artifacts to rewrite or replace MEL experience records.

---

## Revision Behavior

The MEL should be revised when experience information is added, corrected, clarified, split, merged, or retired.

Revision should preserve traceability between recorded experiences, supporting evidence, and downstream artifacts that depend on those records.

When a MEL change affects downstream artifacts, the MEL remains the source of experience authority and downstream artifacts should be updated to reflect the revised experience record.

---

## Long-Term Role

The MEL is intended to remain the durable experience foundation of the Career Knowledge Framework.

Over time, it should make an individual's experience history easier to preserve, review, substantiate, and reuse without requiring each downstream artifact to maintain its own version of the same history.

---

## Summary

The Master Experience Ledger is the authoritative CKF artifact for experience records.

It provides the factual foundation from which capability patterns, assessments, presentation artifacts, and future CKF artifacts are derived.

The MEL must preserve experience authority, support traceability, and remain distinct from downstream interpretation and presentation.
