# Data Schemas

These schemas define the shapes and constraints of core data objects inside the IMAGHOSTNOW architecture.

## Principles
- Every object must be explicit.
- No silent mutation.
- Format must be deterministic.

## Base Schemas
### **Document**
- id: string
- title: string
- layer: string
- created_at: timestamp
- updated_at: timestamp
- body: markdown

### **Event**
- id: string
- type: string
- payload: object
- timestamp: timestamp

## Notes
Schemas are living structures but must never break existing logic.