# Root Flows

These flows govern how information, state, and signals move through the system.

## Canonical Flows

1. **Coherence Propagation**  
   Changes in one layer propagate to others through explicit links  
   (root → framework → algorithmic → architecture → src).

2. **State Evaluation Loop**  
   - Observe current system state (data + diagrams).  
   - Compare against expectations (root + framework + algorithmic).  
   - Classify result as aligned, drifting, or incoherent.  
   - Record the outcome in notes or papers.

3. **Signal Alignment Pass**  
   External signals (analytics, experiments, creative results) are normalized  
   and mapped into the coherence model before influencing structure.

4. **Cross-Layer Reconciliation Cycle**  
   - Detect conflicts between layers (e.g., architecture vs. creative).  
   - Trace them back to root assumptions.  
   - Either update assumptions or realign the implementation.

## Cross-Layer Links

- `algorithmic/` implements flows as operators and evaluators.  
- `data/` maps flows into schemas, logs, and systemic diagrams.  
- `framework/` enforces which flows are valid and which are illegal.  
- `architecture/` provides the concrete channels flows travel through.

When a new flow is introduced, it must be:

- described here at a high level,  
- formalized in `framework/` or `algorithmic/`, and  
- observable via `data/` and `diagrams/`.
