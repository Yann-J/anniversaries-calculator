# anniversaries-calculator

This project is a simple JS solution to compute anniversaries in unusual units (months, hours, minutes...)

## Usage

The tool is available directly from this repo's [Github Pages](https://yann-j.github.io/anniversaries-calculator).

## Design

- List of supported units:
  - months, weeks, days, hours, minutes, seconds
- For each unit, we compute a significant duration
  - This is computed as the power of 10 that is immediately above 1 year (e.g. 1 million minutes = ~2Y)
- Given a date, for each unit, we compute the N (=2) previous and next dates when we hit a round number of significant durations
  - E.g. if your current age is 32,765,769 minutes, we display the dates for your 31, 32, 33, 34 million minutes anniversaries
