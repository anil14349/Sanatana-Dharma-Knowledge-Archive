# Knowledge Graph Architecture

**Document Version:** 1.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Document Type:** Technical Specification  
**Status:** Stable  
**Last Updated:** June 2026

---

## Table of Contents

1. Overview & Purpose
2. Graph Concept & Structure
3. Node Types
4. Relationship Types
5. Graph Properties & Queries
6. Implementation Considerations
7. Discovery & Recommendation
8. Visual Representation

---

## 1. Overview & Purpose

### 1.1 The Knowledge Graph

The **Knowledge Graph** is the network of relationships and interconnections between all knowledge objects in SDKA. It transforms the archive from a collection of isolated topics into an interconnected web of understanding.

### 1.2 Core Purpose

The Knowledge Graph serves several critical functions:

**Discovery**
- Users can explore related knowledge
- New connections become visible
- Research needs become apparent

**Relationship Mapping**
- Understand how concepts interconnect
- Trace philosophical lineages
- Track historical influences
- Connect deities to texts to temples

**Gap Identification**
- Identify missing knowledge
- Find disconnected clusters
- Spot redundancy
- Prioritize research

**Recommendation**
- Suggest related content
- Enable personalized learning paths
- Support "learn more" flows

**Semantic Understanding**
- Encode meaning through relationships
- Support AI/ML applications
- Enable advanced queries
- Facilitate knowledge discovery

---

## 2. Graph Concept & Structure

### 2.1 Basic Components

**Nodes** = Knowledge Objects  
**Edges** = Relationships between them  
**Attributes** = Properties of nodes and edges

```
┌─────────────────────────────────────────────────────┐
│                  KNOWLEDGE GRAPH                     │
│                                                      │
│     Node: Shiva          Node: Puja                 │
│     (Deity)        ──worshipped in──→   (Ritual)   │
│     │                                      │        │
│     │ appears in                    │ connected to   │
│     ↓                                ↓              │
│  Node: Vedas                  Node: Hindu Practice │
│  (Text)                                             │
│                                                      │
│     Nodes are connected through meaningful          │
│     relationships representing how knowledge        │
│     relates to other knowledge.                     │
└─────────────────────────────────────────────────────┘
```

### 2.2 Graph Properties

The SDKA Knowledge Graph is:

- **Directed** — Relationships have direction (Source → Target)
- **Multi-relational** — Multiple types of relationships exist
- **Weighted** — Some relationships are stronger than others
- **Attributed** — Edges carry metadata about relationships
- **Hierarchical** — Contains both hierarchical and lateral connections
- **Dynamic** — Grows as new knowledge objects are added
- **Queryable** — Can be searched for specific paths and patterns

---

## 3. Node Types

### 3.1 Primary Node Types

Every knowledge object becomes a node. Standard node types:

| Node Type | Examples | Attributes |
|-----------|----------|-----------|
| **Deity** | Shiva, Vishnu, Devi, Ganesha | Form, region, manifestations |
| **Text** | Vedas, Puranas, Agamas | Language, century, school |
| **Temple** | Kashi Vishwanath, Meenakshi | Location, deity, history |
| **Ritual** | Puja, Yajna, Aarti | Purpose, tradition, complexity |
| **Philosophy** | Advaita, Dvaita, Samkhya | School, founder, texts |
| **Concept** | Dharma, Karma, Brahman | Definition, applications, traditions |
| **Tradition** | Bengali, Tamil, Kashmir | Region, practices, deities |
| **Geography** | Kashi, Kailash, Mathura | Region, significance, associations |
| **Practice** | Meditation, Mantra, Yoga | Type, context, benefits |
| **Festival** | Diwali, Navaratri, Shivaratri | Season, deities, regions |
| **Symbol** | Aum, Chakra, Swastika | Meaning, usage, traditions |
| **Manuscript** | Palm leaf texts, Temple records | Age, language, location |
| **Lineage** | Shankara Sampradaya, Gaudiya | Founder, practices, regions |

### 3.2 Node Attributes

Essential attributes for every node:

