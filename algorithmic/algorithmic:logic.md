# Algorithmic Logic

This document defines the logic operators, rules, truth constraints, and evaluators  
used across all flows in the coherence system.

## Canonical Operators

- **ALIGN(x, y)**  
  Returns true if x structurally and semantically aligns with y.

- **WEIGHT(signal)**  
  Computes weighted importance based on signal origin, strength, and cross-layer validation.

- **COHERE(a, b)**  
  Returns a coherence score between two components.

- **THRESHOLD(value, limit)**  
  Tests whether a value passes or fails a system threshold.

- **RESOLVE(state)**  
  Performs reconciliation when a component violates rules or invariants.

## Logical Constraints

1. No logic may contradict `root/principles.md`.  
2. Evaluation ordering must follow:  
   `structure → logic → flows`.  
3. Operators may not shortcut reconciliation.  
4. All truth values must be explainable via definitions in the framework.

## Truth Rules

- Truth is inherited from the root.  
- Logic is derived, never primary.  
- A failure in `COHERE()` triggers a reconciliation check.  
- A failed `THRESHOLD()` invokes escalation to the framework.

## Systemic Logic Flow

1. Read structural intent  
2. Evaluate signals  
3. Compute alignment  
4. Compute coherence  
5. Evaluate thresholds  
6. Initiate or skip reconciliation  
7. Emit final state

Logic governs behavior; behavior must honor structure.

