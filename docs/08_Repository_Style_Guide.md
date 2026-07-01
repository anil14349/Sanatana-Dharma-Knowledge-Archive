# SDKA Repository Style Guide
**File:** docs/08_Repository_Style_Guide.md

Version: 1.0.0  
Status: Active Standard

---

# Purpose

This style guide defines the editorial, structural, and technical standards for every document in the Sanatana Dharma Knowledge Archive (SDKA). It ensures consistency across researchers, contributors, and AI-assisted workflows.

---

# Guiding Principles

1. Evidence before opinion.
2. Respect diversity within Sanatana Dharma.
3. Separate fact, interpretation, and living tradition.
4. Prefer clarity over complexity.
5. Document uncertainty explicitly.

---

# Repository Structure

```text
docs/
knowledge-objects/
research-notes/
templates/
assets/
```

Use lowercase file names with hyphens where practical. Knowledge Object folders retain their canonical IDs.

---

# Naming Standards

Knowledge Objects:

```text
KO-RITUAL-0001-Chandi-Pradakshina
KO-TEMPLE-0001-Brihadeeswarar
KO-PERSON-0001-Chandikeshvara
```

Supporting files:

```text
README.md
metadata.yaml
primary-sources.md
evidence-matrix.md
knowledge-graph.md
```

---

# Markdown Standards

- One H1 (`#`) per document.
- Use H2 (`##`) for major sections.
- Use tables for structured comparisons.
- Use fenced code blocks for directory trees and diagrams.
- Keep paragraphs concise.

---

# Front Matter

Knowledge Objects should include YAML metadata:

```yaml
id:
title:
category:
version:
status:
research_maturity:
confidence:
last_reviewed:
```

---

# Writing Style

Use:

- Neutral, precise language.
- Present tense where appropriate.
- Sanskrit terms with English explanation on first use.
- Consistent terminology throughout a document.

Avoid:

- Clickbait.
- Absolute statements without evidence.
- Sectarian language.
- Sensationalism.

---

# Evidence Formatting

Major claims should identify:

- Evidence Level (A–D)
- Confidence
- Source Type

Clearly distinguish:

- Scriptural evidence
- Scholarly interpretation
- Living tradition
- Folklore

---

# Tables & Diagrams

Preferred for:

- Timelines
- Evidence matrices
- Regional comparisons
- Temple layouts
- Knowledge graphs

ASCII diagrams are acceptable until vector graphics are available.

---

# Cross-Linking

Each Knowledge Object should reference:

- Related Knowledge Objects
- Shared concepts
- Relevant scriptures
- Temple architecture
- Research methodology documents

---

# Citations

Prefer:

1. Primary sources.
2. Critical editions.
3. Peer-reviewed scholarship.
4. Temple documentation.

Blogs and social media are discovery sources only unless independently verified.

---

# Versioning

Semantic Versioning:

- MAJOR – structural changes
- MINOR – new validated research
- PATCH – editorial fixes

Record every change in `CHANGELOG.md`.

---

# AI Collaboration

AI-generated content must:

- Follow this style guide.
- Pass the Evidence Audit Checklist.
- Be reviewed before being marked Repository Ready.
- Never invent citations or quotations.

---

# Publication Readiness

Before publishing:

- Knowledge Object at R3 or above.
- Evidence reviewed.
- Metadata complete.
- Cross-links updated.
- Content derived through the official workflow.

---

# Changelog

## v1.0.0

Initial repository-wide style guide.
