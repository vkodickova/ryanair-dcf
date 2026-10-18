# Ryanair DCF valuation

Ten-year unlevered DCF of Ryanair (FY26 to FY35). Valuation date 6 March 2026, share price €26.19.
Built by Viktorie Kodickova.

**Base case result: €31.62 per share** (conservative €24.80, optimistic €39.23).

## Files

| File | Content |
|---|---|
| `Ryanair_DCF_Model_Kodickova_2026.xlsx` | The model. All cells are live formulas. |
| `Ryanair_DCF_Report_Kodickova_2026.pdf` | Two-page report on the method and results. |

## Method

1. **Cost of equity** uses a Blume adjusted beta, 1/3 x 1 + 2/3 x raw beta (WACC 8.58%).
2. **Revenue growth** starts at the scenario rate in FY26 and falls in equal steps to the terminal growth rate in FY35.
3. **Reinvestment** follows growth. Reinvestment rate = growth / RONIC, with RONIC fading from its FY26 implied level (18.7%) to WACC in FY35. CapEx and working capital follow.
4. **Terminal value** uses terminal FCF = NOPAT FY35 x (1+g) x (1 - g/WACC), so terminal reinvestment equals g/WACC of NOPAT (17.5%).
5. **Inputs** include a 12% tax rate and lease liabilities of €111m deducted with gross debt (Q3 FY26 results). FY26 cash flow counts only the 25 days after the valuation date.

## Using the model

- `DCF` sheet: scenario switches in D11:D14, reinvestment in rows 60 to 65, scenario table in rows 87 to 89, sensitivity table in rows 93 to 99.
- `Calc` sheet: the cash flow paths behind the scenario table and the sensitivity table.
- `Notes` sheet: method summary.

For learning purposes only. Not investment advice.
