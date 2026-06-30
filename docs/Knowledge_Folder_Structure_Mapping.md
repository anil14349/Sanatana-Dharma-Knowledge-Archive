# Knowledge Folder Structure & Category Mapping

**Document Version:** 1.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Document Type:** Reference Guide  
**Status:** Active  
**Last Updated:** June 2026

---

## Introduction

This document maps the `/knowledge/` folder structure to the knowledge categories defined in the Master Blueprint. It serves as a reference for:

- **Researchers** — Where to file new knowledge objects
- **Content creators** — Understanding topic organization
- **Developers** — How the knowledge repository is structured
- **Users** — How to navigate the archive

---

## Knowledge Folder Structure Overview

```
/knowledge/
├── acharyas/          → Lineage founders and teachers
├── agamas/            → Agama scriptures and practices
├── architecture/      → Temple and sacred architecture
├── astronomy/         → Jyotisha and celestial knowledge
├── ayurveda/          → Ayurvedic medicine and practice
├── deities/           → Gods, goddesses, manifestations
│   ├── devi/
│   ├── ganesha/
│   ├── hanuman/
│   ├── kartikeya/
│   ├── navagraha/
│   ├── other_deities/
│   ├── shiva/
│   ├── surya/
│   └── vishnu/
├── festivals/         → Celebrations and observances
├── iconography/       → Visual symbolism and representation
├── indian_knowledge_systems/ → Scientific & philosophical systems
├── mantras/           → Sacred sounds and formulas
├── manuscripts/       → Rare texts and palm leaf collections
├── mathas/            → Monastic institutions
├── philosophy/        → Schools of thought and Darshanas
├── pilgrimage/        → Sacred sites and pilgrimage routes
├── regional/          → Regional and tribal traditions
│   ├── andhra_pradesh/
│   ├── assam/
│   ├── bengal/
│   ├── gujarat/
│   ├── himalaya/
│   ├── karnataka/
│   ├── kashmir/
│   ├── kerala/
│   ├── maharashtra/
│   ├── north_east/
│   ├── north_india/
│   ├── odisha/
│   ├── tamil_nadu/
│   ├── telangana/
│   └── tribal_traditions/
├── rituals/           → Ceremonial practices
├── sacred_geography/  → Sacred places and spaces
├── sampradayas/       → Spiritual lineages and traditions
├── sciences/          → Sciences (astronomy, mathematics, etc.)
├── stotras/           → Devotional hymns
├── symbols/           → Sacred symbols and their meanings
├── tantras/           → Tantric texts and practices
├── temples/           → Temples and temple traditions
│   ├── divya_desam/
│   ├── jyotirlinga/
│   ├── pancha_bhoota/
│   ├── regional/
│   ├── shakti_peetha/
│   └── temple_architecture/
├── texts/             → Scriptural and literary texts
│   ├── agama/
│   ├── itihasa/
│   ├── purana/
│   ├── regional_texts/
│   ├── sahasranama/
│   ├── smriti/
│   ├── stotra/
│   ├── tantra/
│   ├── upanishad/
│   └── veda/
└── timeline/          → Historical chronology
```

---

## Detailed Category Mapping

### Deity Knowledge (`/deities/`)

**Purpose:** All divine beings, manifestations, and avatars

