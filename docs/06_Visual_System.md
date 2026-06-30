# Visual System & Design Guidelines

**Document Version:** 1.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Document Type:** Design Specification  
**Status:** Active  
**Last Updated:** June 2026

---

## Table of Contents

1. Visual Philosophy
2. Design Principles
3. Color System
4. Typography Guidelines
5. Page Archetypes
6. Visual Content Guidelines
7. Platform-Specific Guidelines
8. Visual Quality Standards

---

## 1. Visual Philosophy

### 1.1 Core Purpose

The visual system serves SDKA's mission by:

**Authentic Representation**
- Honor traditional iconography
- Respect cultural and sacred symbolism
- Represent diversity of traditions accurately
- Avoid appropriation or distortion

**Beautiful Communication**
- Make complex knowledge visually accessible
- Create visual engagement without distraction
- Support rather than replace content
- Appeal to educated audiences

**Consistent Experience**
- Unified visual identity across platforms
- Recognize SDKA content instantly
- Build brand trust and credibility
- Enable easy content discovery

**Inclusive Presentation**
- Accessible color and contrast
- Support multiple learning styles
- Readable at various sizes
- Respectful representation of all traditions

### 1.2 Visual Hierarchy

SDKA's visual language respects a hierarchy of importance:

```
Authenticity & Accuracy (Highest)
    ↓
Cultural Respect
    ↓
Educational Clarity
    ↓
Visual Beauty
    ↓
Brand Consistency
    ↓
Aesthetic Polish (Lowest, but important)
```

**Principle:** Never sacrifice accuracy, respect, or clarity for beauty or brand consistency.

---

## 2. Design Principles

### 2.1 Core Design Principles

**Principle 1: Respect Sacred Imagery**

- Treat sacred symbols with reverence
- Follow traditional iconography conventions
- Avoid casual or humorous treatment of sacred topics
- Acknowledge regional variations in representation
- Never mock or trivialize spiritual content

**Principle 2: Visual Authenticity**

- Use historically accurate architectural representations
- Reference authentic traditional art styles
- Cite sources for artistic choices
- When uncertain, err toward historical accuracy
- Document artistic interpretive choices

**Principle 3: Clear Hierarchy**

- Primary elements stand out clearly
- Secondary information doesn't compete
- Visual flow guides reader's eye
- Emphasis supports understanding
- Complexity revealed progressively

**Principle 4: Consistent Visual Language**

- Recognize SDKA content instantly
- Consistent use of design elements
- Unified typography and spacing
- Recognizable color application
- Familiar structural patterns

**Principle 5: Cultural Sensitivity**

- Represent all traditions respectfully
- Avoid stereotyping or caricature
- Use appropriate symbolism correctly
- Respect regional variations
- Acknowledge different interpretations

**Principle 6: Accessibility**

- Sufficient color contrast
- Readable at all sizes
- Not dependent on color alone
- Support screen readers and assistive tech
- Clear hierarchy for all users

---

## 3. Color System

### 3.1 Primary Color Palette

**Saffron** #FF6B35
- Traditional Indian color
- Represents spirituality and auspiciousness
- Primary brand color
- Used for primary CTAs and highlights

**Deep Blue** #003D82
- Represents the divine and cosmos
- Used for secondary elements
- Supports clear contrast
- Professional and authoritative

**Cream** #F5E6D3
- Warm, accessible background
- Respects readability
- Calming and sophisticated
- Supports paper-like reading experience

**Charcoal** #2C2C2C
- Primary text color
- High contrast for accessibility
- Professional appearance
- Easy to read at all sizes

### 3.2 Sacred Symbol Colors

**Traditional associations:**

| Color | Association | Usage |
|-------|-------------|-------|
| Saffron | Spirituality, auspiciousness | Positive elements, spiritual topics |
| White | Purity, peace | Clean backgrounds, sacred contexts |
| Red | Energy, transformation | Important elements, rituals |
| Blue | Divine, cosmic | Philosophical topics, Vishnu |
| Yellow/Gold | Wealth, wisdom | Precious knowledge, Lakshmi |
| Green | Fertility, growth | Nature-based topics, growth |
| Black | Mystery, dissolution | Kali, transformation, grounding |