```
Node Attributes:
├─ id: unique identifier
├─ type: node category
├─ title: official name
├─ summary: brief description
├─ status: verified|draft|disputed
├─ created_date: when created
├─ updated_date: when last modified
├─ complexity_level: beginner|intermediate|advanced
├─ geographic_scope: regions involved
├─ temporal_scope: time periods covered
└─ source_material: authoritative sources
```

---

## 4. Relationship Types

### 4.1 Primary Relationship Categories

#### 1. Hierarchical Relationships

**Purpose:** Show parent-child and part-of relationships

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `PART_OF` | Child → Parent | Vishnu → Hindu Deities |
| `SUBDIVIDES` | Parent → Child | Vedas → Rigveda |
| `SPECIALIZES` | Specific → General | Tamil Shiva → Shiva |
| `GENERALIZES` | General → Specific | Shiva → Shaiva Sects |

**Usage:**
```
Meenakshi Temple ──PART_OF──→ Divya Desams
Vishnu Sahasranama ──PART_OF──→ Mahabharata
Kashmir Shaivism ──SPECIALIZES──→ Shaivism
```

#### 2. Scriptural Relationships

**Purpose:** Show textual appearances and references

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `APPEARS_IN` | Topic → Text | Ganesha → Rigveda |
| `DEFINES` | Text → Concept | Upanishads → Brahman |
| `DESCRIBES` | Text → Subject | Bhagavad Gita → Dharma |
| `REFERENCES` | Text → Text | Puranas → Vedas |
| `ELABORATES` | Text → Text | Brahmasutra → Vedas |

**Usage:**
```
Shiva ──APPEARS_IN──→ Rigveda
Bhagavad Gita ──DESCRIBES──→ Karma Yoga
Brahmasutra ──ELABORATES──→ Upanishads
```

#### 3. Devotional Relationships

**Purpose:** Show worship and practice connections

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `WORSHIPPED_IN` | Deity ↔ Place | Ganesha ↔ Kashi Vishwanath |
| `PRACTICES` | Practice → Deity | Puja → Shiva |
| `ASSOCIATED_WITH` | Concept ↔ Ritual | Purification ↔ Puja |
| `RITUAL_OF` | Ritual → Tradition | Aarti → Shaivism |

**Usage:**
```
Ganesha ──WORSHIPPED_IN──→ Kashi Bisheshwar Temple
Puja ──PRACTICES──→ Vishnu
Mantra ──RITUAL_OF──→ Vedic Tradition
```

#### 4. Geographic Relationships

**Purpose:** Show regional and location-based connections

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `LOCATED_IN` | Temple → Region | Kashi Vishwanath → Varanasi |
| `SACRED_TO` | Region → Deity | Kailash → Shiva |
| `PILGRIMAGE_ROUTE` | Location → Location | Kashi ↔ Gaya |
| `REGIONAL_VARIATION` | Topic → Region | Diwali → Tamil Nadu |

**Usage:**
```
Meenakshi Temple ──LOCATED_IN──→ Madurai
Mount Kailash ──SACRED_TO──→ Shiva
Kashi → [pilgrimage routes] → Mathura
```

#### 5. Philosophical Relationships

**Purpose:** Show philosophical school and concept connections

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `SCHOOL_OF` | School ← Founder | Advaita → Shankaracharya |
| `INFLUENCED_BY` | School → School | Advaita → Vedanta |
| `INTERPRETS` | School → Text | Advaita → Upanishads |
| `CRITICIZES` | School → School | Dvaita → Advaita |
| `RELATED_TO` | Concept ↔ Concept | Karma ↔ Dharma |

**Usage:**
```
Advaita Vedanta ──FOUNDED_BY──→ Adi Shankaracharya
Dvaita ──CRITICIZES──→ Advaita
Karma ──RELATED_TO──→ Rebirth
```

#### 6. Temporal Relationships

**Purpose:** Show historical development and evolution

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `PRECEDES` | Earlier → Later | Vedas → Upanishads |
| `EVOLVED_FROM` | Modern → Ancient | Contemporary Puja → Vedic Yagna |
| `INFLUENCED` | Source → Influenced | Vedas → Puranic Thought |

