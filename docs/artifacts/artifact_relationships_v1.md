# CKF Artifact Relationships

**Framework:** Career Knowledge Framework (CKF)  
**Version:** 1.0  
**Status:** Draft – Architectural Specification

---

# Purpose

The Career Knowledge Framework (CKF) is composed of a series of governed artifacts.

Each artifact has a single, well-defined responsibility and consumes information from upstream artifacts while producing information for downstream artifacts.

This document defines those relationships and establishes the authoritative flow of information throughout the framework.

---

# Design Philosophy

CKF is based on a simple architectural principle:

> **Collect information once. Interpret it once. Present it many times.**

Every artifact exists to perform one responsibility.

Artifacts should never duplicate the responsibilities of other artifacts.

---

# Artifact Hierarchy

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

Supporting evidence may be associated with experiences throughout the framework but does not replace the authoritative role of the MEL.

---

# Artifact Responsibilities

## Master Experience Ledger (MEL)

Purpose:

Maintain the authoritative record of an individual's experiences.

Consumes:

* Personal experience
* Supporting evidence (optional)
* Historical records
* User revisions

Produces:

* Authoritative experience information

May NOT:

* Assess capability
* Recommend careers
* Optimize resumes
* Infer strengths

---

## Capability Pattern & Insight Ledger (CPIL)

Purpose:

Derive, organize, relate, preserve, and describe Capability Knowledge from MEL experience records.

Consumes:

* MEL

Produces:

* Capability patterns
* Capability insights
* Capability records
* Capability relationships

May NOT:

* Modify MEL
* Assess capability meaning, strength, or transferability
* Evaluate career suitability
* Generate resumes

---

## Career Capability Assessment (CCA)

Purpose:

Interpret, assess, evaluate, and explain the meaning of Capability Knowledge.

Consumes:

* CPIL

Produces:

* Capability assessments
* Transferable capability analysis
* Development observations
* Career alignment analysis

May NOT:

* Modify MEL
* Modify CPIL
* Derive new Capability Knowledge
* Generate resumes

---

## Resume Generation Framework (RGF)

Purpose:

Transform authoritative career knowledge into presentation-specific career artifacts.

Consumes:

* MEL
* CPIL
* CCA
* Position requirements

Produces:

* Targeted resumes
* Cover letters
* Interview preparation
* LinkedIn recommendations
* Professional summaries

May NOT:

* Modify upstream artifacts

---

# Authority Flow

Authority flows in one direction.

```text
MEL
Experience Authority
 |
 v
CPIL
Capability Knowledge Authority
 |
 v
CCA
Interpretation & Assessment Authority
 |
 v
RGF
Presentation Transformation Authority
 |
 v
Career Artifacts
```

Downstream artifacts may consume upstream information.

They may never replace or redefine upstream information.

---

# Evidence

Evidence is a supporting capability of the framework rather than an independent authoritative artifact.

Evidence may include:

* Documents
* Images
* Videos
* Certificates
* Publications
* Git repositories
* Project artifacts
* Employment records
* Other supporting material

Evidence strengthens transparency and traceability.

The absence of evidence does not prevent an experience from being represented within the MEL.

---

# Derived Artifacts

The framework supports many downstream artifacts beyond resumes.

Examples include:

* LinkedIn profiles
* Professional biographies
* Portfolios
* Job applications
* Capability reports
* Interview preparation
* Career summaries
* AI-assisted career guidance

Each is considered a presentation artifact derived from authoritative upstream knowledge.

---

# Architectural Principles

CKF follows several architectural principles:

* Single authoritative source for experience.
* Single responsibility per artifact.
* Downstream artifacts are derivative.
* Upstream artifacts remain authoritative.
* Traceability is preserved throughout the framework.
* Supporting evidence strengthens, but does not define, experience.
* Presentation never changes authority.

---

# Future Expansion

Future framework artifacts should integrate into this architecture without violating the authority chain.

New artifacts should consume existing authoritative information rather than introducing competing sources of truth.

The long-term objective is to create a scalable knowledge architecture capable of representing professional experience while preserving consistency, provenance, and long-term maintainability.