**Guidance:**
- Use traditional color associations when appropriate
- Respect cultural color significance
- Apply consistently across similar topics
- Consider readability and accessibility
- Avoid color as only distinguishing factor

### 3.3 Color Accessibility

**Required standards:**
- Minimum 4.5:1 contrast ratio for text on background
- 3:1 contrast for large text (18pt+)
- Test with color-blind simulation tools
- Never use color alone to convey meaning
- Provide pattern or text alternatives

**Color combinations to avoid:**
- Red/green only (red-green colorblindness)
- Light red/light green
- Blue/yellow where contrast is insufficient

---

## 4. Typography Guidelines

### 4.1 Typeface Selection

**Primary Typeface: Serif** (for body and most content)
- Conveys authority and tradition
- Easiest to read in longer text
- Professional appearance
- Examples: Garamond, EB Garamond, Crimson Text

**Secondary Typeface: Sans-serif** (for UI elements and headers)
- Clean and modern
- Clear at small sizes
- Examples: Inter, Open Sans, Lato

**Specialty: Decorative** (for Sanskrit and special contexts)
- Traditional Sanskrit fonts when possible
- Sparingly, for special emphasis
- Always readable and intentional

### 4.2 Type Sizes

**Hierarchy:**

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Main heading | 32-40pt | Bold | Article/page title |
| Section heading | 24-28pt | Bold | Major sections |
| Subsection | 18-20pt | Semibold | Subsections |
| Body text | 14-16pt | Regular | Main content |
| Secondary text | 12-13pt | Regular | Captions, metadata |
| Small text | 11-12pt | Regular | Footnotes, fine print |

**Responsive scaling:**
- Scale proportionally on mobile
- Maintain hierarchy on all devices
- Readable at minimum 14pt on mobile
- Desktop: 16pt body text standard

### 4.3 Sanskrit Transliteration

**Display standards:**
- Use proper IAST diacritics: ā, ī, ū, ṁ, ṇ, ṭ, ḍ, ṣ
- Italicize Sanskrit words: *Bhagavad Gita*
- Provide English translation nearby
- Use clear, readable fonts that support diacritics

**Typography example:**
> The *Bhagavadgītā* (Bhagavad Gita in Sanskrit) teaches the concept of *Dharma*.

---

## 5. Page Archetypes

### 5.1 Deity Page Archetype

**Layout structure:**

```
┌─────────────────────────────────────┐
│ HEADER                               │
│ Deity Name | Category Badge | Date   │
└─────────────────────────────────────┘

┌─────────────────────────────────────┐
│                                      │
│  PRIMARY DEITY IMAGE / ARTWORK       │
│                                      │
│  (High-quality traditional art or    │
│   authenticated iconography)         │
│                                      │
└─────────────────────────────────────┘

SUMMARY SECTION
- 2-3 sentence overview
- Key characteristics
- Why this deity matters

MAIN CONTENT
[Sections with subheadings]
- Etymology & Names
- Mythology & Stories
- Iconography
- Worship & Devotion
- Regional Variations
- Sacred Texts

[SIDEBAR - Optional]
- Quick facts
- Associated symbols
- Key attributes
- Related deities

RELATED CONTENT
- Links to related deities
- Temples associated
- Texts mentioning
- Rituals for worship
```

### 5.2 Temple Page Archetype

**Layout structure:**

```
┌─────────────────────────────────────┐
│ HEADER                               │
│ Temple Name | Location | Tradition   │
└─────────────────────────────────────┘

GALLERY
- Exterior view
- Main sanctum
- Architectural details
- Festival images

QUICK INFO
- Location & directions
- Presiding deity
- Founding date
- Religious significance

MAIN CONTENT
[Sections with subheadings]
- History
- Architecture
- Main Deity & Worship
- Principal Rituals
- Festival Calendar
- Pilgrimage Information
- Geographic Significance

VISUAL TIMELINE
- Historical development
- Major renovations
- Significant events

PRACTICAL INFORMATION
- Visiting details
- Ritual times
- Accommodation nearby
- Related pilgrimage sites
```

