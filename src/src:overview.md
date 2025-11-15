# Source Layer Overview

The **src** layer describes how the IMAGHOSTNOW Coherence Architecture is implemented in code.
It is language-agnostic on purpose: this layer explains *how things behave*, not which stack is used.

## Purpose

The src layer:

- Maps conceptual layers (root, framework, algorithmic, data, visual, phase, etc.) to concrete code modules.
- Describes separation of concerns: what belongs in core, what belongs in pipelines, what belongs in utilities.
- Acts as a contract between *architecture* and *whatever language / runtime is currently in use*.

## Structure

- `core/` – Fundamental primitives that everything else depends on.
- `pipelines/` – End-to-end flows that move data, metadata, and decisions through the system.
- `utils/` (optional) – Small helper functions, adapters, glue code that should never contain core logic.

The goal: someone reading this layer should be able to re-implement the system in another language
without touching any of the higher-level documents.

## Notes

The src layer documents *behavior and boundaries*, not implementation details.
If a detail is not stable across languages or runtimes, it does not belong here.

