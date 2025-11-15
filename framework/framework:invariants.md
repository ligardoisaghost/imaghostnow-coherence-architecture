# Framework Invariants

Framework invariants define non-negotiable structural truths.  
If any component or layer violates these, the architecture becomes incoherent.

## Invariant 1 — Single Layer Schema
All layers must be defined in `framework/layers.md`.  
No unofficial or implicit layers are allowed.

## Invariant 2 — One-Way Anchoring
Anchors flow downward only:
root → framework → algorithmic → architecture → src.

No lower layer may override assumptions of a higher one.

## Invariant 3 — Boundary Integrity
Each layer defines:
- what it contains  
- what it references  
- what it may not touch  

Violating boundaries is a structural breach.

## Invariant 4 — Cross-Layer Consistency
Definitions that appear in multiple layers must agree.  
Disagreement triggers a reconciliation cycle via root → framework.

## Invariant 5 — Change Propagation
Any change at the framework level MUST:

1. update `framework/layers.md`  
2. update relevant cross-layer documents  
3. record rationale in `notes/changelog.md`  

Framework changes ripple through the entire architecture.

## Invariant 6 — Schema Stability
The layer schema may evolve, but only through explicit, documented revision.  
Untracked evolution is treated as model corruption.
