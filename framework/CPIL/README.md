# Capability Pattern & Insight Ledger (CPIL) Specification

**Artifact:** Capability Pattern & Insight Ledger (CPIL)  
**Framework:** Career Knowledge Framework (CKF)  
**Version:** 1.0  
**Status:** Draft – Authoritative Artifact Specification

---

## Purpose

The Capability Pattern & Insight Ledger (CPIL) is the authoritative record of an individual's Capability Knowledge within the Career Knowledge Framework.

Capability Knowledge consists of capability patterns, capability insights, and capability records.

The CPIL translates experience information from the Master Experience Ledger (MEL) into structured Capability Knowledge that can be interpreted, assessed, reasoned about, and reused by downstream artifacts.

The CPIL is intended to answer one fundamental question:

> **What capabilities are reasonably supported by this individual's recorded experiences?**

---

## Authority

The CPIL is authoritative for Capability Knowledge only.

The CPIL is not authoritative for experience records. Experience authority remains exclusively with the MEL.

Every CPIL capability must trace back to one or more MEL entries.

The CPIL may derive, organize, clarify, and characterize capabilities from MEL entries, but it may not create experience authority, modify MEL entries, or represent unsupported experience as fact.

Authority flows through the Career Knowledge Framework in the following order:

```text
MEL -> CPIL -> CCA -> RGF
```

Changes to experience information originate in the MEL. Changes to Capability Knowledge originate in the CPIL only when they remain traceable to authoritative MEL entries.

---

## Scope

The CPIL may include capabilities derived from:

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
- Other meaningful experience recorded in the MEL

The CPIL may describe capabilities across technical, operational, strategic, interpersonal, analytical, creative, leadership, domain, and execution-oriented dimensions.

The CPIL describes capabilities as reusable professional attributes, not as standalone claims detached from experience.

---

## Non-Goals

The CPIL does not:

- Record primary experience history.
- Replace or override the MEL.
- Create capabilities without MEL traceability.
- Require external evidence before representing a capability reasonably derived from the MEL.
- Rank an individual against other people.
- Predict hiring outcomes.
- Generate resumes.
- Select resume content for a specific role.
- Serve as a public-facing professional profile by default.

Those responsibilities belong to the MEL, CCA, RGF, or other downstream artifacts as appropriate.

---

## Core Principles

The CPIL is governed by the following principles:

### Downstream of MEL

The CPIL depends on the MEL for experience authority.

No CPIL capability may exist without a traceable relationship to one or more MEL entries.

### Capability Knowledge Authoritative

The CPIL is the canonical CKF source for Capability Knowledge.

Downstream artifacts should use the CPIL when they need capability patterns, capability insights, or capability records rather than re-deriving capabilities directly from experience records.

### Traceable

Each capability must identify the MEL entry or entries from which it is derived.

Traceability allows downstream artifacts to distinguish Capability Knowledge from primary experience history.

### Reasonably Derived

A capability may be represented when it is a reasonable interpretation of an authoritative MEL entry.

External evidence is not required when the capability is sufficiently supported by the MEL entry itself.

### Evidence Supported

Supporting evidence may strengthen the transparency, specificity, and confidence of a capability record.

Evidence does not create experience authority and does not replace the MEL as the source of experience authority.

### Revision Controlled

The CPIL evolves through documented revisions.

Capability records should remain explainable as MEL entries are added, clarified, split, merged, or revised.

### Long-Term

The CPIL is intended to represent an individual's evolving lifetime capability profile rather than the requirements of a single job search.

---

## Internal Structure

Each CPIL entry should describe a capability.

A capability may contain:

- Capability title
- Capability category
- Capability description
- Derived-from MEL entry references
- Related responsibilities, activities, or outcomes
- Contexts in which the capability was demonstrated
- Descriptive context or maturity indicators
- Potential transferability context
- Supporting evidence references, when available
- Confidence notes
- Limitations or boundaries
- Revision history

Individual implementations may extend these fields provided they preserve MEL traceability and the CPIL's authority over Capability Knowledge only.

---

## Capability Categories

The CPIL may organize capabilities into categories such as:

- Technical capabilities
- Domain knowledge
- Operational capabilities
- Analytical capabilities
- Communication capabilities
- Leadership and management capabilities
- Project and program capabilities
- Strategy and planning capabilities
- Research and learning capabilities
- Creative and design capabilities
- Customer, stakeholder, or community capabilities
- Tool, platform, and methodology capabilities

Categories are organizational aids.

They do not create Capability Knowledge authority by themselves and must not obscure the MEL entries from which each capability is derived.

---

## Capability Derivation

Capability derivation is the process of deriving, organizing, relating, preserving, and describing MEL-supported Capability Knowledge.