### 5.3 Text/Scripture Page Archetype

**Layout structure:**

```
┌─────────────────────────────────────┐
│ HEADER                               │
│ Text Name | Type | Period            │
└─────────────────────────────────────┘

TEXT METADATA
- Author/Attribution
- Language & period
- Structure overview
- Translations available

SUMMARY SECTION
- What is this text?
- Historical significance
- Current relevance

STRUCTURE BREAKDOWN
[Visual organization]
- Parts/Cantos/Chapters
- Key passages
- Length & organization

MAJOR THEMES
- Central concepts
- Philosophical teachings
- Practical guidance
- Cultural impact

REPRESENTATIVE PASSAGES
- Important quotes
- With translations
- With context

INTERPRETATION TRADITIONS
- Different schools' views
- Historical interpretations
- Modern understanding

SCHOLARLY RESOURCES
- Academic studies
- Recommended readings
- Research materials
```

---

## 6. Visual Content Guidelines

### 6.1 Image Selection & Use

**Guidelines for all images:**

**Respect:**
- ✅ High-quality professional photographs
- ✅ Authenticated traditional artwork
- ✅ Scholarly illustration or recreation
- ❌ Casual or humorous imagery
- ❌ Cheap digital manipulation
- ❌ Disrespectful parody or mockery

**Authenticity:**
- ✅ Historical accuracy where available
- ✅ Attribution of artwork sources
- ✅ Acknowledgment of artistic interpretation
- ❌ Presenting modern work as ancient
- ❌ Altering sacred imagery
- ❌ Unattributed or stolen images

**Accessibility:**
- ✅ Alt text describing images
- ✅ Sufficient contrast and clarity
- ✅ Readable text within images
- ✅ Captions providing context
- ❌ Images as only source of information
- ❌ Inaccessible embedded text

### 6.2 Image Categories

**Photography**
- Temple exterior and interior
- Architectural details
- Regional landscapes
- Ritual practices
- Contemporary living traditions

**Traditional Artwork**
- Classical deity paintings
- Temple sculptures
- Manuscript illustrations
- Regional art styles
- Traditional iconography

**Scholarly Recreations**
- Artist renderings based on descriptions
- Archaeological reconstructions
- Historical period visualizations
- Clearly marked as recreation

**Information Graphics**
- Genealogies and family trees
- Timeline visualizations
- Geographic maps
- Theological diagrams
- Organizational charts

**Symbolic Illustrations**
- Sacred symbols
- Architectural elements
- Iconographic features
- Philosophical concepts

### 6.3 Visual Storytelling

**For Instagram/Social Media:**

**Page Archetypes:**

| Archetype | Purpose | Visual Style |
|-----------|---------|--------------|
| Quote/Wisdom | Inspiration | Elegant type on complementary background |
| Story | Narrative | Sequential images with unifying aesthetic |
| Infographic | Education | Clean, organized, colorful data viz |
| Compare/Contrast | Learning | Side-by-side visual comparison |
| History | Context | Timeline or progression visualization |
| How-To | Instruction | Step-by-step visual guide |

**Color application for carousel posts:**
- Saffron accent on first slide
- Consistent color theme through series
- White or cream backgrounds for readability
- Text color provides contrast
- Symbols and icons consistent

---

## 7. Platform-Specific Guidelines

### 7.1 Instagram Guidelines

**Image Dimensions:**
- Feed posts: 1080 x 1350px (4:5 ratio)
- Story: 1080 x 1920px (9:16 ratio)
- Reels: 1080 x 1920px (9:16 ratio)
- Carousel: 1080 x 1350px each slide

**Typography for Instagram:**
- 16-20pt minimum for readability
- Limit to 1-2 fonts per post
- High contrast text on background
- Avoid tiny text on photos

