# Risk and Failure Metrics

Each simulated future trajectory is evaluated using safety-oriented failure metrics.
Metrics are intentionally conservative and bounded.

## Primary Risk Metrics

- Attitude violation:
  Roll or pitch exceeding predefined safety limits.

- Altitude loss:
  Excessive loss of altitude over the simulation horizon.

- Energy collapse:
  Battery voltage or power margin falling below recovery thresholds.

- Actuator saturation:
  Sustained operation near maximum actuator limits.

## Risk Evaluation Strategy

For each candidate action:
- Multiple stochastic rollouts are generated.
- Risk is computed per rollout.
- The worst-case risk across rollouts is retained.

The selected action minimizes worst-case risk rather than expected risk.

If all actions exceed an unsafe risk threshold, the system selects ABORT.
