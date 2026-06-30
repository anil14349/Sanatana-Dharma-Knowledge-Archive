# 10 – AI Architecture

**Document Version:** 4.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Status:** Operational Reference  
**Last Updated:** June 2026

---

# Purpose

This document defines how SDKA uses artificial intelligence: what AI may do, what it must never do, and how human review remains the final authority.

**Core principle:** AI is an assistant. It is not the authority.

---

# AI Philosophy

SDKA should use AI to:

- Organize information
- Summarize sources
- Compare traditions
- Suggest graph connections
- Draft content for human review
- Visualize relationships
- Explain concepts in accessible language

SDKA must never use AI to:

- Finalize factual claims without human verification
- Assign confidence scores without human review
- Publish content without editorial and research approval
- Generate restricted or initiation-dependent content
- Replace traditional scholarship with synthetic assertions
- Present AI-generated speculation as scriptural fact

---

# AI Role by Engine

| Engine | AI Role | Human Role |
|--------|---------|------------|
| Research | Source discovery, summarization, comparison drafts | Verify all claims; assign evidence tags |
| Knowledge | Metadata suggestions, relationship proposals | Approve KO content and graph edges |
| Editorial | Series suggestions, caption drafts, scheduling ideas | Final editorial decisions |
| Visual | Composition ideas, alt text drafts, layout suggestions | Art direction and sacred subject approval |
| Publishing | Format adaptation, hashtag suggestions | Final review and publication |
| Analytics | Pattern detection, gap analysis, trend summaries | Interpret and act on insights |

---

# Permitted AI Workflows

## 1. Source Summarization

**Input:** Scripture passage, academic paper, temple record  
**AI task:** Summarize key points, extract quotable references  
**Human task:** Verify summary against original; check for distortion

## 2. Graph Connection Suggestions

**Input:** Existing KO with metadata  
**AI task:** Propose related nodes and edge types  
**Human task:** Validate each suggested relationship

## 3. Research Card Drafting

**Input:** Backlog entry with research questions  
**AI task:** Draft bibliography, preliminary findings structure  
**Human task:** Verify sources exist; reject hallucinated references

## 4. Content Drafting

**Input:** Published KO + editorial plan + visual brief  
**AI task:** Draft carousel script, article, or YouTube narration  
**Human task:** Three-pass review (research, editorial, visual)

## 5. Myth Verification Assistance

**Input:** Popular claim or internet myth  
**AI task:** Search for earliest sources, compile evidence map  
**Human task:** Verify sources; assign final evidence classification

## 6. Gap Analysis

**Input:** Knowledge graph index  
**AI task:** Identify thin clusters, orphan nodes, missing bridges  
**Human task:** Prioritize gaps for backlog

---

# Prohibited AI Workflows

| Workflow | Reason |
|----------|--------|
| Auto-publish content | No human review |
| Generate Sanskrit mantras or restricted rituals | Ethics violation |
| Invent scripture references | Hallucination risk |
| Declare one tradition "correct" | Violates multiple viewpoints framework |
| Scrape and republish copyrighted translations | Legal and ethical risk |
| Create deity imagery without traditional reference | Iconographic inaccuracy |

---

# Hallucination Prevention

AI models invent plausible-sounding sources. SDKA requires:

1. **Every AI-cited source must be verified** by a human against the original text.
2. **No claim enters a KO** from AI output alone—it must trace to a verified source.
3. **Sanskrit quotations** must be checked against printed or digital editions.
4. **Temple names, locations, and dates** must be verified independently.
5. When AI cannot find a source, it must say so—not fabricate one.

---

# Prompt Guidelines

When using AI tools for SDKA work, include these constraints in prompts:

```
You are assisting the Sanatana Dharma Knowledge Archive (SDKA).
Rules:
- Cite only real, verifiable sources. If uncertain, say "source not confirmed."
- Present multiple viewpoints when traditions disagree.
- Never present folklore as scripture.
- Never generate restricted mantras, nyasa, or initiation-dependent content.
- Label speculation clearly.
- Use evidence tags: Scriptural, Agamic, Traditional, Historical, Regional, Folklore, Academic, Speculative.
- Respect all sampradayas without ranking them.
```

---

# AI Tool Categories

| Category | Example Use | SDKA Policy |
|----------|-------------|-------------|
| LLM (ChatGPT, Claude) | Summarization, drafting, comparison | Human review required |
| Image AI (Midjourney, DALL-E) | Concept exploration only | Not for final deity depictions without traditional reference |
| Translation AI | Draft translations for review | Must compare with published translations |
| Search AI (Perplexity) | Source discovery | All sources independently verified |
| Graph AI | Relationship suggestions | Human validates all edges |

**Deity imagery:** Prefer traditional sculpture, painting, and manuscript references. AI-generated deity images may be used for internal mood exploration only—not for publication without art direction review.

---

# Data Privacy

- Do not feed initiation-dependent or restricted content into public AI tools.
- Research notes containing sensitive temple information: use local or private models when available.
- Personal communications with traditional practitioners: never upload to AI without consent.

---

# Future AI Capabilities (Phase 6)

Planned for 2028+ when the knowledge base has 200+ objects:

| Capability | Requirement |
|------------|-------------|
| Public knowledge assistant | 200+ verified KOs; confidence scoring mature |
| Interactive graph explorer | `edges.yaml` populated; visualization tooling |
| AI research assistant (internal) | Proven hallucination prevention workflow |
| Auto-suggest backlog from graph gaps | Stable graph with 10+ clusters |

None of these replace human review.

---

# AI Decision Log

| Decision | Reason | Date |
|----------|--------|------|
| AI assists, never authorizes | Preserve authenticity and trust | 2026 |
| No AI deity imagery for publication | Iconographic accuracy risk | 2026 |
| All AI sources must be human-verified | Hallucination prevention | 2026 |
| Restricted content excluded from AI inputs | Ethics | 2026 |

---

# Related Documents

| Document | Purpose |
|----------|---------|
| `04_Research_Methodology.md` | Research standards AI must follow |
| `03_Knowledge_Object_Specification.md` | KO schema for AI output |
| `07_Knowledge_Graph.md` | Graph for AI suggestions |
| `09_Project_Roadmap.md` | Phase 6 AI timeline |
