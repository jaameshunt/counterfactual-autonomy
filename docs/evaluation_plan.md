# Evaluation Plan

The system will be evaluated using the following criteria:

- Decision latency:
  Ability to maintain fixed update rate under computational load.

- Abort timing:
  Time difference between counterfactual abort and baseline rule-based abort.

- Failure avoidance:
  Reduction in late-stage unsafe conditions.

- Explainability:
  Ability to trace decisions to specific risk metrics.

Evaluation will be conducted using:
- Simulated telemetry
- Log replay
- Controlled flight tests (future work)
