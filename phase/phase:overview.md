# Phase Overview

The phase layer defines how the IMAGHOSTNOW Coherence Architecture behaves across
time, cycles, and operational stages. Each phase modifies system priorities,
constraints, and active subsystems.

## Purpose
Phases allow the architecture to shift behavior without breaking coherence.
They define temporal logic: what changes, what stabilizes, and what rules apply.

## Contents
- **overview.md** — This file. High-level description of the phase layer.
- **states.md** — Defines system states and transitions.
- **cycles.md** — Defines temporal cycles, loops, and progression rules.

## Notes
Phases must be consistent with the root and framework layers.  
No phase may contradict global invariants.
