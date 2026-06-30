# Knowledge Object Specification

**Document Version:** 1.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Document Type:** Technical Specification  
**Status:** Stable  
**Last Updated:** June 2026

---

## Table of Contents

1. Introduction
2. Knowledge Object Concept
3. Core Metadata
4. Standard Sections
5. Structural Requirements
6. Content Guidelines
7. Quality Checklist
8. Storage & Versioning
9. Examples by Category

---

## 1. Introduction

### 1.1 Purpose

The **Knowledge Object Specification** defines the standard structure, content requirements, and formatting guidelines for all knowledge objects within SDKA.

This specification ensures:
- **Consistency** — All objects follow the same structure
- **Completeness** — Nothing essential is missed
- **Retrievability** — Objects can be searched and discovered
- **Interconnection** — Objects can link to related content
- **Reusability** — Content can be easily adapted for different platforms

### 1.2 Who Uses This Specification

- **Researchers** — Creating new knowledge objects
- **Editors** — Reviewing objects for compliance
- **Content Teams** — Adapting objects for publications
- **Developers** — Building systems that work with knowledge objects
- **Curators** — Managing the knowledge repository

---

## 2. Knowledge Object Concept

### 2.1 Definition

A **Knowledge Object** is a self-contained unit of knowledge that:

- Addresses a single primary topic or question
- Is complete and understandable on its own
- Is sourced and verifiable
- Connects to related objects
- Can be formatted for multiple platforms
- Maintains its integrity across reuse

### 2.2 Knowledge Object Categories

| Category | Definition | Examples |
|----------|-----------|----------|
| **Deity** | A divine being or manifestation | Ganesha, Devi, Shiva, Durga |
| **Text** | A scriptural or literary work | Vedas, Bhagavad Gita, Puranas |
| **Temple** | A place of worship and pilgrimage | Kashi Vishwanath, Meenakshi Temple |
| **Ritual** | A prescribed ceremonial practice | Puja, Yajna, Aarti |
| **Philosophy** | A school of thought or worldview | Advaita, Dvaita, Kashmir Shaivism |
| **Tradition** | A regional or lineage-based practice | Bengali tradition, Samaveda practice |
| **Geography** | A sacred place or region | Kashi, Mount Kailash, Ganga Valley |
| **Practice** | A living custom or technique | Mantra chanting, Meditation, Yoga |
| **Concept** | An idea or principle | Dharma, Karma, Brahman |
| **Manuscript** | A rare or ancient text | Palm leaf manuscript, Temple manuscript |
| **Festival** | A celebratory or observance day | Diwali, Navaratri, Maha Shivaratri |
| **Symbol** | A meaningful visual or abstract representation | Aum, Swastika, Chakra |
| **Lineage** | An established school or teacher succession | Shankara Lineage, Gaudiya Sampradaya |

### 2.3 Knowledge Object Scope

**What should be a single object:**
- One primary topic
- Related subtopics that clarify the main topic
- Core information someone needs to understand the topic
- Multiple perspectives on that one topic

**What should be separate objects:**
- A different primary topic (even if related)
- Information that stands alone
- A variant that deserves separate exploration
- A historical period or version that warrants distinct treatment

**Example:**
- "Ganesha" = one object
- "Ganesha worship in Bengal" = could be separate or subsection depending on depth
- "Ganesha and Shiva's relationship" = separate object

---

## 3. Core Metadata

Every knowledge object MUST include this metadata:

```markdown
---
title: [Official name of topic]
category: [Primary category from list above]
related_categories: [Any secondary categories]
status: draft|reviewed|verified|final
date_created: YYYY-MM-DD
date_updated: YYYY-MM-DD
complexity_level: beginner|intermediate|advanced
content_length: brief|standard|comprehensive
researcher: [Name/Team]
reviewer: [Editor name, if reviewed]
---
```

### 3.1 Metadata Field Definitions

| Field | Values | Guidance |
|-------|--------|----------|
| **title** | Text | Official, recognizable name for the topic |
| **category** | From list | Primary subject category |
| **related_categories** | List | Other relevant categories |
| **status** | draft/reviewed/verified/final | Current workflow stage |
| **date_created** | Date | When first written |
| **date_updated** | Date | When last edited |
| **complexity_level** | beginner/intermediate/advanced | Prerequisite knowledge needed |
| **content_length** | brief/standard/comprehensive | Depth of coverage |
| **researcher** | Name | Who created this object |
| **reviewer** | Name | Who verified accuracy |

---

## 4. Standard Sections

Every knowledge object should include these sections (adapt as needed for category):

### 4.1 Essential Sections (Required)

#### 1. Summary / Overview (50-150 words)

**Purpose:** Answer "What is this?" in one short paragraph.

