# DK-Dialect-Inheritance-Pattern

> Cross-domain pattern: Linguistic dialect evolution mirrors object-oriented inheritance

## Discovery Context

- **Date**: January 31, 2026
- **Project**: localization-pt-br-to-pt-pt
- **Trigger**: Creating Açoriano and Manezinho dialect guides

## The Pattern

Dialect relationships follow inheritance patterns similar to object-oriented programming:

```text
┌─────────────────────────────────────────────────────────────────┐
│                 DIALECT INHERITANCE TREE                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   Portuguese (Base Class)                                        │
│   ├── pt-PT (European Portuguese)                                │
│   │   ├── Continental (Standard)                                 │
│   │   └── Açoriano (Regional Variant)                            │
│   │       └── [inherited by] Manezinho (via migration)           │
│   │                                                              │
│   └── pt-BR (Brazilian Portuguese)                               │
│       ├── Standard (Paulista/Carioca)                            │
│       ├── Nordestino (Regional)                                  │
│       └── Manezinho (Azorean + Brazilian fusion)                 │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

## Inheritance Behaviors

| OOP Concept | Linguistic Equivalent | Example |
|-------------|----------------------|---------|
| **Base Class** | Parent dialect | Açoriano (15th-18th century) |
| **Derived Class** | Descendant dialect | Manezinho (modern) |
| **Inherited Method** | Preserved feature | "Tu" pronoun usage |
| **Overridden Method** | Simplified feature | "Tu vai" vs "Tu vais" |
| **New Method** | Innovation | Gaúcho loanwords (bah, tchê) |
| **Abstract Method** | Lost feature | "Vós" formal plural |
| **Interface** | Mutual intelligibility | All Portuguese variants understand each other |

## Practical Applications

### 1. Localization Architecture
Structure localization projects as inheritance hierarchies:
- Base glossary (common terms)
- Regional overrides (variant-specific terms)
- Dialect extensions (local innovations)

### 2. Translation Memory Design
Build TMs with inheritance:
- Parent TM: Core language pair
- Child TM: Regional adaptations
- Fallback chain: Regional → Standard → Base

### 3. Terminology Management
Version control terminology like code:
- Main branch = standard language
- Feature branches = regional variants
- Merge conflicts = competing usage

## Evidence from This Project

| Feature | Açoriano (Base) | Manezinho (Derived) | Standard pt-BR |
|---------|-----------------|---------------------|----------------|
| 2nd person | Tu (conjugated) | Tu (often unconjugated) | Você |
| "Look!" | Espia | Olha | Olha |
| Maritime vocab | Extensive | Preserved | Different |
| Prosody | Sing-song | Sing-song (inherited) | Flat |
| "Young woman" | Rapariga (neutral) | Rapariga (neutral) | Offensive |

## Cross-Domain Transfer Potential

This pattern applies to:
- **Software localization** - UI string inheritance
- **Content strategy** - Regional content variants
- **Knowledge management** - Document version trees
- **API versioning** - Backwards compatibility chains

## Synapse Connections

- [localization/SKILL.md] → Pattern discovered during localization work
- [bootstrap-learning.instructions.md] → Cross-domain knowledge transfer
- [cross-domain-transfer.prompt.md] → Applying pattern to other domains

---

*Pattern discovered during meditation on Portuguese dialect localization project*
