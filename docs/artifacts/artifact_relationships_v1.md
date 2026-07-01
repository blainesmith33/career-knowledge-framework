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
      │
      ▼
Master Experience Ledger (MEL)
      │
      ▼
Capability Profile & Intelligence Ledger (CPIL)
      │
      ▼
Career Capability Assessment (CCA)
      │
      ▼
Resume Generation Framework (RGF)
      │
      ▼
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

## Capability Profile & Intelligence Ledger (CPIL)

Purpose:

Transform experiences into structured capability records.

Consumes:

* MEL

Produces:

* Capability inventory
* Capability relationships
* Capability classifications

May NOT:

* Modify MEL
* Evaluate career suitability
* Generate resumes

---

## Career Capability Assessment (CCA)

Purpose:

Analyze capabilities and identify meaningful patterns.

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
* Generate resumes

---

## Resume Generation Framework (RGF)

Purpose:

Transform authoritative career knowledge into presentation-specific artifacts.

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
 ↓
CPIL
 ↓
CCA
 ↓
RGF
 ↓
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