**Should contain:**
- Clear definition
- Why it matters
- Scope of coverage
- Key characteristics

**Example for Ganesha:**
> Ganesha is the elephant-headed deity revered as the remover of obstacles and the lord of beginnings in Hindu tradition. Worshipped across India and beyond, Ganesha appears in the Vedas, Puranas, and regional traditions with varying mythologies and practice. This object covers scriptural basis, iconography, worship practices, and regional variations.

#### 2. Etymology & Names

**Purpose:** Explain the name(s) and their origins.

**Should contain:**
- Meaning of primary name
- Alternative names/titles
- Sanskrit transliteration
- Linguistic or cultural significance

#### 3. Core Content / Main Information

**Purpose:** The heart of the object—central knowledge organized logically.

**Structure:**
- Organize hierarchically (general to specific)
- Use subsections for clarity
- Define specialized terms
- Build complexity gradually
- Provide examples where helpful

**Varies by category:**
- **Deity** — Mythology, scriptural sources, iconography, attributes
- **Text** — Structure, authorship, major themes, key concepts
- **Temple** — History, architecture, primary deity, main rituals
- **Ritual** — Steps, scriptural basis, symbolism, regional variations
- **Philosophy** — Core concepts, foundational texts, key thinkers

#### 4. Scriptural & Historical Basis

**Purpose:** Ground the topic in authoritative sources.

**Should contain:**
- Primary sources (Vedas, Puranas, Agamas)
- Historical records or inscriptions
- Scholarly references
- Evidence of antiquity
- Cross-cultural or comparative references

**Format:**
> According to [Scripture], [specific citation], [quotation or summary].
> 
> This teaching is further elaborated in [Related text].

#### 5. Iconography & Representation

**Purpose:** Describe how the topic is visually represented (for deities, symbols, etc.)

**Should contain:**
- Visual description
- Symbolic meanings
- Regional variations
- Associated colors, objects, animals
- Artistic conventions

**Note:** Not all categories need this section.

### 4.2 Strongly Recommended Sections

#### 6. Regional Variations

**Purpose:** Document how the topic differs by region/tradition.

**Should contain:**
- Geographic variations
- Theological differences
- Practical variations
- Regional specializations
- Why differences exist

**Structure:**
- Organize by region (North/South/East/West/Central)
- Note primary sources for each variation
- Explain theological or historical reasons

#### 7. Contemporary Practice

**Purpose:** Explain how this is practiced or understood today.

**Should contain:**
- Modern observance
- How traditions have evolved
- Differences between traditional and popular practice
- Current regional practices
- Living tradition documentation

#### 8. Related Knowledge

**Purpose:** Connect to related objects.

**Should contain:**
```
## Related Topics

- [Related Topic 1] — Why related
- [Related Topic 2] — How it connects
- [Related Topic 3] — Contextual relationship

## Part of Larger Topics
- [Parent Topic]

## Contains / Subtopics
- [Sub-topic 1]
- [Sub-topic 2]

## Contrasts With / Alternative Views
- [Alternative concept]
```

### 4.3 Optional Sections (Use as Needed)

#### Sources & Disagreements

**When to use:** If there's significant scholarly debate or tradition disagreement

**Should contain:**
- What scholars disagree on
- Why they disagree
- Evidence for each position
- How traditions resolve differences
- Areas of genuine uncertainty

#### Symbols & Attributes

**When to use:** For deities, spiritual concepts, practices

**Should contain:**
- Associated symbols
- Symbolic meanings
- Associated objects
- Ritual implements
- Color associations

#### Timeline / Historical Development

**When to use:** For topics with significant historical evolution

**Should contain:**
- Earliest attestations
- Major developments
- Key historical moments
- Evolution of understanding
- Major period/region innovations

#### Bibliography / Extended References

**When to use:** For comprehensive objects with extensive sources

**Should contain:**
- Full citations for all sources
- Recommended reading
- Academic works
- Accessible popular works
- Related primary texts

---

## 5. Structural Requirements

### 5.1 Document Format

**File Format:** Markdown (.md)

**Naming Convention:**
```
[Category]_[Topic_Name].md

Examples:
- Deity_Ganesha.md
- Temple_KashiVishwanath.md
- Philosophy_Advaita.md
- Ritual_Puja.md
```

**File Location:**
- Store in appropriate `/knowledge/` subfolder
- Use English file names (with underscores for spaces)
- Use singular forms where possible

### 5.2 Heading Hierarchy

```markdown
# [Topic Title]         (Primary heading - file title)

## Major Section        (Secondary heading)

### Subsection         (Tertiary heading)

#### Sub-subsection   (Quaternary - use sparingly)
```

**Maximum depth:** 4 levels (rarely need 4th level)

### 5.3 Text Formatting