**Subfolders:**
- **devi/** — Goddess manifestations and Shakti traditions
- **ganesha/** — Ganesha and related traditions
- **hanuman/** — Hanuman and devotional practices
- **kartikeya/** — Kartikeya, Murugan, and regional forms
- **navagraha/** — Nine planetary deities
- **other_deities/** — Lesser-known and regional deities
- **shiva/** — Shiva and Shaiva traditions
- **surya/** — Sun god and solar worship
- **vishnu/** — Vishnu and Vaishnava traditions

**File naming:** `Deity_[DeityName].md`

**Examples:**
- `/deities/shiva/Deity_Shiva.md`
- `/deities/devi/Deity_Durga.md`
- `/deities/ganesha/Deity_Ganesha.md`

**Note:** Deities can have multiple objects:
- Main deity article
- Regional variations (e.g., `Deity_Shiva_Kashmir.md`)
- Specific manifestations (e.g., `Deity_NatarBusiness.md`)

---

### Textual Knowledge (`/texts/`)

**Purpose:** All scriptures, literary works, and written traditions

**Subfolders:**

| Subfolder | Content | Examples |
|-----------|---------|----------|
| **veda/** | Four Vedas and related | Rigveda, Yajurveda, Samaveda, Atharvaveda |
| **upanishad/** | Upanishadic texts | Isha, Kena, Katha, Mundaka |
| **itihasa/** | Epic histories | Mahabharata, Ramayana |
| **purana/** | Puranic texts | Srimad Bhagavatam, Vishnu Purana, Shiva Purana |
| **agama/** | Agama traditions | Shaiva Agamas, Vaishnava Samhitas |
| **smriti/** | Dharma Shastras | Manusmriti, Yajnavalkya Smriti |
| **stotra/** | Hymns and stotras | Aditya Hridayam, Lalita Sahasranama |
| **tantra/** | Tantric texts | Tantra Yoga traditions |
| **sahasranama/** | Thousand-name texts | Vishnu Sahasranama, Lalita Sahasranama |
| **regional_texts/** | Regional literatures | Tamil Sangam, Kannada classics |

**File naming:** `Text_[TextName].md`

**Examples:**
- `/texts/veda/Text_Rigveda.md`
- `/texts/upanishad/Text_ChanUpy.md` (Chandogya Upanishad)
- `/texts/purana/Text_SrimadBhagavatam.md`

---

### Temple Knowledge (`/temples/`)

**Purpose:** Sacred shrines, temple traditions, and pilgrimage sites

**Subfolders:**

| Subfolder | Content | Purpose |
|-----------|---------|---------|
| **jyotirlinga/** | 12 Jyotirlingas | Shiva's most sacred manifestations |
| **divya_desam/** | 108 Divya Desams | Vishnu's most sacred temples |
| **shakti_peetha/** | Shakti Peethas | Goddess temples (51 traditional sites) |
| **pancha_bhoota/** | Five Element temples | Shiva manifestations |
| **temple_architecture/** | Architectural styles | Temple design principles and techniques |
| **regional/** | Other regional temples | Important temples not in above categories |

**File naming:** `Temple_[TempleName]_[LocationIfNeeded].md`

**Examples:**
- `/temples/jyotirlinga/Temple_SomnathJyotirlinga.md`
- `/temples/divya_desam/Temple_TirumalaTemple.md`
- `/temples/shakti_peetha/Temple_KaamaKhyaShaktiPeetha.md`
- `/temples/temple_architecture/TempleArchitecture_ChozhaStyle.md`
- `/temples/regional/Temple_KashiBhairav.md`

---

### Ritual & Practice Knowledge (`/rituals/`)

**Purpose:** Ceremonial practices, worship rituals, and daily observances

**File naming:** `Ritual_[RitualName].md`

**Examples:**
- `/rituals/Ritual_Puja.md`
- `/rituals/Ritual_Yajna.md`
- `/rituals/Ritual_Aarti.md`
- `/rituals/Ritual_Havan.md`
- `/rituals/Ritual_AbhishekCeremony.md`

**Related but separate categories:**
- Mantras (`/mantras/`) — Sacred sound formulas
- Stotras (`/stotras/`) — Devotional hymns
- Tantras (`/tantras/`) — Tantric practices

---

### Philosophy Knowledge (`/philosophy/`)

**Purpose:** Schools of thought, Darshanas, and philosophical concepts

**File naming:** `Philosophy_[SchoolName].md` or `Concept_[ConceptName].md`

**Examples:**
- `/philosophy/Philosophy_Advaita.md`
- `/philosophy/Philosophy_Dvaita.md`
- `/philosophy/Philosophy_KashmirShaivism.md`
- `/philosophy/Concept_Brahman.md`
- `/philosophy/Concept_Dharma.md`
- `/philosophy/Concept_Karma.md`

**May also include:**
- Historical evolution of schools
- Key philosophers in schools
- Textual bases for schools
- Comparative philosophy

---

### Sacred Geography (`/sacred_geography/`)

**Purpose:** Sacred places, pilgrimage routes, and spiritual geography

**File naming:** `Geography_[PlaceName].md` or `Pilgrimage_[RouteName].md`

**Examples:**
- `/sacred_geography/Geography_Kashi.md`
- `/sacred_geography/Geography_Kailash.md`
- `/sacred_geography/Geography_Mathura.md`
- `/sacred_geography/Pilgrimage_ChharDham.md`
- `/sacred_geography/Pilgrimage_SaptaPuri.md`

**Related but separate:**
- Temple locations (`/temples/`)
- Regional traditions (`/regional/`)

---

### Regional Knowledge (`/regional/`)

**Purpose:** Region-specific traditions, practices, and knowledge

**Geographic subfolders:**
- **andhra_pradesh/** — Andhra Pradesh traditions
- **assam/** — Assam and Northeast traditions
- **bengal/** — Bengali traditions
- **gujarat/** — Gujarati traditions
- **himalaya/** — Himalayan traditions
- **karnataka/** — Kannada traditions
- **kashmir/** — Kashmir Shaiva traditions
- **kerala/** — Kerala/Tamil traditions
- **maharashtra/** — Maharashtrian traditions
- **north_east/** — Northeastern traditions (general)
- **north_india/** — North Indian traditions
- **odisha/** — Odishan traditions
- **tamil_nadu/** — Tamil traditions
- **telangana/** — Telangana traditions
- **tribal_traditions/** — Tribal and indigenous traditions

**File naming:** `[Region]_[TopicName].md` or `Tradition_[TraditionName].md`

**Examples:**
- `/regional/tamil_nadu/TamilTradition_SrirangamTemple.md`
- `/regional/kashmir/KashmirShaivism_LingarajTemple.md`
- `/regional/bengal/BengaliTradition_KaliWorship.md`
- `/regional/tribal_traditions/TribalTradition_TheyamDance.md`

---

### Knowledge Systems (`/indian_knowledge_systems/`)

**Purpose:** Traditional Indian sciences and scholarly systems

**Includes:**

| System | Examples |
|--------|----------|
| **Jyotisha** | Vedic astrology, planetary science |
| **Ayurveda** | Traditional medicine, doshas |
| **Vastu** | Sacred architecture principles |
| **Natya** | Dance and performance theory |
| **Sangeet** | Music and musical theory |
| **Vyakaran** | Sanskrit grammar |
| **Nyaya** | Logic and epistemology |
| **Mathematics** | Ancient mathematical systems |
| **Astronomy** | Scientific astronomy |

**File naming:** `System_[SystemName].md` or `[Topic].md`

**Examples:**
- `/indian_knowledge_systems/Ayurveda_Doshas.md`
- `/indian_knowledge_systems/Jyotisha_Vedic.md`
- `/indian_knowledge_systems/Vastu_Principles.md`
- `/indian_knowledge_systems/Natya_Bharata.md`

**Note:** Some systems have dedicated folders:
- `/ayurveda/` — Separate dedicated folder
- `/astronomy/` — Separate dedicated folder

---

### Supporting Knowledge Categories

#### Mantras (`/mantras/`)
**Purpose:** Sacred sound formulas and their uses

**File naming:** `Mantra_[MantraName].md`

**Examples:**
- `/mantras/Mantra_Gayatri.md`
- `/mantras/Mantra_Maha_Mrityunjaya.md`

#### Stotras (`/stotras/`)
**Purpose:** Devotional hymns and praise poems

**File naming:** `Stotra_[StotraName].md`

**Examples:**
- `/stotras/Stotra_Aditya_Hridayam.md`
- `/stotras/Stotra_Lalita_Sahasranama.md`

#### Symbols (`/symbols/`)
**Purpose:** Sacred symbols and their meanings

**File naming:** `Symbol_[SymbolName].md`

**Examples:**
- `/symbols/Symbol_Aum.md`
- `/symbols/Symbol_Chakra.md`
- `/symbols/Symbol_Swastika.md`

#### Iconography (`/iconography/`)
**Purpose:** Visual representation conventions and symbolic meanings

**File naming:** `Iconography_[Topic].md`

**Examples:**
- `/iconography/Iconography_DeityColors.md`
- `/iconography/Iconography_VehiclesOfDeities.md`
- `/iconography/Iconography_TempleSymbols.md`

#### Manuscripts (`/manuscripts/`)
**Purpose:** Rare, ancient, and damaged texts

**File naming:** `Manuscript_[ManuscriptName].md`

**Examples:**
- `/manuscripts/Manuscript_PalmLeafBhagavata.md`
- `/manuscripts/Manuscript_TempleArchives.md`

#### Sampradayas (`/sampradayas/`)
**Purpose:** Spiritual lineages and organized traditions

**File naming:** `Sampradaya_[TraditionalName].md` or `Lineage_[LineageName].md`

**Examples:**
- `/sampradayas/Sampradaya_Shankara.md`
- `/sampradayas/Sampradaya_Ramanuja.md`
- `/sampradayas/Lineage_Gaudiya_Vaishnavism.md`

#### Acharyas (`/acharyas/`)
**Purpose:** Great teachers, philosophers, and lineage founders

**File naming:** `Acharya_[AcharyaName].md`

**Examples:**
- `/acharyas/Acharya_AdiShankaracharya.md`
- `/acharyas/Acharya_Ramanuja.md`
- `/acharyas/Acharya_Madhva.md`

#### Mathas (`/mathas/`)
**Purpose:** Monastic institutions and ashrams

**File naming:** `Matha_[MathaName].md`

**Examples:**
- `/mathas/Matha_SringeriShankara.md`
- `/mathas/Matha_DwarkaShankara.md`

#### Tantras (`/tantras/`)
**Purpose:** Tantric texts and practices

**File naming:** `Tantra_[TantraName].md`

**Examples:**
- `/tantras/Tantra_KulamargaTantra.md`
- `/tantras/Tantra_SriVidya.md`

#### Timeline (`/timeline/`)
**Purpose:** Chronological history and dated events

**File naming:** `Timeline_[Period].md` or `Chronology_[Topic].md`

**Examples:**
- `/timeline/Timeline_Vedic_Period.md`
- `/timeline/Chronology_TempleBuilding.md`

---

## Organization Principles

### 1. Primary Categorization

Each object belongs primarily to ONE folder based on:
- What is the main topic?
- What would a user search for first?
- Where would someone naturally look?

**Example:**
- Ganesha primary object → `/deities/ganesha/Deity_Ganesha.md`
- Ganesha worship in Bengal → `/regional/bengal/Tradition_GaneshaBengal.md` OR `/deities/ganesha/Ganesha_Bengal.md`
- Ganesha in Rigveda → `/texts/veda/Text_Rigveda.md` (within Rigveda article)

### 2. Cross-Category Connection

Objects can reference content in other folders through:
- **Explicit cross-references:** "See also: [Deity_Ganesha.md](../../deities/ganesha/Deity_Ganesha.md)"
- **Knowledge graph relationships:** Stored in metadata
- **Related knowledge sections:** Listed at end of objects

### 3. Specialized Subfolders

Some categories have meaningful subdivisions:
- `/deities/` has deity-specific subfolders
- `/temples/` has tradition-specific subfolders
- `/texts/` has text-type subfolders
- `/regional/` has geographic subfolders

### 4. General Categories

Some categories stand alone:
- `/mantras/` — Individual mantra files
- `/symbols/` — Individual symbol files
- `/festivals/` — Individual festival files
- `/philosophy/` — Individual school files

---

## File Naming Conventions

### Standard Naming Pattern

```
[Category]_[Topic_Name].md
```

**Rules:**
- Use PascalCase for multi-word topics
- Replace spaces with underscores
- Start with category prefix when helpful (e.g., Deity_, Text_, Temple_)
- Keep names concise but descriptive
- Use English (not Sanskrit) for filenames, though Sanskrit can be in content

**Examples:**

✅ Good:
- `Deity_Ganesha.md`
- `Temple_KashiVishwanath.md`
- `Text_Bhagavad_Gita.md`
- `Philosophy_Advaita.md`
- `Ritual_Puja.md`

❌ Avoid:
- `ganesha.md` (no category prefix)
- `Deity Ganesha.md` (spaces not underscores)
- `Bhagavadgita.md` (not separated)
- `deity_of_new_beginnings.md` (too descriptive)

### Regional Subfolder Convention

```
/regional/[region]/[Topic_Name].md
```

**Examples:**
- `/regional/tamil_nadu/Tradition_SrirangamTemple.md`
- `/regional/kashmir/Tradition_KashmirShaivism.md`

### Temple Subfolder Convention

```
/temples/[tradition]/Temple_[Name]_[Location].md
```

**Examples:**
- `/temples/jyotirlinga/Temple_Somanath_Gujarat.md`
- `/temples/divya_desam/Temple_Tirumala_AndhraPradesh.md`

---

## Current Status & Maintenance

### Folder Structure Completeness
- ✅ Main category folders created
- ✅ Deity subfolders organized
- ✅ Temple subfolders organized
- ✅ Regional subfolders organized
- ✅ Text subfolders organized
- 🔄 Content population ongoing

### Future Refinements
- Automated folder structure validation
- Cross-folder relationship mapping
- Automated suggestions for related content
- Taxonomy refinement based on growth patterns

---

## Using This Guide

**For Researchers:**
1. Identify your topic's primary category
2. Find the appropriate subfolder
3. Use the naming convention for your file
4. Add cross-references to related content

**For Content Teams:**
1. Understand the organizational logic
2. Use folder structure for content discovery
3. Create content calendars by category
4. Identify content gaps by examining folder completeness

**For System Developers:**
1. Use structure for navigation and search
2. Implement folder-based category tags
3. Create automated suggestions based on structure
4. Build path-based permission systems if needed

---

## Questions & Refinements

If you encounter a topic that doesn't clearly fit:

1. **Decide on primary category** — Where would most users look?
2. **Create cross-references** — Link from related categories
3. **Add to knowledge graph** — Map relationships explicitly
4. **Consider subfolder** — If many related objects, create subfolder
5. **Document the decision** — Note why you chose this location

For systematic improvements to this structure, propose changes to the Senior Editor.

---

## Appendix: Quick Reference

| Category | Folder | Examples | Sub-folders |
|----------|--------|----------|------------|
| Deities | `/deities/` | Shiva, Vishnu, Devi | By deity |
| Texts | `/texts/` | Vedas, Puranas | By text type |
| Temples | `/temples/` | Varanasi, Tirupati | By temple type |
| Rituals | `/rituals/` | Puja, Yajna | None |
| Philosophy | `/philosophy/` | Advaita, Dvaita | None |
| Mantras | `/mantras/` | Gayatri, Maha Mrityunjaya | None |
| Regions | `/regional/` | Tamil Nadu, Kashmir | By state/region |
| Pilgrimage | `/pilgrimage/` | Chardham, Sapta Puri | None |
| Geography | `/sacred_geography/` | Kashi, Kailash | None |
| Symbols | `/symbols/` | Aum, Chakra | None |
| Knowledge Systems | `/indian_knowledge_systems/` | Ayurveda, Jyotisha | None |
| Architecture | `/architecture/` | Temple design | None |
| Astronomy | `/astronomy/` | Vedic astrology | None |
| Manuscripts | `/manuscripts/` | Rare texts | None |
| Lineages | `/sampradayas/` | Shankara Lineage | None |
| Teachers | `/acharyas/` | Shankaracharya | None |
| Monasteries | `/mathas/` | Sringeri Matha | None |
| Hymns | `/stotras/` | Aditya Hridayam | None |
| Tantras | `/tantras/` | Sri Vidya | None |
| History | `/timeline/` | Vedic Period | None |

---

This mapping ensures consistency, discoverability, and logical organization of the entire SDKA knowledge repository.
