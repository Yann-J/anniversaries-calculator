# anniversaries-calculator

This project is a simple JS solution to compute anniversaries in unusual units (months, hours, minutes...)

## Design

- List of supported units:
  - M, W, H, m, s
- For each unit, compute one or more significant durations
  - Suggestion: the powers of 10 that are around 1Y (e.g. 1 million minutes = 2Y)
- Given a date, for each unit, compute the N (2?) previous and next dates when we hit a round number of significat durations
