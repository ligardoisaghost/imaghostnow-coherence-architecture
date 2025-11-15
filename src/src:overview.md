# Source Layer Overview

The source layer defines the operational mechanics of the IMAGHOSTNOW
Coherence Architecture.  
Where other layers describe structure or semantics, the source layer describes
execution: how coherence is calculated, maintained, and propagated.

## Purpose

- Provide the minimal operational core
- Define executable transformations
- Establish the order of evaluation
- Coordinate flows across all layers
- Maintain deterministic behavior across systems

## Structure

- `overview.md` — purpose and execution outline  
- `core.md` — operational primitives and internal functions  
- `pipelines.md` — multi-stage coherence evaluation pipelines  

## Notes

The source layer is not conceptual.  
It is the closest representation of the system’s “engine.”