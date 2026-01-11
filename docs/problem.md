# Problem Statement

Modern autonomous aerial systems make control decisions based on a single predicted
future derived from uncertain state estimates and imperfect models. When this
prediction is incorrect, the system often commits to unsafe actions and fails
abruptly rather than degrading gracefully.

This limitation is particularly acute in small unmanned aircraft operating under
uncertainty, where sensing, environmental disturbances, and energy constraints
can change rapidly and unpredictably.

The absence of onboard reasoning about multiple plausible futures leads to
overconfident decision-making and delayed recovery actions.

## Research Question

Can an autonomous aerial system improve safety and robustness by evaluating
multiple plausible future trajectories in real time and selecting actions based
on worst-case outcome minimization rather than nominal optimality?

## Scope

This research focuses on:
- Short-horizon (2–3 s) onboard decision-making
- Real-time operation under uncertainty
- Safety-driven action selection rather than performance optimization

The system does not attempt full path planning or mission optimization.