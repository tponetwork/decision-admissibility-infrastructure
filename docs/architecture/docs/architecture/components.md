# DAI Architectural Components

Decision Admissibility Infrastructure is composed of several structural components.

Core components:

1. Decision Intake Layer  
Receives proposed decisions from enterprise systems, AI agents, or human operators.

2. Decision Unit Normalization  
Transforms the incoming decision into a standardized Decision Unit (DU).

3. Authority Verification  
Confirms that the actor submitting the decision holds the required authority.

4. Admissibility Engine  
Evaluates the Decision Unit against deterministic admissibility rules.

5. Verdict Engine  
Produces one of three outcomes:
- Admissible
- Conditional
- Inadmissible

6. Execution Gate  
Controls whether the decision can enter execution systems.

7. Governance Ledger  
Maintains an immutable record of decision evaluation and verdicts.
