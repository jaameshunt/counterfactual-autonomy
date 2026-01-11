# Candidate Action Set

The autonomy system evaluates a discrete and intentionally limited set of
high-level actions:

1. CONTINUE  
   Maintain current control commands and flight mode.

2. SLOW  
   Reduce forward velocity and aggressive attitude commands to increase stability.

3. CLIMB  
   Increase altitude to expand safety margins and reduce ground risk.

4. ABORT  
   Transition to a predefined safe recovery state (e.g., hover, loiter, or RTL).

The action space is constrained to preserve explainability and deterministic
behavior.

Only the ABORT action is permitted to directly modify flight mode, ensuring
that the autonomy system cannot force continuation into unsafe states.