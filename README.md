
# investor-tools
A tool that will munge basic stock activity (buy/sells) with the input (as CSV). Most brokerage apps should already let you export your activity via CSV.

## Goals
- [Wash Sales](https://www.investopedia.com/terms/w/washsalerule.asp)
- Capital gains/losses after selling a share or all shares of a stock
  - All shares (current data below shows this scenario)
  - Partial sells (long-term goal)


## CSV Input Example

Ideally, each input CSV will have its own detail similar to this:

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

## Stargazers over time

[![Stargazers over time](https://starchart.cc/MrGavintech/investor-tools.svg)](https://starchart.cc/MrGavintech/investor-tools)
