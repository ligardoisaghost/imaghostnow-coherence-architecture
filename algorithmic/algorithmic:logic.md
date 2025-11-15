# Algorithmic Logic

This file defines the operational logic rules the system applies during evaluation.

## Core Logic
1. **Coherence-First Evaluation**  
   Every operation must preserve coherence or elevate it.

2. **Minimal Contradiction Principle**  
   Conflicting data is not discarded; it is logged, weighted, and re-evaluated.

3. **Bidirectional Reasoning Loop**  
   Top-down and bottom-up checks occur in alternating cycles.

4. **Temporal Anchoring**  
   Every inference is tied to its time source to prevent drift.

## Operators
- ASSERT() — Introduces a new fact with source metadata.  
- RECONCILE() — Harmonizes conflicting states.  
- TRACE() — Retrieves causal chain for a coherence check.  
- WEIGH() — Assigns confidence scores.

## Notes
Logic rules here are enforced by all upper-level layers.
