# 🎨 Localization Style Guide

## Core Principles

1. **Preserve character voice** - Personality > literal translation
2. **Natural dialogue** - Must sound native to Portuguese ears
3. **Lip-sync awareness** - Consider dubbing timing
4. **Cultural equivalence** - Adapt references appropriately

---

## Pronoun System

### Second Person Transformation

| 🇧🇷 Brazilian | 🇵🇹 European | Notes |
|--------------|--------------|-------|
| Você fala | Tu falas | Informal contexts |
| Você pode | Tu podes | With verb conjugation |
| O senhor / A senhora | O senhor / A senhora | Formal (keep same) |

**Example:**
```
BR: Você não pode fazer isso!
PT: Tu não podes fazer isto!
```

### When to Keep "Você"

- Very formal contexts (business, elderly respect)
- When character is deliberately distancing
- Regional character from Alentejo (where "você" is common)

---

## Clitic Pronoun Placement

### Rule: Move pronouns AFTER the verb (enclisis) in pt-PT

| 🇧🇷 Brazilian | 🇵🇹 European |
|--------------|--------------|
| Me dá isso | Dá-me isso |
| Te amo | Amo-te |
| Ele me disse | Ele disse-me |
| Ela se levantou | Ela levantou-se |
| Vou te contar | Vou contar-te |

### Exceptions (proclisis - pronoun BEFORE verb)

**After negation:**
```
Não me digas isso.
Nunca te esquecerei.
Ninguém me viu.
```

**After certain adverbs:**
```
Já te disse.
Ainda me lembro.
Sempre te amei.
Também me parece.
```

**In subordinate clauses:**
```
Espero que me ligues.
Quando te vi...
Se me deres tempo...
O homem que te ajudou.
```

**After question words:**
```
Quem te disse?
O que lhe aconteceu?
Onde te meteste?
```

---

## Gerund → a + Infinitive

### Standard Transformation

| 🇧🇷 Brazilian | 🇵🇹 European |
|--------------|--------------|
| Estou fazendo | Estou a fazer |
| Ela está chorando | Ela está a chorar |
| Continuou andando | Continuou a andar |
| Ficou olhando | Ficou a olhar |
| Anda trabalhando | Anda a trabalhar |

### Verbs That Use This Pattern

- estar + gerund → estar + a + infinitive
- continuar + gerund → continuar + a + infinitive
- ficar + gerund → ficar + a + infinitive
- andar + gerund → andar + a + infinitive
- vir + gerund → vir + a + infinitive (sometimes)

---

## Demonstratives

| Distance | 🇧🇷 Brazilian | 🇵🇹 European |
|----------|--------------|--------------|
| Near speaker | Isso (general) | Isto |
| Near listener | Isso | Isso |
| Far from both | Aquilo | Aquilo |

**Rule:** pt-PT maintains three-way distinction more strictly

```
BR: Isso é muito bom.
PT: Isto é muito bom. (if referring to something nearby)
```

---

## Contractions

| Full Form | 🇧🇷 Spoken | 🇵🇹 Written |
|-----------|-----------|-------------|
| para + a | pra | para a |
| para + o | pro | para o |
| está | tá | está |
| estava | tava | estava |

**Note:** pt-PT prefers full forms in written dialogue. Use contractions only for very casual/young characters.

---

## Register Guidelines

| Character Type | pt-BR Register | pt-PT Equivalent |
|----------------|----------------|------------------|
| Young urban | Gírias cariocas | Calão lisboeta |
| Formal elderly | Senhor/Senhora | Senhor/Senhora |
| Working class | Coloquial popular | Coloquial popular |
| Professional | Formal neutro | Formal neutro |
| Child | Infantil | Infantil |
| Criminal/Street | Gíria marginal | Calão da rua |

### Youth Slang Equivalents

| 🇧🇷 Brazilian | 🇵🇹 European |
|--------------|--------------|
| Mano | Mano / Bro |
| Véi | Pá |
| Tipo | Tipo |
| Mó legal | Bué fixe |
| Zueira | Gozo |

---

## Formatting Standards

### Script Format
```
CENA [N] - [INT./EXT.] [LOCALIZAÇÃO] - [TEMPO]

[Descrição de ação em português europeu]

                    PERSONAGEM
          (indicação de cena)
    Diálogo em português europeu.
```

### File Naming Convention
```
original:   nome-do-filme_pt-BR_v1.fountain
localized:  nome-do-filme_pt-PT_v1.fountain
```

### Version Control
- `v1` = First draft
- `v2` = Post-review revision
- `v3` = Final approved version
- Add `_FINAL` suffix for delivery version

---

## Common Pitfalls

### ❌ Avoid

1. **Over-translating** - Don't change what doesn't need changing
2. **Mixing registers** - Don't have a street kid speaking formally
3. **False friends** - Watch for words that look similar but differ in meaning
4. **Cultural impositions** - Don't force Brazilian references into Portuguese context

### ✅ Remember

1. **Read aloud** - If it sounds unnatural, revise
2. **Character consistency** - Each character should have consistent speech patterns
3. **Context matters** - Same word may need different translations in different scenes
4. **When in doubt** - Consult a native pt-PT speaker