A CPIL capability may be derived from:

- Explicit skills listed in a MEL entry
- Responsibilities described in a MEL entry
- Outcomes or deliverables recorded in a MEL entry
- Tools, methods, or domains associated with a MEL entry
- Repeated patterns across multiple MEL entries
- Reasonable implications of the work performed in a MEL entry

Derivation must remain conservative, explainable, and traceable.

The CPIL may infer a capability when the inference is a reasonable consequence of recorded experience. It must not inflate the scope, duration, seniority, or certainty of that capability beyond what the MEL supports.

---

## Supporting Evidence

Supporting evidence is optional.

Evidence may include:

- Certificates
- Licenses
- Work samples
- Publications
- Git repositories
- Presentations
- Portfolios
- Performance artifacts
- Historical applications
- Employment records
- Project documentation
- Images, videos, or demonstrations
- Other supporting materials

Evidence strengthens transparency and confidence in a capability record.

Evidence does not create experience authority. A capability may still be represented when it is reasonably derived from an authoritative MEL entry even if no separate supporting evidence is available.

---

## Confidence and Limits

The CPIL may describe confidence, maturity, recency, breadth, depth, or limits associated with a capability.

Confidence should reflect the quality and specificity of the MEL support, the number of related MEL entries, recency, duration, outcomes, and any supporting evidence.

Confidence must not be treated as a substitute for traceability.

Limitations should be recorded when the MEL supports a capability only in a narrow context, at a limited scale, during a specific period, or with incomplete detail.

---

## Inputs

The CPIL accepts information from:

- Master Experience Ledger entries
- MEL revision history
- Skills, responsibilities, outcomes, and notes recorded in the MEL
- Supporting evidence referenced by MEL entries
- Capability clarification provided by the individual when tied back to MEL entries

The CPIL must not accept untraceable capability claims as authoritative Capability Knowledge.

---

## Outputs

The CPIL provides authoritative Capability Knowledge to:

- Career Capability Assessment (CCA)
- Resume Generation Framework (RGF)
- Position-specific resumes
- LinkedIn profiles
- Professional portfolios
- Career analyses
- Future CKF artifacts

Outputs from the CPIL should preserve traceability to MEL-derived Capability Knowledge wherever practical.

---

## Relationship to Other Artifacts

The CPIL sits downstream of the MEL and upstream of assessment and presentation artifacts.

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

The CPIL records Capability Knowledge derived from experience.

The CCA interprets and assesses Capability Knowledge against career, role, or market contexts.

The RGF transforms authoritative experience, capability pattern, insight, and assessment information into presentation-specific career artifacts.

---

## Prohibited Behavior

The CPIL must not:

- Invent capabilities without MEL support.
- Treat evidence as a replacement for MEL authority.
- Treat absence of external evidence as absence of capability when the MEL reasonably supports the capability.
- Modify MEL experience records.
- Represent experience records as if they originated in the CPIL.
- Convert weak or narrow experience support into broad capability claims.
- Assess capability meaning, strength, transferability, career fit, or professional direction.
- Present speculative, aspirational, or desired capabilities as established capabilities.
- Override downstream assessment decisions made by the CCA.
- Generate final resume language as if it were the RGF.

---

## Revision Behavior

The CPIL should be revised when:

- MEL entries are added, removed, clarified, split, merged, or corrected.
- Capability Knowledge becomes more precise.
- Supporting evidence becomes available.
- Confidence or limitation notes need refinement.
- Capability categories are reorganized.
- Downstream artifacts reveal ambiguity that should be resolved at the Capability Knowledge level.

Revision should preserve the relationship between each capability and the MEL entry or entries that support it.

When a MEL change invalidates a capability, the CPIL should revise, retire, or qualify the affected capability rather than preserve it as an unsupported claim.

---

## Long-Term Role

The CPIL is intended to become the durable capability layer of the Career Knowledge Framework.

Over time, it should make an individual's capabilities easier to understand, compare, assess, and reuse without repeatedly reinterpreting raw experience history.

The CPIL supports long-term career knowledge management by separating experience authority from Capability Knowledge authority while preserving traceability between them.

---

## Summary

The Capability Pattern & Insight Ledger is the authoritative CKF artifact for Capability Knowledge.

It remains downstream of the Master Experience Ledger and depends on the MEL for all experience authority.

Every CPIL capability must trace back to one or more MEL entries.

Supporting evidence improves transparency and confidence, but evidence does not create experience authority and is not required when a capability is reasonably derived from an authoritative MEL entry.

The CPIL provides the structured Capability Knowledge foundation used by downstream assessment, resume generation, and future career artifacts.
