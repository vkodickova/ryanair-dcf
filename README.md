# Ryanair DCF valuation

Ten-year unlevered DCF of Ryanair (FY26 to FY35). Valuation date 6 March 2026, share price €26.19.
Built by Viktorie Kodickova.

**Base case result: €31.62 per share** (conservative €24.80, optimistic €39.23). The first version of the model gave €30.97.

## Files

| File | Content |
|---|---|
| `Ryanair_DCF_Model_Kodickova_2026.xlsx` | The model. All cells are live formulas. Changed cells are green and the `Changes` sheet lists each change. |
| `Ryanair_DCF_Report_Kodickova_2026.pdf` | Two-page report on the method and results. |

## Changes

1. **Blume adjusted beta:** 1/3 x 1 + 2/3 x raw beta feeds the cost of equity (WACC 8.58%).
2. **Terminal value tied to growth:** terminal FCF = NOPAT FY35 x (1+g) x (1 - g/WACC), so terminal reinvestment is g/WACC of NOPAT (17.5%).
3. **Growth fades to the terminal rate:** from FY27 growth falls in equal steps so FY35 growth equals the terminal growth rate, in all three scenarios.
4. **Reinvestment follows growth:** reinvestment rate = growth / RONIC. RONIC fades from its FY26 implied level (18.7%) to WACC in FY35, and CapEx and working capital follow.
5. **Tax rate 12%:** the effective tax rate reported in the Q3 FY26 results (previously 10%).
6. **FY26 cash flow prorated:** only the 25 days after the valuation date are counted.
7. **Leases in the equity bridge:** lease liabilities of €111m are deducted together with gross debt.
8. **Ratios label:** "Total Debt" renamed Total Liabilities.

## Checking the model

- `Changes` sheet: the changes, before and after, and the step-by-step checkpoints.
- `DCF` sheet: scenario switches in D11:D14, reinvestment in rows 60 to 65, scenario table in rows 87 to 89, sensitivity table in rows 93 to 99.
- `Calc` sheet: the step-by-step valuations and the cash flow paths behind the scenario and sensitivity tables.

For learning purposes only. Not investment advice.
