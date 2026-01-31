# 🎬 Movie Script Localization: Portuguese Variants

> Localization project for adapting Portuguese scripts across regional variants

## Project Info

| Field | Value |
|-------|-------|
| Source Language | Portuguese (Brazil) - pt-BR |
| Target Languages | pt-PT (Continental), pt-PT-AZ (Azores), pt-BR-SC (Manezinho) |
| Project Type | Movie Script / Screenplay |

## Language Variants

| Code | Variant | Region | Notes |
|------|---------|--------|-------|
| pt-BR | Brazilian Standard | Brazil (general) | Source language |
| pt-PT | European Standard | Portugal (continental) | Primary target |
| pt-PT-AZ | Açoriano | Azores Islands | Archaic features, unique vocab |
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
| `scripts/original/` | Original pt-BR screenplays |
| `scripts/localized/` | Localized pt-PT (continental) versions |
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

### pt-PT (Continental)
- [x] Glossary complete
- [x] Style guide defined
- [ ] Scene 1 localized
- [ ] QA review passed

### pt-PT-AZ (Azores)
- [x] Dialect guide created
- [ ] Vocabulary documented
- [ ] Sample localization

### pt-BR-SC (Manezinho)
- [x] Dialect guide created
- [ ] Vocabulary documented
- [ ] Sample localization

## Created By

Alex Cognitive Architecture - Localization Skill
