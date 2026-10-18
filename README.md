# Ryanair DCF valuation

Ten-year unlevered DCF of Ryanair (FY26 to FY35). Valuation date 6 March 2026, share price €26.19.
Built by Viktorie Kodickova.

**Base case result: €31.41 per share** (conservative €23.67, optimistic €40.04).

## Files

| File | Content |
|---|---|
| `Ryanair_DCF_Model_Kodickova_2026.xlsx` | The model. All cells are live formulas. |
| `Ryanair_DCF_Report_Kodickova_2026.pdf` | Two-page report on the method and results. |

## Method

1. **Cost of equity** uses a Blume adjusted beta: 1/3 x 1 + 2/3 x raw beta (WACC 8.58%).
2. **Revenue growth** starts at the scenario rate in FY26 and falls in equal steps to the terminal growth rate in FY35.
3. **Terminal value** uses terminal FCF = NOPAT FY35 x (1+g) x (1 - g/WACC), so terminal reinvestment equals g/WACC of NOPAT (17.5%).

## Checking the model

- `DCF` sheet: scenario switches in D11:D14, scenario table in rows 87 to 89, sensitivity table in rows 93 to 99.
- `Calc` sheet: the cash flow paths behind the scenario table and the sensitivity table.
- `Notes` sheet: method summary and known weak points.

## Known weak points

- Tax at 10% against Pillar Two (15% would give about €29 per share).
- FY26 FCF is not prorated for the stub period.
- The "Total Debt 10,470" label in the Ratios sheet is actually total liabilities.
- Leases are not added to debt separately.
- CapEx, D&A and working capital stay fixed percentages of sales through the growth fade.

For learning purposes only. Not investment advice.
