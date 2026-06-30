# 08 – Content Production

**Document Version:** 4.0  
**Project:** Sanatana Dharma Knowledge Archive (SDKA)  
**Status:** Operational Reference  
**Last Updated:** June 2026

---

# Purpose

This document defines the end-to-end production workflow: how a verified knowledge object becomes published content across formats and platforms.

---

# Production Philosophy

- **One source, many formats** — Every publication exports from the same KO.
- **No shortcuts** — Production cannot begin without a `published` KO and editorial plan.
- **Quality over volume** — One excellent carousel beats five rushed posts.
- **Preserve assets** — Source files are kept for cross-platform reuse.

---

# Production Pipeline

```
Knowledge Object (published)
        ↓
Editorial Plan (series, level, queue)
        ↓
Visual Brief (archetypes, art direction)
        ↓
Format Draft (carousel / article / script)
        ↓
Review (research + editorial + visual)
        ↓
Final Assets (designed slides, exports)
        ↓
Publication (platform upload)
        ↓
Archive (store published version + metrics)
```

---

# Format Types

| Format | Template | Primary Platform | Secondary Use |
|--------|----------|------------------|---------------|
| Carousel | `templates/carousel_template.md` | Instagram | Website gallery, PDF |
| Article | `templates/article_template.md` | Website, blog | Newsletter, book chapters |
| YouTube Script | `templates/youtube_script_template.md` | YouTube | Podcast narration |
| Research Card | `templates/research_card_template.md` | Internal | KO creation input |

Future formats: podcast outline, course module, encyclopedia entry—all derived from the same KO.

---

# Stage 1: Pre-Production Checklist

Before any production work begins:

- [ ] KO status is `published`
- [ ] Editorial plan exists (series, level, queue position)
- [ ] Visual brief created (`06_Visual_System.md`)
- [ ] Archetype sequence defined
- [ ] No restricted content in public-facing plan
- [ ] Graph connections identified for "Connection" slide

---

# Stage 2: Draft Production

### Carousel

1. Open `templates/carousel_template.md`
2. Fill slide-by-slide from visual brief
3. Pull claims from KO **Core Claims** section only
4. Tag evidence in slide notes (not always on slide face)
5. Write caption draft

### Article

1. Open `templates/article_template.md`
2. Expand KO sections into long-form prose
3. Add inline source references
4. Include "Further Reading" from KO bibliography

### YouTube Script

1. Open `templates/youtube_script_template.md`
2. Write spoken narrative from KO
3. Mark visual/B-roll cues
4. Time estimate per section

---

# Stage 3: Review

Three-pass review before finalization:

| Pass | Reviewer Focus | Checks |
|------|----------------|--------|
| Research | Accuracy | Claims match KO; evidence tags correct; no new unverified claims |
| Editorial | Education | Series fit; level appropriate; leads to next topic; voice consistent |
| Visual | Design | Archetypes followed; iconography correct; mobile readability; style guide |

All three passes must pass. Any failure returns to draft.

---

# Stage 4: Asset Creation

- Design slides in primary design tool (Figma, Canva, Adobe)
- Export at platform resolution (Instagram: 1080×1350 px portrait)
- Save source files to `assets/`
- Save published exports to `assets/published/{platform}/{date}-{slug}/`

---

# Stage 5: Publication

### Instagram Checklist

- [ ] Carousel images in correct order
- [ ] Caption: hook → context → CTA to learn more
- [ ] Hashtags: 5–10 relevant, not spammy
- [ ] Alt text on each image (accessibility)
- [ ] Location tag if temple/region specific
- [ ] Schedule or publish at optimal time

### Post-Publication

- [ ] Log in publication tracker (date, URL, format, KO ID)
- [ ] Update KO `content_status` to `published`
- [ ] Note initial metrics after 48 hours
- [ ] Capture audience questions for backlog

---

# Publication Tracker

Maintain in `knowledge/publication_log.md`:

```markdown
| Date | KO ID | Title | Format | Platform | URL | Saves | Shares | Notes |
|------|-------|-------|--------|----------|-----|-------|--------|-------|
| 2026-06-30 | TOP-0001 | Panchamukha Hanuman | Carousel | Instagram | ... | ... | ... | ... |
```

---

# Repurposing Workflow

One KO can produce multiple formats over time:

```
KO published
  → Week 1: Instagram carousel
  → Week 3: Long-form article
  → Month 2: YouTube video
  → Month 3: Website encyclopedia entry
```

Each format gets its own production cycle but shares the same research foundation. Do not re-research for each format.

---

# Quality Framework

### Content Quality

- Accurate, evidence-tagged claims
- Respectful tone
- Clear audience level
- Educational value

### Visual Quality

- Meets visual checklist (`06_Visual_System.md`)
- Style guide compliant
- Mobile-readable

### Production Quality

- No typos or transliteration errors
- Consistent naming (Sanskrit, deity names)
- Complete metadata in publication log

---

# Performance Framework

Track but do not optimize solely for:

| Metric | Use |
|--------|-----|
| Saves | Indicates educational value |
| Shares | Indicates resonance |
| Comments | Source of research questions |
| Profile visits | Indicates trust building |
| Follower growth | Lagging indicator |

High saves + meaningful comments > high likes alone.

---

# Related Documents

| Document | Purpose |
|----------|---------|
| `05_Editorial_System.md` | What to produce |
| `06_Visual_System.md` | How it should look |
| `11_Style_Guide.md` | Voice and brand |
| `templates/` | Format templates |
