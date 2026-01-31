# 📊 Data & Analysis

## Data Management

### Folder Structure

| Folder        | Contents                         | Access Level |
| ------------- | -------------------------------- | ------------ |
| `raw/`        | Unprocessed data (anonymized)    | Restricted   |
| `processed/`  | Cleaned, transformed data        | Restricted   |
| `analysis/`   | Statistical outputs, visualizations | Open      |
| `codebooks/`  | Variable definitions, coding schemes | Open     |

## Data Sources

### Phase 1: Survey Data

| Dataset       | Format    | Variables | Expected N |
| ------------- | --------- | --------- | ---------- |
| Demographics  | CSV       | ~15       | 250        |
| Trust Scales  | CSV       | ~40       | 250        |
| Scenarios     | CSV       | ~20       | 250        |
| AI Experience | CSV       | ~10       | 250        |

### Phase 2: Interview Data

| Dataset         | Format     | Files      | Expected   |
| --------------- | ---------- | ---------- | ---------- |
| Transcripts     | DOCX/TXT   | 25-30      | ~20-30 hrs |
| Audio (backup)  | MP3        | 25-30      | Encrypted  |
| Codes           | NVivo/CSV  | 1          | ~200 codes |
| Themes          | DOCX       | 1          | ~10 themes |

### Phase 3: Usability Data

| Dataset         | Format    | Variables | Expected N |
| --------------- | --------- | --------- | ---------- |
| Task Performance| CSV       | ~10       | 15-20      |
| SUS Scores      | CSV       | 10        | 15-20      |
| Think-aloud     | DOCX      | 15-20     | ~15 hrs    |

## Analysis Pipeline

```text
┌─────────────────────────────────────────────────────────────────┐
│                      ANALYSIS WORKFLOW                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   RAW DATA          PROCESSING         ANALYSIS         OUTPUT  │
│   ┌────────┐       ┌──────────┐       ┌─────────┐     ┌───────┐ │
│   │ Survey │──────▶│  Clean   │──────▶│   SEM   │────▶│Tables │ │
│   │ Export │       │ Recode   │       │  CFA    │     │Figures│ │
│   └────────┘       └──────────┘       └─────────┘     └───────┘ │
│                                                                  │
│   ┌────────┐       ┌──────────┐       ┌─────────┐     ┌───────┐ │
│   │ Audio  │──────▶│Transcribe│──────▶│ Thematic│────▶│Themes │ │
│   │        │       │  Clean   │       │ Analysis│     │Quotes │ │
│   └────────┘       └──────────┘       └─────────┘     └───────┘ │
│                                                                  │
│   ┌────────┐       ┌──────────┐       ┌─────────┐     ┌───────┐ │
│   │ Usabil │──────▶│  Score   │──────▶│Descrip- │────▶│Report │ │
│   │  Data  │       │ Compile  │       │  tives  │     │       │ │
│   └────────┘       └──────────┘       └─────────┘     └───────┘ │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

## Variable Codebook Template

### Survey Variables

| Variable     | Label                    | Type        | Values/Range      |
| ------------ | ------------------------ | ----------- | ----------------- |
| ID           | Participant ID           | Nominal     | P001-P999         |
| AGE          | Age in years             | Continuous  | 18-99             |
| GENDER       | Gender identity          | Nominal     | 1=M, 2=F, 3=NB, 4=Other |
| INDUSTRY     | Industry sector          | Nominal     | 1-10 (see legend) |
| AI_EXP       | Years using AI tools     | Continuous  | 0-20              |
| TRUST_1      | Trust scale item 1       | Ordinal     | 1-7 Likert        |
| ...          | ...                      | ...         | ...               |

### Qualitative Codes

| Code ID | Code Name           | Definition                           | Example Quote |
| ------- | ------------------- | ------------------------------------ | ------------- |
| TR01    | Initial Trust       | First impressions of AI system       | TBD           |
| TR02    | Trust Building      | Experiences that increased trust     | TBD           |
| TR03    | Trust Breakdown     | Events that damaged trust            | TBD           |
| ...     | ...                 | ...                                  | ...           |

## Reproducibility

### Scripts Location

| Script           | Purpose                    | Language |
| ---------------- | -------------------------- | -------- |
| `01_clean.R`     | Data cleaning              | R        |
| `02_describe.R`  | Descriptive statistics     | R        |
| `03_cfa.R`       | Confirmatory factor analysis | R      |
| `04_sem.R`       | Structural equation model  | R        |
| `05_figures.R`   | Publication figures        | R        |

### Software Versions

Document all software versions for reproducibility:

- R version: X.X.X
- Key packages: lavaan, tidyverse, ggplot2
- NVivo version: X
- SPSS version: X (if used)

## Data Security

| Measure            | Implementation                          |
| ------------------ | --------------------------------------- |
| Anonymization      | No names, randomized IDs                |
| Encryption         | AES-256 for storage                     |
| Access Control     | Password-protected folders              |
| Backup             | 3-2-1 rule (3 copies, 2 media, 1 offsite) |
| Retention          | Per IRB protocol (typically 5-7 years)  |

## FAIR Principles

| Principle      | Implementation                              |
| -------------- | ------------------------------------------- |
| Findable       | DOI on publication, metadata documented     |
| Accessible     | Repository deposit (OSF, Zenodo)            |
| Interoperable  | Standard formats (CSV, JSON)                |
| Reusable       | Clear documentation, license specified      |
