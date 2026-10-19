# Problem-Set-1-Econ_3916_PS1
Econ 3916 Problem Set 1

# Econ 3916 PS1: The Cost of Living Brief

A Laspeyres price index for a two-earner household (2019 to 2024), benchmarked against official FRED series and tested for sensitivity to its spending weights.

**Result:** the household's cost of living rose **26.8%** (index 126.76, 2019 = 100). The index is most sensitive to the weight on **Food**, not Rent, even though Rent has the largest weight.

## What's in the notebook

1. **Basket:** six categories in `household_basket`, a Laspeyres index vs an unweighted average (126.76 vs 124.83).
2. **Official series:** seven FRED series rebased to 2019 = 100 and plotted against the household index.
3. **Data audit:** start/end dates, missing months, common sample (starts Jan 1993), and seasonally adjusted vs unadjusted used-car prices.
4. **Sensitivity:** each category's weight swept from 0 to 0.5 with the others rescaled proportionally; AI-assisted, with the transcript and checks in the notebook.

## Sensitivity (index points per +0.01 of weight)

| Category | Weight | Price rise | Effect |
|---|---:|---:|---:|
| Food | 0.158 | 52.7% | +0.31 |
| Recreation | 0.079 | 9.1% | -0.19 |
| Medical | 0.066 | 10.9% | -0.17 |
| Rent | 0.417 | 20.7% | -0.10 |
| Transportation | 0.245 | 30.6% | +0.05 |
| Energy (excl. gas) | 0.035 | 25.0% | -0.02 |

A category matters when its price rise differs from the rest of the basket, not simply when its weight is large.