**Usage:**
```
Vedas ──PRECEDES──→ Upanishads
Shankara ──INFLUENCED──→ Later Vedantic Thought
Vedic Ritual ──EVOLVED_INTO──→ Temple Ritual
```

#### 7. Comparative Relationships

**Purpose:** Show contrasts, similarities, and alternatives

| Relationship | Direction | Example |
|-------------|-----------|---------|
| `CONTRASTS_WITH` | Topic ↔ Topic | Advaita ↔ Dvaita |
| `SIMILAR_TO` | Topic ↔ Topic | Dvaita ↔ Qualified Monism |
| `ALTERNATIVE_TO` | Option ↔ Option | Silent Meditation ↔ Mantra |

**Usage:**
```
Advaita ──CONTRASTS_WITH──→ Dvaita
Bhakti Yoga ──SIMILAR_TO──→ Devotional Theism
```

### 4.2 Relationship Attributes

Every edge carries metadata:

```
Relationship Attributes:
├─ source: source node ID
├─ target: target node ID
├─ type: relationship category
├─ strength: weak|moderate|strong
├─ bidirectional: true|false
├─ evidence: source supporting relationship
├─ confidence: high|medium|low
├─ context: brief explanation
└─ created_date: when relationship added
```

**Example:**
```
Source: Shiva (Deity)
Target: Kashi Vishwanath (Temple)
Type: WORSHIPPED_IN
Strength: Strong
Bidirectional: Yes
Evidence: Agama texts, temple records
Confidence: High
Context: Shiva's primary temple, mentioned in Kashi Khanda
```

---

## 5. Graph Properties & Queries

### 5.1 Key Properties

The Knowledge Graph enables:

**Direct Connections**
```
What texts mention Ganesha?
Ganesha ←[APPEARS_IN]← [Texts]

Which deities are worshipped at Varanasi?
[Deities] ─[WORSHIPPED_IN]→ Varanasi temples
```

**Path Queries**
```
How does Shiva connect to Yoga?
Shiva → Shaivism → Philosophy → Yoga

What connects Bhakti to Ganesha?
Bhakti → Worship Practices → Puja → Ganesha
```

**Relationship Density**
```
Which topics are most interconnected? (High degree nodes)
Which topics are isolated? (Low degree nodes)
Which topic pairs bridge otherwise separate clusters?
```

**Hierarchies**
```
All forms of Shiva worship
All Puranic texts
All North Indian temples
```

### 5.2 Example Queries

**Query 1: Related Topics**
```
START: Ganesha (Deity)
FIND: All directly connected nodes
RETURN: Related topics with relationship types

Result:
├─ Appears in: Rigveda, Vedas
├─ Worshipped in: Kashi Bisheshwar, Varanasi temples
├─ Associated with: Obstacle removal, Beginnings
├─ Festival: Ganesh Chaturthi
├─ Philosophy: Discussed in various schools
└─ Iconography: Elephant, Modaka, Goad
```

**Query 2: Philosophical Chain**
```
START: Brahman (Concept)
FIND: All interpretation paths
THROUGH: Advaita, Dvaita, Qualified Monism

Result:
├─ Advaita interpretation: Non-dual, sole reality
├─ Dvaita interpretation: Different from Brahman
└─ QualifiedMonism: Both different and non-different
```

**Query 3: Geographic Spread**
```
START: Shakti worship (Practice)
FIND: All regions where practiced
RETURN: Regions + specific manifestations

Result:
├─ North India: Kali worship
├─ South India: Kamakshi, Meenakshi
├─ Northeast India: Durga in various forms
└─ Kashmir: Specific Shakti interpretation
```

---

## 6. Implementation Considerations

### 6.1 Storage Options

**Option 1: Graph Database** (Recommended for scale)
- Neo4j, ArangoDB, JanusGraph
- Native relationship storage
- Efficient traversal queries
- Complex pattern matching
- Scalable to millions of nodes

