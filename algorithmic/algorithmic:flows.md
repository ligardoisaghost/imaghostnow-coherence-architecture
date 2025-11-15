# Algorithmic Flows

This file describes system motion through time and state.

## State Machine

**States**
- INPUT
- EVALUATE
- RECONCILE
- UPDATE
- STABILIZE

**Transitions**
INPUT → EVALUATE  
EVALUATE → RECONCILE  
RECONCILE → UPDATE  
UPDATE → STABILIZE  
STABILIZE → INPUT

## Evaluation Cycle
1. Capture signal  
2. Anchor temporally  
3. Compare against invariants  
4. Apply logic  
5. Update coherence layer  
6. Store result

## Notes
Flows define *rhythm*. Logic defines *rules*. Together they form the living behavior of the architecture.