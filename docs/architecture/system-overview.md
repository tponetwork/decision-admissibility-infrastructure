# System Overview

Decision Admissibility Infrastructure (DAI) defines a structural governance
layer that determines whether a decision may enter the execution path.

The system operates before execution and enforces a fail-closed control boundary.

Core flow:

Human Authority
↓
Decision Proposal
↓
Decision Intake
↓
Decision Unit Normalization
↓
Authority Verification
↓
Admissibility Engine
↓
Verdict

Possible outcomes:

Admissible → Execution Gate → Enterprise Systems → Action

Conditional → Escalation / Additional Authorization

Inadmissible → Execution Block
