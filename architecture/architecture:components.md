architecture/components.md

This file itemizes all components, from signal detectors to pattern classifiers to state evaluators. Each component has a role that cannot be duplicated elsewhere without destabilizing clarity. Components interface through strict contracts and shared invariants. The description identifies failure points and how each piece compensates for others. This ensures the architecture remains modular and self-diagnosing.
