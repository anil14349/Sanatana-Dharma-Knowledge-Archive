# SDKA Knowledge Object Template
**File:** docs/05_Knowledge_Object_Template.md

Version: 1.0.0  
Status: Active Standard

---

# Purpose

This document defines the standard structure for every **Knowledge Object (KO)** in the Sanatana Dharma Knowledge Archive (SDKA).

Every Knowledge Object must follow this template to ensure consistency, traceability, maintainability, and future automation.

A Knowledge Object is the canonical unit of knowledge within SDKA. All content (Instagram, YouTube, website, books, podcasts, etc.) must be derived from a validated Knowledge Object.

---

# Knowledge Package Structure

```text
knowledge-objects/
└── <category>/
    └── KO-XXXX-Topic/
        ├── README.md
        ├── metadata.yaml
        ├── primary-sources.md
        ├── architecture.md          (optional)
        ├── ritual.md                (optional)
        ├── historical-development.md
        ├── symbolism.md
        ├── living-traditions.md
        ├── regional-variations.md   (optional)
        ├── misconceptions.md
        ├── evidence-matrix.md
        ├── bibliography.md
        ├── knowledge-graph.md
        ├── CHANGELOG.md
        └── content/
            ├── instagram.md
            ├── youtube.md           (optional)
            ├── website.md           (optional)
            └── shorts.md            (optional)
```

---

# Required Metadata

Each Knowledge Object must include:

- Knowledge Object ID
- Title
- Alternate titles
- Category
- Subcategory
- Version
- Status
- Research Maturity
- Confidence Level
- Primary Tradition
- Related Knowledge Objects
- Keywords
- Last Reviewed Date

---

# Mandatory Repository Files

| File | Required | Purpose |
|------|----------|---------|
| README.md | ✅ | Canonical overview |
| metadata.yaml | ✅ | Structured metadata |
| primary-sources.md | ✅ | Primary textual evidence |
| evidence-matrix.md | ✅ | Claim validation |
| bibliography.md | ✅ | References |
| knowledge-graph.md | ✅ | Semantic relationships |
| CHANGELOG.md | ✅ | Version history |

The remaining files are included where applicable.

---

# Research Workflow

Every Knowledge Object progresses through the following stages:

1. Topic Selection
2. Preliminary Research
3. Source Collection
4. Evidence Validation
5. Knowledge Object Draft
6. Evidence Audit
7. Repository Review
8. Freeze (R3)
9. Content Production
10. Continuous Updates

---

# Writing Standards

- Write in clear, neutral language.
- Distinguish evidence from interpretation.
- Avoid unsupported universal claims.
- Document regional variation explicitly.
- Respect Guru-parampara and temple-specific traditions.
- Record research gaps instead of making assumptions.

---

# Evidence Requirements

Every major statement should include:

- Evidence Level (A–D)
- Confidence Rating
- Source Type
- Verification Status

Unsupported claims should be documented as such.

---

# Knowledge Graph Requirements

Each Knowledge Object must:

- Link to related Knowledge Objects.
- Define new concepts introduced.
- Record relationships with rituals, scriptures, temples, people, and philosophy.

---

# Content Derivation

No content should be created directly from research notes.

Pipeline:

Research Notes
↓
Knowledge Object
↓
Evidence Audit
↓
Frozen (R3)
↓
Instagram
↓
YouTube
↓
Website
↓
Books

---

# Research Maturity Model

| Level | Meaning |
|------|---------|
| R0 | Idea |
| R1 | Preliminary Research |
| R2 | Evidence Validated |
| R3 | Repository Ready |
| R4 | Published |
| R5 | Living Document |

---

# Versioning Policy

- MAJOR: Structural changes.
- MINOR: New validated research.
- PATCH: Corrections and editorial improvements.

Example:

- 1.0.0 — Initial release
- 1.1.0 — New evidence
- 1.1.1 — Editorial fixes

---

# Quality Gate

A Knowledge Object must pass:

- Evidence Audit Checklist
- Repository Review
- Metadata Validation
- Knowledge Graph Review

before being marked **Frozen**.

---

# Future Enhancements

Future SDKA versions may add:

- Automated metadata validation.
- Schema-based verification.
- AI-assisted cross-linking.
- Website generation.
- Knowledge graph visualization.
- RAG indexing.

---

# Changelog

## v1.0.0

- Initial Knowledge Object Template.
- Established the standard structure and workflow for all future SDKA Knowledge Objects.
