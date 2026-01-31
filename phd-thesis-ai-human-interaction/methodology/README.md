# 🔬 Methodology

## Research Design

**Mixed Methods Sequential Explanatory Design**

This design uses quantitative data collection and analysis followed by qualitative data collection and analysis to explain and elaborate on quantitative findings.

```text
┌─────────────────────────────────────────────────────────────────┐
│                    RESEARCH DESIGN FLOW                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   Phase 1 (QUAN)        Phase 2 (QUAL)        Phase 3 (DESIGN)  │
│   ┌──────────────┐     ┌──────────────┐     ┌──────────────┐    │
│   │   Survey     │────▶│  Interviews  │────▶│  Prototype   │    │
│   │   N=200-300  │     │   N=20-30    │     │   N=15-20    │    │
│   └──────────────┘     └──────────────┘     └──────────────┘    │
│          │                    │                    │             │
│          ▼                    ▼                    ▼             │
│   ┌──────────────┐     ┌──────────────┐     ┌──────────────┐    │
│   │  Statistical │     │   Thematic   │     │  Usability   │    │
│   │   Analysis   │     │   Analysis   │     │   Testing    │    │
│   └──────────────┘     └──────────────┘     └──────────────┘    │
│          │                    │                    │             │
│          └────────────────────┴────────────────────┘             │
│                               │                                  │
│                               ▼                                  │
│                    ┌──────────────────┐                          │
│                    │    INTEGRATION   │                          │
│                    │   & FRAMEWORK    │                          │
│                    └──────────────────┘                          │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

## Phase 1: Quantitative Survey

### Purpose

Measure relationships between cognitive factors, organizational factors, trust calibration, and decision quality in human-AI collaboration.

### Constructs & Measures

| Construct                | Measure                        | Source                    |
| ------------------------ | ------------------------------ | ------------------------- |
| Trust in AI              | Trust in Automation Scale      | Jian et al. (2000)        |
| Propensity to Trust      | General Trust Scale            | Mayer & Davis (1999)      |
| Cognitive Load           | NASA-TLX                       | Hart & Staveland (1988)   |
| AI Literacy              | AI Literacy Scale              | Ng et al. (2021)          |
| Reliance Behavior        | Behavioral scenarios           | Custom development        |
| Decision Quality         | Accuracy metrics               | Task-specific             |
| Explanation Satisfaction | XAI Satisfaction Scale         | Hoffman et al. (2018)     |

### Sampling

| Criterion        | Specification                              |
| ---------------- | ------------------------------------------ |
| Population       | Enterprise employees using AI tools        |
| Sampling Method  | Stratified by industry and role            |
| Target N         | 250 (minimum 200 for SEM)                  |
| Industries       | Tech, Finance, Healthcare, Manufacturing   |
| Roles            | Analysts, Managers, Executives             |

### Analysis Plan

1. Descriptive statistics
2. Confirmatory Factor Analysis (CFA)
3. Structural Equation Modeling (SEM)
4. Mediation/moderation analysis
5. Multi-group analysis by industry

## Phase 2: Qualitative Interviews

### Purpose

Explore and explain quantitative findings through rich, detailed accounts of human-AI interaction experiences.

### Interview Protocol

| Section            | Duration | Topics                                           |
| ------------------ | -------- | ------------------------------------------------ |
| Introduction       | 5 min    | Purpose, consent, rapport                        |
| AI Experience      | 15 min   | Current AI use, decision contexts                |
| Trust Development  | 20 min   | How trust formed, critical incidents             |
| Challenges         | 15 min   | Over/under-reliance experiences                  |
| Ideal State        | 10 min   | What would improve collaboration                 |
| Wrap-up            | 5 min    | Additional thoughts, thank you                   |

### Sampling Strategy

- Purposive sampling from Phase 1 respondents
- Maximum variation on trust scores (high, medium, low)
- Ensure diversity in industry and role

### Analysis

- Thematic analysis (Braun & Clarke, 2006)
- Coding in NVivo/Atlas.ti
- Member checking for validity

## Phase 3: Design Intervention

### Purpose

Develop and test a prototype AI interface incorporating research findings.

### Design Process

1. **Synthesize** findings from Phases 1 & 2
2. **Ideate** design solutions with stakeholders
3. **Prototype** key trust-building features
4. **Test** with new participants
5. **Iterate** based on feedback

### Evaluation Criteria

| Criterion           | Measure                           |
| ------------------- | --------------------------------- |
| Usability           | System Usability Scale (SUS)      |
| Trust Calibration   | Pre/post trust measures           |
| Decision Accuracy   | Task performance                  |
| User Satisfaction   | Post-task questionnaire           |

## Validity & Reliability

### Quantitative

| Threat                | Mitigation                                  |
| --------------------- | ------------------------------------------- |
| Internal validity     | Control variables, randomization            |
| External validity     | Diverse sample, multiple industries         |
| Construct validity    | Validated scales, pilot testing             |
| Statistical conclusion| Adequate sample size, effect size reporting |

### Qualitative

| Criterion             | Strategy                                    |
| --------------------- | ------------------------------------------- |
| Credibility           | Member checking, prolonged engagement       |
| Transferability       | Thick description, diverse sample           |
| Dependability         | Audit trail, peer debriefing                |
| Confirmability        | Reflexivity, multiple coders                |

## Ethical Considerations

### IRB Requirements

- [ ] Submit IRB application
- [ ] Informed consent forms
- [ ] Data management plan
- [ ] Risk assessment

### Data Protection

- All data anonymized
- Secure storage (encrypted)
- Participant right to withdraw
- GDPR/CCPA compliance if applicable

### AI Ethics

- Transparent about AI use in research
- No deception in AI scenarios
- Fair representation of AI capabilities

## Folder Structure

| Folder          | Contents                               |
| --------------- | -------------------------------------- |
| `instruments/`  | Survey, interview guide, scales        |
| `protocols/`    | IRB, consent forms, procedures         |
| `pilots/`       | Pilot study materials and results      |
| `analysis/`     | Analysis scripts and codebooks         |

## Tools

| Purpose          | Tool                                   |
| ---------------- | -------------------------------------- |
| Survey           | Qualtrics / SurveyMonkey               |
| Statistics       | R / SPSS / AMOS                        |
| Qual Analysis    | NVivo / Atlas.ti                       |
| Transcription    | Otter.ai / Rev                         |
| Prototyping      | Figma / Adobe XD                       |
