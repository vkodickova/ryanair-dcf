# Ryanair DCF valuation

Ten-year unlevered DCF of Ryanair (FY26 to FY35). Valuation date 6 March 2026, share price €26.19.
Built by Viktorie Kodickova.

**Base case result: €33.59 per share** (conservative €26.44, optimistic €41.59). The first version of the model gave €30.97.

## Files

| File | Content |
|---|---|
| `Ryanair_DCF_Model_Kodickova_2026.xlsx` | The model. All cells are live formulas. Changed cells are green and the `Changes` sheet lists each change. |
| `Ryanair_DCF_Report_Kodickova_2026.pdf` | Two-page report on the method and results. |

## Changes

1. **Blume adjusted beta:** 1/3 x 1 + 2/3 x raw beta feeds the cost of equity (WACC 8.60% to 8.58%).
2. **Terminal value tied to growth:** terminal FCF = NOPAT FY35 x (1+g) x (1 - g/WACC), so terminal reinvestment is g/WACC of NOPAT (17.5%).
3. **Growth fades to the terminal rate:** from FY27 growth falls in equal steps so FY35 growth equals the terminal growth rate, in all three scenarios.
4. **Reinvestment follows growth:** reinvestment rate = growth / RONIC. RONIC fades from 19.1% in FY26 to WACC in FY35, and CapEx and working capital follow.

## Checking the model

- `Changes` sheet: the four changes, before and after, the step-by-step checkpoints and the known weak points.
- `DCF` sheet: scenario switches in D11:D14, reinvestment in rows 60 to 65, scenario table in rows 87 to 89, sensitivity table in rows 93 to 99.
- `Calc` sheet: the step-by-step valuations and the cash flow paths behind the scenario and sensitivity tables.

## Known weak points

- Tax at 10% against Pillar Two (15% would give about €31.5 per share).
- FY26 FCF is not prorated for the stub period.
- The "Total Debt 10,470" label in the Ratios sheet is actually total liabilities.
- Leases are not added to debt separately.
- The RONIC path (19.1% in FY26 fading to WACC in FY35) is an analyst assumption.

For learning purposes only. Not investment advice.
