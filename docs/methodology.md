# Methodology

At each decision cycle, the autonomy system performs the following steps:

1. Ingest the current estimated system state.
2. Generate multiple stochastic future rollouts for each candidate action.
3. Inject uncertainty into dynamics and disturbances.
4. Evaluate safety metrics for each rollout.
5. Aggregate results using worst-case risk.
6. Select the action minimizing worst-case risk.

The process is repeated at a fixed real-time rate (e.g., 10 Hz).

This approach prioritizes robustness to uncertainty and early detection of
unsafe commitments.
