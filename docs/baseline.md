# Baseline Decision System

The baseline system represents a conventional autonomy approach using
single-trajectory prediction and fixed thresholds.

## Decision Logic

- CONTINUE if all metrics are within limits
- ABORT if any metric exceeds its threshold

## Metrics Monitored

- Attitude limits
- Altitude loss rate
- Battery voltage
- Actuator saturation

## Limitations

The baseline system does not reason about future uncertainty and only reacts
when thresholds are crossed.