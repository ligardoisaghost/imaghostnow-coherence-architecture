# Framework Overview

The framework layer defines the architectural skeleton of the IMAGHOSTNOW Coherence Architecture.  
This layer establishes how subsystems interact, what dependencies exist, and how coherence flows through the structure.

## Purpose
The framework layer maps the global architecture into discrete layers:  
logic, structure, behavior, representation, and execution.

Each layer defines a different dimension of coherence.  
Nothing in the system may violate the order or meaning of these layers.

## Contents
- **overview.md** – High-level description of architectural purpose and hierarchy.
- **layers.md** – Defines each coherence layer and its responsibilities.
- **invariants.md** – Lists the global rules that cannot be violated anywhere in the system.

## Notes
The framework layer is authoritative: downstream systems must conform to it.  
Changes require justification and alignment with the root layer.