**Option 2: Document Database** (Current approach)
- MongoDB, CosmosDB
- Flexible schema
- Embedded relationships
- Sufficient for current scale
- Migration path to graph DB available

**Option 3: RDF/Semantic Web** (Future possibility)
- Triple stores (Virtuoso, AllegroGraph)
- Semantic reasoning
- SPARQL queries
- Linked data compatibility
- Long-term interoperability

### 6.2 Current Implementation

**Current state (v4.0):**
- Markdown files with cross-references
- Manually-created relationship metadata
- Basic interconnection tracking
- File-based storage

**Evolution path:**
- v4.1: Automated relationship extraction
- v4.2: Graph database migration
- v5.0: Advanced graph querying and recommendations

### 6.3 Maintenance & Updating

**Regular tasks:**
- Add new relationships as content is researched
- Update confidence levels based on new evidence
- Remove incorrect relationships
- Strengthen weak relationships with evidence
- Monitor for orphaned or isolated nodes

**Quality assurance:**
- Verify bidirectional relationships
- Check consistency across connections
- Update when source material changes
- Document controversial relationships

---

## 7. Discovery & Recommendation

### 7.1 Discovery Patterns

The Knowledge Graph enables several discovery patterns:

**Serendipitous Discovery**
```
User reads about Ganesha
→ Sees "appears in Vedas" 
→ Explores Vedic knowledge
→ Discovers Vedic cosmology
```

**Thematic Exploration**
```
User interested in Meditation
→ Sees connected practices (Yoga, Mantra)
→ Explores different meditation traditions
→ Finds philosophical underpinnings
```

**Regional Deep Dive**
```
User learns about Tamil Nadu
→ Sees associated temples, deities, festivals
→ Explores regional practices and texts
→ Understands cultural specificity
```

### 7.2 Recommendation Engine (Future)

**Recommendation types:**
- "Users interested in X also studied Y"
- "People who know A find B helpful"
- "Complete your learning path: read Z next"

**Path recommendations:**
```
Beginner: 
Ganesha (beginner deity) 
→ Basic Puja practice
→ Introduction to Hinduism

Intermediate:
Shiva (intermediate deity)
→ Shaiva philosophy
→ Temple traditions
→ Tantric practices (if interested)

Advanced:
Compare Shiva in Vedas vs Puranas
→ Shaivism vs other schools
→ Historical evolution
→ Textual criticism
```

---

## 8. Visual Representation

### 8.1 Graph Visualization

The Knowledge Graph can be visualized in multiple ways:

**Force-Directed Graph**
```
Nodes repel each other, edges act as springs
Result: Clusters of related topics form naturally
Benefit: Visual identification of topic domains
```

**Hierarchical Layout**
```
Organized by type or category
Result: Structural relationships visible
Benefit: Clear organization, easy to navigate
```

**Radial Layout**
```
Central topic radiates outward in layers
Result: Topic and its relationships visible
Benefit: Focus on single topic's neighborhood
```

### 8.2 Visualization Elements

**Node Representation:**
- Size = connectivity (more connections = larger)
- Color = category (deity = red, text = blue, etc.)
- Shape = status (verified, draft, disputed)
- Labels = topic name

**Edge Representation:**
- Line weight = relationship strength
- Color = relationship type
- Arrows = direction (for non-bidirectional)
- Labels = relationship type

**Example:**
```
Big red circle labeled "Shiva" = 
  - Deity (category, red)
  - Highly connected (large)
  
Thick blue line to "Rigveda" = 
  - Strong relationship (thick)
  - Textual relationship (blue)
  - APPEARS_IN relationship
```

---

## Conclusion

The Knowledge Graph transforms SDKA from a repository of isolated knowledge objects into an interconnected web of understanding. By explicitly mapping relationships between topics, the archive enables discovery, supports learning, identifies gaps, and facilitates recommendations—all while making the structure of Sanātana Dharma knowledge visible and explorable.

The graph architecture provides a foundation for both current navigation needs and future AI/ML applications while maintaining the core principle of research-driven, source-aware knowledge preservation.
