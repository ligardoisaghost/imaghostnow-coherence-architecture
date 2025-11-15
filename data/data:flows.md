# Data Flows

This file defines how information moves through the architecture.

## Principles
- Flow must be traceable.
- No orphan data.
- Every transformation must leave a timestamped footprint.

## Flow Types
### Ingestion Flow
Raw → validated → structured → stored

### Retrieval Flow
User/module → fetch → normalize → output

### Transformation Flow
input → process → validate → persist

## Notes
Breaking the data flow rules destabilizes the coherence architecture.