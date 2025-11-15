# System Invariants

Invariants are conditions that must remain true for the IMAGHOSTNOW architecture to be considered valid.  
Breaking an invariant means the model and reality have diverged.

## Global Invariants

1. **Single Source of Truth for Structure**  
   The combination of `root/` + `framework/` defines the official structure.  
   No other file is allowed to redefine the global topology.

2. **Layer Boundaries Are Explicit**  
   Every file belongs to exactly one primary layer, even if it references others.

3. **Versioned Change**  
   Any modification to root principles, structure, or flows must be:
   - recorded in `notes/changelog.md`, and  
   - justified with a brief rationale.

4. **Observable Behavior**  
   Every algorithmic or architectural change must have:
   - an expected effect on flows or states, and  
   - a way to verify that effect with data or diagrams.

5. **Cross-Layer Consistency**  
   If two layers describe the same concept (e.g., “phase-2 fingerprint”),  
   their definitions must be reconciled and referenced, not duplicated independently.

6. **Reconstructability**  
   A competent reader, starting from `root/` and `framework/`,  
   must be able to reconstruct the intention behind any component in `src/`.

## Invariant Scope

Each invariant is assumed to apply to:

- current documents and code, and  
- future additions, unless explicitly exempted with justification.

Exemptions must be rare, documented, and temporary.



