
# stock-tools
A tool that will munge basic stock activity (buy/sells) via CSV.

## Goals
- Wash Sales
- Capital gains/losses


## CSV Input Example

Ideally, each security will have been aggregated and will have its own detail similar to this:

**Partial Apex Clearing sample:**
| Symbol | Net Amt. | Trade Action | Trade Date |
|--|--|--|--|
| GOOGL | -1000.08 | Buy | 2020-03-01
| GOOGL | 1000.52 | Sell | 2020-03-18
| FB | -20.00 | Buy | 2020-03-01
| FB | 19.23 | Sell | 2020-03-18

## Output Example

Ideally, each security will have been aggregated and will have its own detail similar to this:

| Symbol | Gain/Loss | Wash Sale Loss | 
|--|--|--|
| GOOGL | 0.44 | 0 |
| FB | -0.77 | -0.77 |
