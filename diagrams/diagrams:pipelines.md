# Pipelines

This document describes the main pipelines that run through the architecture.

## 1. Ingestion → Coherence → Publication

1. **Ingest**
   - Collect raw material: videos, analytics exports, notes, transcripts.
   - Store under `data/` with clear schemas.

2. **Coherence Pass**
   - Apply framework + algorithmic rules to interpret what the data means.
   - Record decisions and assumptions.

3. **Publication**
   - Export into `creative/` (artifacts, videos, music releases) and `papers/` (formal write-ups).

## 2. Feedback Loop

1. Released artifact generates new signals (views, comments, retention curves).
2. Signals return to `data/` as structured evidence.
3. Algorithmic layer updates profiles, thresholds, and fingerprints.
4. Framework + root only change when long-term patterns demand it.

## Notes

Each pipeline should eventually be mirrored as an actual diagram:
swimlanes, arrows, timestamps, and example instances.
This file defines the canonical steps that any visual representation must respect.