**Content Types:**
- Carousels (3-7 slides)
- Educational reels (15-60 seconds)
- Carousel stories (temporary)
- Quotes and wisdom posts
- Behind-the-scenes research
- Community engagement

**Visual Identity:**
- Consistent filter or color grading
- Recognizable header design
- Logo placement consistent
- Typography consistent
- Color palette carries through

### 7.2 YouTube Guidelines

**Thumbnail Design:**
- 1280 x 720px (16:9 ratio)
- Large, readable text (14pt+)
- High contrast and contrast
- Faces or compelling imagery
- Consistent branding elements
- Saffron and blue for SDKA identity

**Video Title Cards:**
- Consistent branding
- Readable at any size
- 2-3 seconds minimum display
- Transition effects minimal
- Typography consistent with brand

**Audio Considerations:**
- Music that honors sacred contexts
- Sound design that supports not distracts
- Clear audio mixing
- No disrespectful sound effects

### 7.3 Website Guidelines

**Typography:**
- 16pt body text standard
- Serif font for readability
- High contrast (dark text on light)
- Line height 1.6-1.8 for comfortable reading

**Color Application:**
- Saffron for CTAs and highlights
- Deep blue for secondary actions
- Cream for backgrounds
- Charcoal for text

**Navigation:**
- Clear category navigation
- Breadcrumb trails for location
- Related content suggestions
- Consistent sidebar/menu

**Layout:**
- Clean, uncluttered design
- Generous whitespace
- Single column for content
- Sidebar for supplementary info
- Responsive on all devices

---

## 8. Visual Quality Standards

### 8.1 Quality Checklist

Before publishing visual content:

**Content Quality**
- [ ] Image represents topic accurately
- [ ] No distortion or misrepresentation
- [ ] Respectful and appropriate
- [ ] High resolution (300dpi for print, 72dpi web min)
- [ ] Properly attributed/credited

**Design Quality**
- [ ] Color palette applied consistently
- [ ] Typography follows standards
- [ ] Visual hierarchy clear
- [ ] Professional appearance
- [ ] Aligned and properly spaced

**Accessibility**
- [ ] Alt text provided for all images
- [ ] Color contrast sufficient (4.5:1)
- [ ] Text readable at all sizes
- [ ] No essential information in image only
- [ ] Accessible to colorblind viewers

**Platform Optimization**
- [ ] Correct dimensions for platform
- [ ] File size optimized
- [ ] Loads quickly
- [ ] Looks good on mobile
- [ ] Metadata complete

**Brand Consistency**
- [ ] Recognizable as SDKA content
- [ ] Logo/branding applied correctly
- [ ] Typography consistent
- [ ] Color scheme followed
- [ ] Style coherent with archive

### 8.2 Image Optimization

**File Format Selection:**
- PNG for graphics and screenshots (transparency support)
- JPG for photographs (smaller file size)
- WebP for web (modern compression)
- SVG for logos and icons (scalable)

**File Size Standards:**
- Web images: <500KB typical
- Social media: <1MB
- Print: full resolution needed
- Thumbnails: <100KB

**Optimization Process:**
1. Export at appropriate size
2. Compress without visible quality loss
3. Test on multiple devices
4. Verify load time
5. Archive original high-resolution

---

## 9. Aesthetic Evolution

The visual system should evolve as:
- Project grows and matures
- Audience expectations change
- Design trends shift (while maintaining timelessness)
- Technological capabilities advance
- Community feedback informs improvements

**Principle:** Maintain consistency while allowing thoughtful evolution.

---

## Conclusion

The SDKA visual system balances beauty with authenticity, consistency with respect for diverse traditions, and polish with accessibility. Every visual choice should serve the mission of preserving and presenting authentic knowledge of Sanātana Dharma in its truest form.

The visual system enables SDKA content to be instantly recognizable, beautifully presented, and accessible to audiences across all platforms while maintaining the highest standards of cultural respect and intellectual integrity.
