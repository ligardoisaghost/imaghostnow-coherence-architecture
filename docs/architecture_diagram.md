# System Architecture Diagram (Text Form)

## 1. Core Datasets
EL_LIGARDO_DATA_CORE/
   ├── 01_YT_ANALYTICS/
   │      ├── raw_zips/
   │      ├── raw_csv/
   │      └── pipeline/ (normalize, export, dashboards)
   ├── data_raw/
   ├── data_processed/
   ├── public_exports/
   └── reports/

imaghostnow-coherence-architecture/
   ├── architecture/
   ├── core/
   ├── creative/
   ├── diagrams/
   ├── docs/
   │     ├── INDEX_HMR_SYSTEM.md
   │     └── architecture_diagram.md (this file)
   ├── maps/
   ├── notes/
   ├── papers/
   ├── phase/
   ├── phase2_reports/
   └── visual/

HMR_Knowledge_Kit_v1_0/
   ├── Substack_essays/
   ├── Lab_Protocol/
   ├── Gemini_Audit/
   └── Metadata/

---

## 2. Data Flow, Stepwise

1) Export from YouTube Studio  
   – Lifetime analytics CSV/ZIP → saved to raw exports

2) Normalize + ingest  
   – Unzipped into 01_YT_ANALYTICS/raw_zips/raw_csv  
   – Copied into data_raw/ as needed

3) Run Phase-2 pipeline  
   ↳ ./run_phase2_reports.sh  
      ↳ yt_ingestion/pipeline/step_normalize.sh  
           → data_processed/YT_ANALYTICS_NORMALIZED  
      ↳ yt_ingestion/pipeline/run_exports.sh  
           → public_exports/daily_metrics  
           → public_exports/category_metrics  
           → public_exports/search_metrics  
      ↳ yt_ingestion/pipeline/step_dashboards.sh  
           → dashboards/make_markdown_overview.sh  
           → reports/dashboard_YYYYMMDD.md

4) Publish architecture-level views  
   – Commit + push to GitHub repos

---

## 3. Cross-Repository Topology

            ┌──────────────────────────────┐
            │  EL_LIGARDO_DATA_CORE        │
            │  (raw → processed → exports) │
            └───────────────┬──────────────┘
                            │
                            ▼
            ┌──────────────────────────────┐
            │ imaghostnow-coherence-arch   │
            │  (diagrams, maps, pipelines) │
            └───────────────┬──────────────┘
                            │
                            ▼
            ┌──────────────────────────────┐
            │ HMR_Knowledge_Kit_v1_0       │
            │ (narrative, lab protocol)    │
            └──────────────────────────────┘
## 3. Data flow, stepwise

1) Export from YouTube Studio
   – Lifetime analytics CSV/ZIP → saved to raw exports

2) Normalize + ingest
   – Unzipped into 01_YT_ANALYTICS/raw_zips/raw_csv
   – Copied into data_raw/ as needed

3) Run Phase-2 pipeline
   ↳ ./run_phase2_reports.sh
      ↳ yt_ingestion/pipeline/step_normalize.sh
           → data_processed/YT_ANALYTICS_NORMALIZED
      ↳ yt_ingestion/pipeline/run_exports.sh
           → public_exports/daily_metrics
           → public_exports/category_metrics
           → public_exports/search_metrics
      ↳ yt_ingestion/pipeline/step_dashboards.sh
           → dashboards/make_markdown_overview.sh
           → reports/dashboard_YYYYMMDD.md

4) Publish architecture-level views
   – Commit + push to GitHub repos# System Architecture Diagram (Text Form)