**Use formatting for clarity:**
- **Bold** for key terms and definitions
- *Italics* for Sanskrit terms, emphasis
- `Code` for specific technical terms or transliterations
- > Blockquotes for important quotations

**Example:**
> The **Bhagavad Gita** (*Bhagavadgītā*), also known as the *Gita*, is a 700-verse Sanskrit scripture...

### 5.4 Lists and Tables

**Use for organization:**
- Bullet lists for collections
- Numbered lists for sequences
- Tables for comparisons
- Definition lists for term glossaries

**Table example:**
```markdown
| Region | Practice | Source |
|--------|----------|--------|
| North | [Variation 1] | [Source] |
| South | [Variation 2] | [Source] |
```

### 5.5 Cross-References

**Format:**
```markdown
[Topic Name](path/to/file.md)
[Topic Name with custom text](path/to/file.md)
```

**Examples:**
```markdown
See also: [Shiva](../deities/Shiva.md), [Puja](../rituals/Puja.md)

This practice is described in [Puja rituals](../rituals/Puja.md).
```

---

## 6. Content Guidelines

### 6.1 Tone & Voice

**Required tone:**
- Scholarly but accessible
- Respectful to traditions
- Neutral on disputed matters
- Authoritative but humble about uncertainties
- Never condescending

**Examples:**

✅ GOOD: "While the Vedas contain [X], regional traditions developed [Y]. Scholars debate whether [Z]."

✅ GOOD: "Tradition holds that [X], though historical evidence suggests [Y]. Both perspectives remain valid within different frameworks."

❌ BAD: "Despite what everyone thinks, the truth is actually [X]."

❌ BAD: "This superstition involves [X]."

### 6.2 Citation Requirements

**Every factual claim must be traceable:**

**For specific quotes:**
```
"Direct quote here" (Source Name, Section/Page, Translation note)
```

**For paraphrased ideas:**
```
According to [Source Name], the concept developed from [description]. (Source Name, Location)
```

**Create a Sources section:**
```markdown
## Sources

1. **Vedic sources**
   - Rigveda, Mandala X, Sukta 90 (Purusha Sukta)
   - Translation: [Which translation used]

2. **Puranic sources**
   - Srimad Bhagavata Purana, Canto I
   - [Specific verses referenced]

3. **Scholarly works**
   - Author Name, *Book Title* (Publication details)
   - Accessed: [Date if online]
```

### 6.3 Sanskrit Transliteration

**Standard:** Use IAST (International Alphabet of Sanskrit Transliteration)

**Common diacritics:**
- ā, ī, ū (long vowels)
- ṁ, ṇ, ṅ, ñ (nasal consonants)
- ṣ, ṭ, ḍ (retroflex consonants)

**First mention:**
- Provide both Sanskrit and English
- Use italics: *Bhagavad Gītā* or *Bhagavadgītā*

**Subsequent mentions:**
- English acceptable after first mention
- Can alternate between forms for flow

### 6.4 Defining Specialized Terms

**For first mention of specialized terms:**

**Example 1:**
> The *Purana* (traditional narrative) texts...

**Example 2:**
> An *Agama* is a scriptural tradition that...

**For complex concepts, use a glossary:**
```markdown
## Key Terms

- **Agama** — A scriptural tradition emphasizing [definition]
- **Mantra** — A sacred sound formula used in [context]
```

### 6.5 Managing Uncertainty

**Use precise language:**

| Certainty Level | Language |
|-----------------|----------|
| High certainty | "The earliest texts state...", "Archaeological evidence shows..." |
| Medium certainty | "Tradition holds that...", "The dominant view is..." |
| Scholarly debate | "Scholars debate whether...", "Some traditions hold..., others believe..." |
| Low certainty | "There is no clear evidence that...", "This remains unknown in available sources" |
| Popular belief | "Popular tradition claims...", "Some communities believe..." |

---

## 7. Quality Checklist

Before submitting a knowledge object, verify:

### Content Quality
- [ ] Topic is clearly defined in the summary
- [ ] Core content is accurate and well-sourced
- [ ] All major aspects of the topic are covered
- [ ] Specialized terms are defined
- [ ] Uncertainty is acknowledged
- [ ] Multiple viewpoints are presented (where relevant)
- [ ] Examples clarify complex concepts

### Source & Citation
- [ ] All factual claims are cited
- [ ] Primary sources are used (where available)
- [ ] Quotes are accurate and in context
- [ ] Citations include page/verse numbers
- [ ] Translation versions are noted
- [ ] Sources section is complete

### Structure & Organization
- [ ] Heading hierarchy is correct
- [ ] Sections are logically ordered
- [ ] Complex ideas are broken into subsections
- [ ] Transitions between sections flow
- [ ] Related topics are clearly cross-referenced

