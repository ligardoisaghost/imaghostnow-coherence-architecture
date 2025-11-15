# Pipelines & Execution Flows

This file documents the executable side of the architecture:
how data, metadata, and decisions move through the system in practice.

## Purpose

Pipelines:

- Connect **data**, **algorithmic**, and **creative** layers into coherent runs.
- Define what “a run” means: ingestion, analysis, generation, publication, or review.
- Encode ordering, retries, fallbacks, and logging requirements.

## Typical Pipelines

Examples (to be refined as the system evolves):

- **Analytics Ingestion Pipeline**
  - Fetch metrics from external platforms.
  - Normalize into canonical data schemas.
  - Persist snapshots and compute deltas.

- **Shorts Decision Pipeline**
  - Read current phase + state.
  - Evaluate metrics against thresholds.
  - Emit recommended actions (drop, delay, retire, escalate).

- **Creative Feedback Pipeline**
  - Ingest human notes, annotations, and external expert feedback.
  - Attach them to assets as structured metadata.
  - Update state machines and research agenda entries.

## Guarantees

Every pipeline must specify:

- Inputs and outputs (by schema, not by implementation detail).
- Failure modes and what “safe failure” looks like.
- Which layers it touches and which invariants it must preserve.

## Notes

The pipelines described here are *executable narratives*:
they should be clear enough that an engineer can implement them
without reading internal chat logs or external notes.

