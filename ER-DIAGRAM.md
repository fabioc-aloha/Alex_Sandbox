# Entity Relationship Diagram

> Mermaid ER diagram representing the workspace structure

```mermaid
erDiagram
    %% ========================================
    %% PhD Thesis Project
    %% ========================================

    THESIS {
        string title "AI-Human Interaction"
        string degree "DBA"
        string researcher "Fabio Correa"
        string orcid "0009-0000-2271-9380"
        string status "In Progress"
    }

    RESEARCH_QUESTION {
        int id PK
        string code "RQ1, RQ2, RQ3"
        string question
        string focus_area
    }

    CHAPTER {
        int number PK
        string title
        string status "Drafting|Planned"
    }

    LITERATURE {
        string id PK
        string type "source|note|synthesis|gap"
        string topic
        string citation
    }

    METHODOLOGY {
        string id PK
        string type "protocol|instrument|pilot|analysis"
        string description
    }

    DATA {
        string id PK
        string type "raw|processed|codebook|analysis"
        string description
    }

    MILESTONE {
        string name PK
        date target_date
        string status "Pending|Complete"
    }

    THESIS ||--o{ RESEARCH_QUESTION : "investigates"
    THESIS ||--o{ CHAPTER : "contains"
    THESIS ||--o{ MILESTONE : "tracks"
    CHAPTER ||--o{ LITERATURE : "references"
    THESIS ||--o{ METHODOLOGY : "employs"
    METHODOLOGY ||--o{ DATA : "produces"
    DATA ||--o{ CHAPTER : "informs"

    %% ========================================
    %% Localization Project
    %% ========================================

    LOCALIZATION_PROJECT {
        string name PK
        string source_language "pt-BR"
        string project_type "Movie Script"
    }

    LANGUAGE_VARIANT {
        string code PK "pt-BR|pt-PT|pt-PT-AZ|pt-BR-SC"
        string name
        string region
        string notes
    }

    SCRIPT {
        string id PK
        string title
        string type "original|localized"
        string variant_code FK
    }

    GLOSSARY {
        string term_id PK
        string source_term
        string target_term
        string variant_code FK
    }

    STYLE_GUIDE {
        string id PK
        string rule_type
        string description
    }

    REFERENCE_MATERIAL {
        string id PK
        string type "vocabulary|grammar|expressions|dialect"
        string variant_code FK
        string content
    }

    QA_CHECKLIST {
        string id PK
        string check_item
        boolean passed
    }

    LOCALIZATION_PROJECT ||--o{ LANGUAGE_VARIANT : "targets"
    LOCALIZATION_PROJECT ||--o{ SCRIPT : "contains"
    SCRIPT }o--|| LANGUAGE_VARIANT : "written_in"
    LOCALIZATION_PROJECT ||--|| GLOSSARY : "uses"
    LOCALIZATION_PROJECT ||--|| STYLE_GUIDE : "follows"
    LANGUAGE_VARIANT ||--o{ REFERENCE_MATERIAL : "documented_by"
    SCRIPT ||--o{ QA_CHECKLIST : "validated_by"
    GLOSSARY }o--|| LANGUAGE_VARIANT : "maps_to"
```

## Entity Descriptions

### PhD Thesis Project

| Entity | Description |
|--------|-------------|
| `THESIS` | Main doctoral research on AI-Human Interaction |
| `RESEARCH_QUESTION` | Three RQs about AI reliance, trust, and transparency |
| `CHAPTER` | Seven thesis chapters with progress tracking |
| `LITERATURE` | Academic sources, notes, synthesis, and gap analysis |
| `METHODOLOGY` | Research protocols, instruments, pilots, analysis methods |
| `DATA` | Raw data, processed outputs, codebooks, analysis results |
| `MILESTONE` | Key deadlines and deliverables |

### Localization Project

| Entity | Description |
|--------|-------------|
| `LOCALIZATION_PROJECT` | Movie script adaptation across Portuguese variants |
| `LANGUAGE_VARIANT` | pt-BR, pt-PT, pt-PT-AZ (Azores), pt-BR-SC (Manezinho) |
| `SCRIPT` | Original and localized screenplay versions |
| `GLOSSARY` | Term mappings between language variants |
| `STYLE_GUIDE` | Localization standards and conventions |
| `REFERENCE_MATERIAL` | Vocabulary, grammar, expressions, dialect guides |
| `QA_CHECKLIST` | Quality assurance validation items |
