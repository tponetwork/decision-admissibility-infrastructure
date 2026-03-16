# Decision Unit (DU)

The Decision Unit (DU) is the atomic governance object evaluated by the
Decision Admissibility Infrastructure (DAI).

Every proposed action entering the system must be represented as a
Decision Unit before evaluation.

## Minimum Fields

decision_id  
Unique identifier of the decision.

actor_identity  
The entity requesting execution (human, system, or AI agent).

authority_context  
Proof of authority for the actor submitting the decision.

jurisdiction_context  
Operational and regulatory context in which the decision operates.

risk_class  
Classification of the decision impact (low, moderate, high, critical).

execution_target  
The system or infrastructure where execution would occur.

evidence_links  
References supporting the decision (documents, models, analysis).

timestamp  
Time at which the decision was submitted.

## Cryptographic Anchor

Each Decision Unit produces a deterministic hash:

DU_HASH = HASH(decision_payload)

The hash acts as the canonical reference for evaluation,
audit logging, and consensus replication.

## Governance Invariant

A Decision Unit missing required fields is automatically:

INADMISSIBLE
