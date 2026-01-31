# Alex Skills Catalog (Generated)

> Generated: 2026-01-31
> Total Skills: **38** (33 inheritable, 0 master-only, 2 VS Code, 2 M365, 1 temporary)
> Total Connections: **149** (19 bidirectional, 49 weak)

---

## Network Diagram

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'lineColor': '#666', 'primaryColor': '#e8f4f8', 'primaryBorderColor': '#0969da'}}}%%
flowchart LR
    subgraph Other["📦 Other"]
        AR[academic-research]
        AA[architecture-audit]
        BA[business-analysis]
        CM[change-management]
        CW[creative-writing]
        GD[graphic-design]
        L[localization]
        PM[project-management]
    end
    subgraph Cognitive["🧠 Cognitive"]
        AR[appropriate-reliance]
        BL[bootstrap-learning]
        CL[cognitive-load]
        LP[learning-psychology]
    end
    subgraph Architecture["🏗️ Architecture"]
        AH[architecture-health]
        SCG[skill-catalog-generator]
    end
    subgraph Documentation["📝 Documentation"]
        AAA[ascii-art-alignment]
        LCM[lint-clean-markdown]
        MM[markdown-mermaid]
        WP[writing-publication]
    end
    subgraph Temporary["🧪 Temporary"]
        BT[beta-tester]
    end
    subgraph Vscode["💻 Vscode"]
        CPP[chat-participant-patterns]
        VEP[vscode-extension-patterns]
    end
    subgraph Engineering["🔧 Engineering"]
        CR[code-review]
        DP[debugging-patterns]
        GW[git-workflow]
        PS[project-scaffolding]
        RP[refactoring-patterns]
        TS[testing-strategies]
        VE[vscode-environment]
    end
    subgraph Operations["🚨 Operations"]
        ERP[error-recovery-patterns]
        IR[incident-response]
        RP[release-preflight]
        RCA[root-cause-analysis]
    end
    subgraph Visual["🎨 Visual"]
        IH[image-handling]
        SG[svg-graphics]
    end
    subgraph M365["☁️ M365"]
        MAD[m365-agent-debugging]
        TAP[teams-app-patterns]
    end
    subgraph Security["🔐 Security"]
        MS[microsoft-sfi]
        PRA[privacy-responsible-ai]
    end

    %% Connections
    AR <--> WP
    AR --> BL & LP
    AR -.-> RCA & CL
    AAA <--> MM
    AAA --> LCM & WP
    BT --> AH & DP & ERP & RCA
    BT -.-> IR
    BL --> LP & CL & AR
    BA --> PM & CM
    BA -.-> RCA & TS & WP
    CM <--> PM
    CM --> BA
    CM -.-> RCA & AR & CL
    CPP --> VEP & CL
    CR --> TS & GW
    CR -.-> RP
    CL --> LP & AR
    CW <--> WP & AR
    CW -.-> CL & AR
    DP --> GW & VEP
    ERP --> DP & IR & TS
    GW --> RP
    GD <--> CW & MM & AAA
    GD --> VEP
    GD -.-> CL & WP
    IH <--> SG
    IH --> PS & VEP
    IR -.-> RCA
    IR --> ERP & DP
    LP --> AR
    LCM <--> MM
    LCM --> WP
    L <--> TS & VEP & WP & GD
    L -.-> PM & CL & CR
    MM --> WP & LCM
    MS <--> PRA
    MS -.-> CR
    MS --> IR
    PRA --> MS & IR
    PRA -.-> CR
    PM --> BA & RCA
    PM -.-> TS & RP & IR
    PS --> MM & SG & LCM & GW
    RP --> TS & DP & CR & GW & VEP & MAD
    RP <--> BT
    RCA --> DP & IR
    RCA -.-> ERP
    SCG --> MM & AH
    SCG -.-> LP & PS
    SG --> PS & IH & MM
    SG -.-> AAA
    TAP --> MAD & RP
    TS <--> DP
    TS --> RP & CR
    VE --> PS & VEP & GW & DP
    WP --> MM
    WP -.-> LCM & AR

    %% Styling
    classDef master fill:#fff3cd,stroke:#856404
    classDef vscode fill:#e1f0ff,stroke:#0969da
    classDef m365 fill:#e6f4ea,stroke:#1a7f37
    classDef inheritable fill:#e0f7fa,stroke:#00838f
    classDef temp fill:#f3e8ff,stroke:#7c3aed,stroke-dasharray:5 5
    classDef stale stroke-dasharray:5 5,stroke-width:2px

    class CPP,VEP vscode
    class MAD,TAP m365
    class AR,AR,AA,AH,AAA,BL,BA,CM,CR,CL,CW,DP,ERP,GW,GD,IH,IR,LP,LCM,L,MM,MS,PRA,PM,PS,RP,RP,RCA,SCG,SG,TS,VE,WP inheritable
    class BT temp
    class CPP,GW,MAD,MS,PRA,TAP,VEP stale
