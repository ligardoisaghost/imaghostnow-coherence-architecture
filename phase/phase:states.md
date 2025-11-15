# System States

States describe stable configurations of the architecture under different
operational conditions.

## Core States
- **Dormant** — Minimal activity, system awaits trigger conditions.
- **Active** — Normal operational mode, all subsystems responsive.
- **Accelerated** — High-intensity mode. Fewer constraints. Faster iteration.
- **Restricted** — Safety-limited mode. Reduced privileges. Guardrails active.
- **Transitional** — Moving between states; partial subsystem activation.

## Transition Rules
- Transitions must be monotonic in a single direction unless explicitly defined.
- No state may bypass “Transitional” unless allowed by invariants.
- States inherit global constraints from root/principles.md.

## Notes
A state shift is a global event: every subsystem adjusts its behavior.
