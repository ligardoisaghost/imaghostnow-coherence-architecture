# Core Modules

The **core** modules represent the smallest set of primitives that must exist
for the IMAGHOSTNOW Coherence Architecture to function.

## Responsibilities

Core modules must:

- Encode the global invariants defined in the **root** and **framework** layers.
- Provide stable types / data structures that higher layers can rely on.
- Expose minimal, explicit interfaces instead of leaking internal details.

Examples of core responsibilities:

- Canonical representation of:
  - tracks / works / aliases
  - shorts / videos / visual assets
  - metrics, events, analytic snapshots
- Core state machine(s) that track phase, states, and transitions.
- Base error / anomaly types used by all higher-level modules.

## Constraints

- Core code must not depend on visualization, UI, or external services directly.
- Any integration with outside systems is handled via adapters or pipelines.
- Changes to core modules require justification against the **root/principles** file.

## Notes

If a change here breaks more than one layer at once, that is expected:
core is allowed to *radiate* impact, but changes must be rare and deliberate.