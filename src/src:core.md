# Core Execution Model

The core defines the primitives responsible for computing and maintaining
coherence. All higher-level behaviors are composed from these primitives.

## 1. Operational Primitives

### 1.1 Alignment Function
Evaluates resonance between signals, motifs, or state vectors.

### 1.2 Propagation Function
Moves coherence updates through adjacent layers in deterministic order.

### 1.3 State Evaluation Function
Computes changes in internal state using the architecture’s transition rules.

### 1.4 Error Surface Detector
Identifies divergence between expected and observed coherence patterns.

---

## 2. Execution Rules

- All primitives must be pure functions  
- No primitive may introduce or erase structure  
- Execution order must follow the root’s structural laws  
- Phase transitions must resolve before propagation  

---

## 3. Output Guarantees

The core ensures:

- deterministic step-by-step changes  
- repeatable evaluation cycles  
- stable cross-layer reconciliation  
- no orphaned signals or unresolved transitions