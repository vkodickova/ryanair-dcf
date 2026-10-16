# Ryanair DCF valuation (v2)

Ten-year unlevered DCF of Ryanair (FY26 to FY35). Valuation date 6 March 2026, share price €26.19.
Built by Viktorie Kodickova and updated in October 2026 after interview feedback.

**Base case result: €31.41 per share** (original model €30.97).

## Files

| File | Content |
|---|---|
| `Ryanair_DCF_Valuation_Kodickova_2026_v2.xlsx` | The model. All cells are live formulas. |
| `Ryanair_DCF_Update_Report_Kodickova_2026.pdf` | Two-page report on what changed, how and why. |

## What changed in v2

1. **Blume adjusted beta.** Adjusted beta = 1/3 x 1 + 2/3 x raw beta feeds the cost of equity (WACC 8.60% to 8.58%).
2. **Terminal FCF tied to growth.** Terminal FCF = NOPAT FY35 x (1+g) x (1 - g/WACC), so terminal reinvestment falls from about 47% to 17.5% of NOPAT.
3. **Growth fades to the terminal rate.** From FY27 growth falls in equal steps so FY35 growth equals the terminal growth rate, in all three scenarios.

Correcting the terminal year alone would give about €41 per share. The growth fade brings the value back to about €31.

## Checking the model

- `Changes` sheet: before and after table and the reconciliation of each step against my own replication (tolerance €0.30).
- `DCF` sheet: scenario switches in D11:D14, scenario table in rows 87 to 89, sensitivity table in rows 93 to 99.
- `Calc` sheet: the step-by-step valuations behind the reconciliation, the scenario table and the sensitivity table.

## Known weak points

- Tax at 10% against Pillar Two (15% would give about €28 per share on the original model and about €29 on v2).
- FY26 FCF is not prorated for the stub period.
- The "Total Debt 10,470" label in the Ratios sheet is actually total liabilities.
- Leases are not added to debt separately.
- CapEx, D&A and working capital stay fixed percentages of sales through the fade.

For learning purposes only. Not investment advice.
