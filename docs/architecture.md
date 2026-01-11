# System Architecture

The autonomy system operates as a companion computer process.

Sensors → State Estimation → Counterfactual Rollouts → Risk Evaluation → Action Selection

The flight controller retains authority over stabilization and control.
The autonomy system may only trigger a safe abort action.