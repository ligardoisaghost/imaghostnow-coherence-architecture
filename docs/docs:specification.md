# IMAGHOSTNOW Specification

The specification defines the formal grammar, binding rules, interfaces, and
contractual invariants of the architecture.

## 1. System Grammar

### 1.1 Core Terms
- **Layer** — a semantic division of the architecture  
- **Invariant** — a rule that must hold across all layers  
- **Flow** — directional movement of information or state  
- **Mapping** — explicit representation of cross-layer relationships  

### 1.2 Naming Conventions
- Directories are singular (`root`, `framework`, `phase`)  
- Files use lowercase-with-dashes  
- Cross references use fully qualified paths (`phase/systemstates.md`)  

---

## 2. Coherence Contracts

### 2.1 Root-Level Contracts
- No layer may contradict root invariants  
- System structure must remain globally consistent  
- All cycles must resolve without logical dead-ends  

### 2.2 Layer Interactions
- Each layer must define:  
  - Overview  
  - Internal logic  
  - External expectations  

- Inter-layer flows must be defined in diagrams and data  

---

## 3. Validation Rules

### 3.1 Structural Validation
- All layers must maintain a single, non-fragmented overview  
- Every formal diagram must appear in both `data/` and `diagrams/`  

### 3.2 Logical Validation
- Logic operators must match definitions in `algorithmic/logic.md`  
- No circular references without explicit justification  

---

## 4. External Interfaces

Defines how external tools, systems, or collaborators may interact with the architecture.

### 4.1 Allowed Surfaces
- Visual motifs  
- Structural diagrams  
- System-level states  

### 4.2 Forbidden Surfaces
- Internal invariants  
- Raw state transitions  
- Unresolved TODOs

---

This specification evolves only through formal review and recorded justification in `notes/changelog.md`.
