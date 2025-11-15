# Cross-Layer Relationships

This document defines how the layers of the IMAGHOSTNOW Coherence Architecture relate, depend, and propagate change.  
It treats the system as a single structure instead of isolated folders.

---

## 1. Layer roles at a glance

- **root/**  
  Defines identity, invariants, and fundamental flows. Nothing is allowed to contradict this layer.

- **framework/**  
  Wraps the root in stable scaffolding: layers, invariants, and governance rules for change.

- **algorithmic/**  
  Encodes dynamic behavior: evaluation rules, operators, thresholds, and feedback loops.

- **architecture/**  
  Describes structural layouts, components, and interfaces used by the rest of the system.

- **diagrams/**  
  Visual projections of structure, flows, and system maps. Human-readable snapshots of the deeper logic.

- **data/**  
  Tracks system maps, pipelines, and other machine-facing structures derived from diagrams and algorithms.

- **visual/**  
  Governs palette, motifs, and visual voice. Attaches coherence rules to imagery and design.

- **creative/**  
  Holds narrative, sonic, and conceptual motifs. Connects human-facing “story” to structural intent.

- **phase/**  
  Captures states, cycles, and temporal regimes. Describes how the system evolves over time.

- **papers/**  
  Houses formal reasoning and conceptual expansions. Used as an explanation and reference layer.

- **notes/**  
  Scratch space: changelog, todos, and working memory. Records how and why the system changed.

- **docs/**  
  External-facing documentation: overview, specification, and appendices for publication.

- **src/**  
  Source blueprints and pipeline descriptions for eventual code, scripts, and automation.

---

## 2. Primary relationship channels

### 2.1 Root → Framework → Everything

- **root/** defines:
  - Core principles  
  - System invariants  
  - Fundamental flows  

- **framework/**:
  - Interprets those invariants as explicit layers  
  - Defines how layers are allowed to interact  
  - Holds the rules for legal vs illegal change

Every other layer must be consistent with both **root/** and **framework/**. Any violation is treated as a systemic fault.

---

### 2.2 Algorithmic ↔ Architecture

- **architecture/**:
  - Declares components, interfaces, and structural channels
  - Describes where flows are allowed to travel

- **algorithmic/**:
  - Defines the operators and evaluation rules that move through those channels
  - Encodes thresholds, state transitions, and feedback loops

Result: architecture is the “hardware layout”, algorithmic is the “behavioral firmware.”

---

### 2.3 Diagrams ↔ Data ↔ Src

- **diagrams/**:
  - Human-facing system maps and flows
  - Used to reason about structure and change

- **data/**:
  - System maps and pipelines in a machine-oriented form
  - Mirrors the diagram logic in a structured way

- **src/**:
  - Describes how those structures eventually become code, scripts, tools, and pipelines

Path:  
_diagrams_ → _data_ → _src_ → external implementations.

---

### 2.4 Visual ↔ Creative ↔ Phase

- **visual/**:
  - Palette, motifs, and visual voice
  - Ensures images obey coherence rules

- **creative/**:
  - Sonic, narrative, and conceptual motifs
  - Links emotional tone to structural intent

- **phase/**:
  - States, cycles, and temporal regimes
  - Describes when and how visual/creative modes are activated

Together, these layers define how the system “feels” and how that feeling changes over time without breaking structural coherence.

---

### 2.5 Papers ↔ Docs ↔ Notes

- **papers/**:
  - Deep reasoning, formal arguments, and conceptual expansions

- **docs/**:
  - Clean external documentation derived from papers and architecture

- **notes/**:
  - Day-to-day decisions, todos, and change logs

Flow:  
_notes_ capture changes → _papers_ justify them → _docs_ publish the stable picture.

---

## 3. Coherence propagation rules

1. **Root-first**  
   Any structural or behavioral change must reconcile with `root/` and `framework/` before it is considered valid.

2. **Structure before behavior**  
   - Edit `architecture/` and `diagrams/` first.  
   - Then adjust `algorithmic/` and `data/`.  
   - Only then touch `src/`.

3. **Meaning before aesthetics**  
   - Update `root/`, `framework/`, `creative/`, and `phase/` when the system’s meaning or intent shifts.  
   - Only then update `visual/` to reflect the new state.

4. **Documentation as a trailing edge**  
   - `notes/` record the change as it happens.  
   - `papers/` capture the argument once it stabilizes.  
   - `docs/` are updated last, when the new picture is coherent.

---

## 4. Example trace: introducing a new motif

1. Define the intent and constraint in `root/` and `framework/`.  
2. Reflect the structural impact in `architecture/` and `diagrams/`.  
3. Update operators or thresholds in `algorithmic/` and mirrored structures in `data/`.  
4. Describe new pipelines or code plans in `src/`.  
5. Add the motif to `creative/` and lock its visual expression in `visual/`.  
6. Adjust `phase/` to define when this motif is active.  
7. Record the change in `notes/`, argue it in `papers/`, and roll it into `docs/`.

This path keeps every layer synchronized and prevents silent drift.

---

## 5. Change governance

Any non-trivial modification should answer:

- Which **root principle** is being preserved or extended?  
- Which **framework rule** authorizes the change?  
- Which **layers** are directly affected?  
- How is the change represented in:  
  - structure (`architecture/`, `diagrams/`)  
  - behavior (`algorithmic/`, `data/`, `src/`)  
  - expression (`creative/`, `visual/`, `phase/`)  
  - explanation (`notes/`, `papers/`, `docs/`)

If a proposed change cannot be traced along this path, it is not yet coherent and should stay in `notes/` until it is.