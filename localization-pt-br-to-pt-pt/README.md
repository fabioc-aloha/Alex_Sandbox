# 🎬 Movie Script Localization: Portuguese Variants

> Localization project for adapting "A Farinha do Mar" across Portuguese regional variants

## Project Info

| Field | Value |
|-------|-------|
| Original Source | Greek (el-GR) with English subtitles |
| Source for Localization | Portuguese (Brazil) - pt-BR |
| Target Languages | pt-PT (Continental), pt-PT-AZ (Azores), pt-BR-SC (Manezinho) |
| Project Type | Movie Script / Screenplay |
| Current Script | "A Farinha do Mar" (The Flour of the Sea) |

## About the Script

**"A Farinha do Mar"** is a dark comedy-drama in three acts based on real events from 2001. The story follows a coastal village when cocaine washes ashore and residents mistake it for flour, baking it into bread with catastrophic and darkly comedic consequences.

| Element | Description |
|---------|-------------|
| Genre | Drama / Dark Comedy |
| Setting | Coastal fishing village, 2001 |
| Acts | 3 (The Tide, The Addiction, The War) |
| Themes | Community, addiction, resilience, class conflict |

## Language Variants

| Code | Variant | Region | Notes |
|------|---------|--------|-------|
| el-GR | Greek Original | Kalymnos, Greece | Original screenplay with English subs |
| pt-BR | Brazilian Standard | Brazil (general) | Canonical Portuguese source |
| pt-PT | European Standard | Portugal (continental) | Primary target |
| pt-PT-AZ | Açoriano | São Miguel, Azores | Archaic features, unique vocab |
| pt-BR-SC | Manezinho | Florianópolis, SC | Azorean-influenced Brazilian |

## Quick Start

1. Place original scripts in `scripts/original/`
2. Review `GLOSSARY.md` and `STYLE-GUIDE.md`
3. Check regional dialect guides for target variant
4. Create localized version in appropriate `scripts/localized-*` folder
5. Run through `qa/review-checklist.md`

## Folder Structure

| Folder | Purpose |
|--------|---------|
| `scripts/original/` | Original pt-BR screenplays (canonical source) |
| `scripts/localized/` | Localized versions (pt-PT continental + Greek original) |
| `scripts/localized-azores/` | Localized pt-PT-AZ (Açoriano) versions |
| `scripts/localized-manezinho/` | Localized pt-BR-SC (Manezinho) versions |
| `reference/` | Vocabulary, grammar, expressions, dialect guides |
| `qa/` | Quality assurance checklists |

## Key Resources

### Core Guides
- [Glossary](GLOSSARY.md) - Term mappings pt-BR → pt-PT
- [Style Guide](STYLE-GUIDE.md) - Localization standards
- [Grammar Rules](reference/grammar-rules.md) - Syntactic transformations
- [Expressions](reference/expressions.md) - Idiom equivalents

### Regional Variants
- [Azores Portuguese](reference/azores-portuguese.md) - Açoriano dialect guide
- [Manezinho](reference/manezinho-floripa.md) - Florianópolis dialect guide

## Status

### Scripts Available

| Version | File | Lines | Status |
|---------|------|-------|--------|
| Greek + English | `a-farinha-do-mar_el-GR_en-subs.md` | 903 | ✅ Complete |
| pt-BR (Standard) | `a-farinha-do-mar_pt-BR.md` | ~600 | ✅ Complete |
| pt-PT (Continental) | `a-farinha-do-mar_pt-PT.md` | ~600 | ✅ Complete |
| pt-PT-AZ (Azores) | `a-farinha-do-mar_pt-PT-AZ.md` | 575 | ✅ Complete |
| pt-BR-SC (Manezinho) | `a-farinha-do-mar_pt-BR-SC.md` | 603 | ✅ Complete |

### Localization Checklists

#### pt-PT (Continental)
- [x] Glossary complete
- [x] Style guide defined
- [x] Full script localized
- [x] "Tu" conjugation applied
- [x] Clitic placement (enclisis)
- [x] Gerund → "a + infinitive"
- [ ] Native speaker review

#### pt-PT-AZ (Azores)
- [x] Dialect guide created
- [x] Vocabulary documented
- [x] Full script localized
- [x] Azorean expressions ("Espia", "cheira-me a esturro")
- [x] Local food references (massa sovada, bolo lêvedo)
- [x] GNR as police force
- [ ] Native speaker review

#### pt-BR-SC (Manezinho)
- [x] Dialect guide created
- [x] Vocabulary documented
- [x] Full script localized
- [x] Manezinho expressions ("Ô", "cruz credo", "tri")
- [x] Local food references (pirão, tainha)
- [x] Cantado accent notation
- [ ] Native speaker review

## Character Adaptation Table

| Role | Greek | pt-BR | pt-PT | Azores | Manezinho |
|------|-------|-------|-------|--------|-----------|
| Protagonist | Μπαρμπα-Μανώλης | Seu Manuel | Ti Manuel | Ti Manuel | Seu Mané |
| Baker | Κυρα-Μαρία | Dona Maria | Maria das Dores | Maria das Dores | Dona Maria |
| Son | Γιώργος | Jorge | Jorge | Zé Augusto | Zé Augusto |
| Villain | Κώστας "Ο Αθηναίος" | Carlos "O Paulista" | Carlos "O Brasileiro" | Carlos "O Brasileiro" | Carlos "O Paulista" |
| Henchman | Νίκος | Nino | Nino | Toninho | Toninho |

## Created By

Alex Cognitive Architecture - Localization Skill

---

*Last updated: 2026-01-31*
