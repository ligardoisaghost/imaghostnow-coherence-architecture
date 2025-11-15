# Root Structure Map

The root structure describes how the major layers fit together.  
It provides a stable map so that future changes don’t drift into chaos.

## Top-Level Layers

- `root/` – Identity, principles, invariants, and flows.  
- `framework/` – Abstract structure, layers, and cross-layer relationships.  
- `algorithmic/` – Logic, evaluation rules, and dynamic behavior.  
- `data/` – Schemas, data contracts, and ingestion/exposure flows.  
- `diagrams/` – System maps, pipelines, and visual coherence graphs.  
- `architecture/` – Concrete system components, interfaces, and contracts.  
- `visual/` – Visual metaphors, palette, and aesthetic constraints.  
- `creative/` – Narrative tone, motifs, voice, and story logic.  
- `papers/` – Formal treatments, research agenda, and whitepaper.  
- `phase/` – Lifecycle states, cycles, and temporal behavior.  
- `src/` – Implementations, scripts, and pipelines.  
- `notes/` – Changelog, backlog, and working notes.

## Structural Relationships

- `root/` ← anchors every other directory.  
- `framework/` ← defines the schema of how layers talk to each other.  
- `algorithmic/` ← encodes the behavior assumed by `framework/`.  
- `data/` + `diagrams/` ← provide the observable evidence that the model matches reality.  
- `architecture/` ← binds the above into concrete components and interfaces.  
- `visual/` + `creative/` ← expose the system to humans in a coherent way.  
- `phase/` ← tracks where in the lifecycle any experiment or deployment is.  
- `src/` ← is the operational surface that must not drift from this map.

Any new directory or major refactor must be reflected here first.
