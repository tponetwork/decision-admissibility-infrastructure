## Architecture

Decision Admissibility Infrastructure (DAI) introduces a structural control layer that governs whether a proposed decision may enter execution.

Instead of evaluating actions after they occur, DAI evaluates the admissibility of a decision before it can mutate operational systems.

Every decision is normalized into a Decision Unit (DU) and evaluated against governance constraints derived from institutional authority.

The evaluation produces one of three possible verdicts:

- **Admissible** — the decision may proceed through the Execution Gate into operational systems.
- **Conditional** — additional authority or escalation is required before execution.
- **Inadmissible** — the decision is structurally blocked from execution.

All evaluated decisions produce an **Audit Record**, enabling governance review and traceability of decision flows across enterprise systems.