```

---

## Legend

| Color | Inheritance |
| ----- | ----------- |
| 🟨 Yellow | Master-only |
| 🟦 Blue | VS Code heir |
| 🟩 Green | M365 heir |
| 🟪 Purple (dashed) | Temporary |
| 🧊 Cyan | Inheritable |

| Arrow | Meaning |
| ----- | ------- |
| `<-->` | Bidirectional (mutual) |
| `-->` | Strong connection (≥0.7) |
| `-.->` | Weak connection (<0.7) |

---

## Skills by Inheritance

### 🧊 Inheritable (33)

| Skill | Connections |
| ----- | ----------- |
| academic-research | 6 |
| appropriate-reliance | 4 |
| architecture-audit | 7 |
| architecture-health | 3 |
| ascii-art-alignment | 3 |
| bootstrap-learning | 4 |
| business-analysis | 6 |
| change-management | 7 |
| code-review | 3 |
| cognitive-load | 3 |
| creative-writing | 6 |
| debugging-patterns | 2 |
| error-recovery-patterns | 3 |
| git-workflow | 2 |
| graphic-design | 7 |
| image-handling | 3 |
| incident-response | 3 |
| learning-psychology | 3 |
| lint-clean-markdown | 3 |
| localization | 8 |
| markdown-mermaid | 2 |
| microsoft-sfi | 4 |
| privacy-responsible-ai | 3 |
| project-management | 7 |
| project-scaffolding | 4 |
| refactoring-patterns | 3 |
| release-preflight | 5 |
| root-cause-analysis | 3 |
| skill-catalog-generator | 5 |
| svg-graphics | 4 |
| testing-strategies | 3 |
| vscode-environment | 4 |
| writing-publication | 3 |

### 🟨 Master-Only (0)

| Skill | Connections |
| ----- | ----------- |


### 🟦 VS Code Heir (2)

| Skill | Connections |
| ----- | ----------- |
| chat-participant-patterns | 3 |
| vscode-extension-patterns | 2 |

### 🟩 M365 Heir (2)

| Skill | Connections |
| ----- | ----------- |
| m365-agent-debugging | 1 |
| teams-app-patterns | 2 |

### 🟪 Temporary (1)

| Skill | Connections | Remove After |
| ----- | ----------- | ------------ |
| beta-tester | 5 | stable-release |

---

## Staleness-Prone Skills

| Skill | Reason |
| ----- | ------ |
| vscode-extension-patterns | Platform/API changes frequently |
| chat-participant-patterns | Platform/API changes frequently |
| m365-agent-debugging | Platform/API changes frequently |
| teams-app-patterns | Platform/API changes frequently |
| llm-model-selection | Platform/API changes frequently |
| git-workflow | Platform/API changes frequently |
| privacy-responsible-ai | Platform/API changes frequently |
| microsoft-sfi | Platform/API changes frequently |

---

*Generated by Alex: Generate Skill Catalog command*