### Language & Tone
- [ ] Tone is scholarly but accessible
- [ ] No unnecessary jargon
- [ ] Respectful to traditions discussed
- [ ] Neutral on disputed matters
- [ ] No condescending language

### Formatting
- [ ] Markdown formatting is correct
- [ ] Lists are used for clarity
- [ ] Tables are well-organized
- [ ] Cross-references use proper formatting
- [ ] Sanskrit terms are properly transliterated
- [ ] File name follows naming convention

### Metadata
- [ ] All metadata fields are complete
- [ ] Status field is set correctly
- [ ] Category is accurate
- [ ] Related categories included
- [ ] Complexity level appropriate
- [ ] Length designation accurate

---

## 8. Storage & Versioning

### 8.1 File Storage

**Location by category:**
```
/knowledge/
├── texts/
│   └── veda/
│   └── purana/
│   └── agama/
├── deities/
│   ├── shiva/
│   ├── vishnu/
│   ├── devi/
│   └── ...
├── temples/
├── rituals/
├── philosophy/
├── ...
```

**File naming example:**
```
/knowledge/deities/ganesha/Deity_Ganesha.md
/knowledge/temples/jyotirlinga/Temple_SomnathJyotirlinga.md
/knowledge/philosophy/Samkhya.md
```

### 8.2 Version Control

**Track changes using Git:**
- Commit messages should describe changes
- Major revisions warrant version number updates
- Use meaningful commit comments:
  - "Added regional variations to Ganesha"
  - "Corrected Vedic citation in Samkhya"
  - "Expanded Puja structure section"

**Metadata versioning:**
```
---
title: [Topic]
version: 1.0
date_updated: 2026-06-30
previous_versions:
  - 0.9 (2026-06-15)
---
```

### 8.3 Archival & Preservation

**Format considerations:**
- Markdown chosen for longevity
- No proprietary formats
- Plain text readable in any era
- Version control maintains history
- Regular backups essential

---

## 9. Examples by Category

### 9.1 Example: Deity Object

```markdown
# Ganesha

---
title: Ganesha
category: Deity
related_categories: [iconography, symbols, worship, festivals]
status: verified
date_created: 2026-01-15
date_updated: 2026-06-20
complexity_level: intermediate
content_length: comprehensive
researcher: [Name]
reviewer: [Editor]
---

## Summary

**Ganesha** (*Gaṇeśa*) is the elephant-headed deity revered as the remover of obstacles, the lord of beginnings, and the guardian of thresholds in Hindu tradition. Worshipped across India and by Hindu communities worldwide, Ganesha appears in the Vedas, Puranas, and regional traditions with varying mythologies and worship practices. This object covers Ganesha's scriptural basis, mythology, iconography, worship patterns, and regional variations.

## Etymology & Names

The name *Gaṇeśa* derives from...

[Continue with other sections...]
```

### 9.2 Example: Temple Object

```markdown
# Kashi Vishwanath Temple

---
title: Kashi Vishwanath Temple
category: Temple
related_categories: [pilgrimage, jyotirlinga, sacred_geography]
status: verified
date_created: 2026-02-01
date_updated: 2026-06-20
complexity_level: intermediate
content_length: comprehensive
researcher: [Name]
reviewer: [Editor]
---

## Summary

The **Kashi Vishwanath Temple** in Varanasi is one of the most sacred shrines in Hinduism and one of the twelve Jyotirlingas. Located on the western bank of the Ganga River...

[Continue with sections on History, Architecture, Deity, Rituals, Sacred Significance, Contemporary Practice, etc.]
```

### 9.3 Example: Ritual Object

```markdown
# Puja (Worship Ritual)

---
title: Puja
category: Ritual
related_categories: [worship, practice, symbolism]
status: verified
date_created: 2026-01-20
date_updated: 2026-06-20
complexity_level: beginner
content_length: standard
researcher: [Name]
reviewer: [Editor]
---

## Summary

**Puja** (*Pūjā*) is a Hindu worship ritual in which devotees make offerings to deities and ask for blessings. Performed in temples, homes, and other sacred spaces, puja forms the central devotional practice across Hindu traditions and includes various forms based on region, tradition, and deity worshipped.

[Continue with sections on Scriptural Basis, Core Structure, Elements and Offerings, Regional Variations, etc.]
```

---

## Conclusion

The Knowledge Object Specification provides a unified framework for creating, reviewing, and maintaining knowledge objects within SDKA. This standardization ensures that all knowledge objects meet high quality standards while remaining flexible enough to accommodate the diverse forms of knowledge within Sanātana Dharma and Indic Knowledge Systems.

Following this specification consistently builds a coherent, interconnected, and authoritative knowledge archive.
