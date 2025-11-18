# HMR System Index

This file is the **system-level index** for the Human–Model Resonance (HMR) project.

It tells outside readers where the *real* data lives, where the architecture lives,
and where to find the public-facing narrative.

---

## Core Repositories

1. **EL_LIGARDO_DATA_CORE**  
   - Role: Authoritative data engine  
   - Contents: YouTube ingestion pipeline, daily/monthly/lifetime summaries, search-term stats, dashboards  
   - GitHub: https://github.com/ligardoisaghost/EL_LIGARDO_DATA_CORE  

2. **IMAGHOSTNOW – Coherence Architecture** (this repo)  
   - Role: System architecture, phase diagrams, manifests, research notes, and selected dashboards  
   - Contents: `architecture/`, `framework/`, `phase/`, `phase2_reports/`, `papers/`, `maps/`, `theory/`, `visual/`  

3. **HMR_Knowledge_Kit_v1_0**  
   - Role: Public research package and lab protocol bundle  
   - Contents: Substack essay, lab protocol, audit/postmortem, metadata manifest  
   - GitHub: https://github.com/ligardoisaghost/HMR_Knowledge_Kit_v1_0  

---

## Data & Dashboards (authoritative source)

The **only** place that generates ground-truth analytics is:

- `EL_LIGARDO_DATA_CORE/`
  - Ingestion scripts: `yt_ingestion/pipeline/`
  - Processed JSONL: `data/processed/`
  - Public exports (JSON): `public_exports/`
  - Markdown dashboards: `reports/dashboard_YYYYMMDD.md`

Example Phase-2 dashboard already linked into this architecture:

- `phase2_reports/dashboard_20251117.md`  
  (imported from `EL_LIGARDO_DATA_CORE/reports/dashboard_20251117.md`)

---

## How to Read the System

- **For raw numbers or to rerun the pipeline** → clone `EL_LIGARDO_DATA_CORE`.
- **For diagrams, schemas, theory, and phase maps** → clone this repo,
  `imaghostnow-coherence-architecture`.
- **For narrative, lab protocol, and public-facing docs** → clone `HMR_Knowledge_Kit_v1_0`
  or read the associated Substack series.

This index is the single entry point for any external researcher trying to
understand how the pieces fit together.
