# 3-Statement Financial Model

An integrated Excel financial modelling project connecting the **Income Statement, Balance Sheet, and Cash Flow Statement** with scenario analysis, five-year forecasting, financial ratios, monthly budgeting, variance analysis, and management insights.

The model is designed to demonstrate practical **FP&A, financial modelling, accounting, forecasting, and management reporting** skills.

---

## Executive Summary

![Executive Summary](./Finance%20Model-Forecast-Excel/Screenshots/executive.png)

The model starts with a 2026 actual/base year and forecasts financial performance through **2031E**.

Key outputs include:

* Revenue and Net Income growth
* EBITDA and Net Margin development
* Cash generation
* Liquidity and leverage ratios
* Working capital performance
* Base / Upside / Downside scenario comparison
* Actual vs Budget variance analysis

---

## Project Objectives

The main objective of this project was to build a fully linked financial model where changes in operating assumptions automatically flow through all three financial statements.

The model allows users to evaluate how changes in:

* Revenue growth
* COGS
* Operating expenses
* Depreciation
* Tax rates
* Interest rates
* Accounts Receivable days
* Inventory days
* Accounts Payable days
* Capital expenditure

affect profitability, working capital, cash flow, and the balance sheet.

---

## Model Architecture

```text
Assumptions
    ↓
Income Statement
    ↓
Balance Sheet ↔ Cash Flow Statement
    ↓
Ratios & KPIs
    ↓
Executive Summary
    ↓
Monthly Forecast
    ↓
Actual vs Budget vs Forecast
    ↓
Insights & Recommendations
```

The model includes automated integrity checks to ensure that:

```text
Assets = Liabilities + Equity
```

and:

```text
Cash Flow Ending Cash = Balance Sheet Cash
```

---

## Scenario Analysis

![Assumptions](screenshots/assumptions.png)

The model includes three operating scenarios:

* **Base**
* **Upside**
* **Downside**

A scenario selector automatically updates the active financial assumptions used throughout the model.

Scenario drivers include:

* Revenue growth
* COGS as % of Revenue
* Opex as % of Revenue
* Depreciation as % of Revenue
* Tax rate
* Interest rate
* DSO
* DIO
* DPO
* CapEx

This allows the model to be used for sensitivity analysis and financial planning.

---

## Income Statement

![Income Statement](screenshots/incomestatement.png)

The Income Statement forecasts:

* Revenue
* COGS
* Gross Profit
* Operating Expenses
* EBITDA
* Depreciation
* EBIT
* Interest Expense
* EBT
* Tax
* Net Income

Forecast period:

**2026A → 2031E**

The forecast is driven directly by assumptions selected in the scenario engine.

---

## Balance Sheet

![Balance Sheet](screenshots/balancesheet.png)

The Balance Sheet includes:

### Current Assets

* Cash
* Accounts Receivable
* Inventory

### Non-Current Assets

* Net PP&E

### Liabilities

* Accounts Payable
* Current Portion of Debt
* Long-Term Debt

### Equity

Equity is updated using retained earnings generated from forecast Net Income.

Working capital balances are calculated using operational drivers such as **DSO, DIO, and DPO**.

---

## Cash Flow Statement

![Cash Flow Statement](screenshots/cashflow.png)

The Cash Flow Statement is linked directly to the Income Statement and Balance Sheet.

It includes:

### Operating Cash Flow

* Net Income
* Depreciation
* Changes in Accounts Receivable
* Changes in Inventory
* Changes in Accounts Payable

### Investing Cash Flow

* Capital Expenditure

### Financing Cash Flow

The current version assumes a constant debt balance with no additional borrowing or repayment.

Ending cash automatically flows back into the Balance Sheet.

---

## Financial Ratios & KPIs

![Financial Ratios & KPIs](screenshots/ratio.png)

The model calculates key financial metrics including:

* Revenue Growth %
* Gross Margin %
* EBITDA Margin %
* Net Margin %
* Current Ratio
* Debt / Equity
* Days Sales Outstanding
* Days Inventory Outstanding
* Days Payable Outstanding

The sheet also includes automated model integrity checks.

---

## Monthly Forecast

![Monthly Forecast](screenshots/monthly.png)

The annual 2027 Base Budget is converted into a 12-month operating forecast.

The monthly model includes:

* Revenue
* COGS
* Gross Profit
* Opex
* EBITDA
* Depreciation
* EBIT
* Interest Expense
* EBT
* Tax
* Net Income

The monthly totals are automatically reconciled against the annual budget.

---

## Actual vs Budget vs Latest Estimate

![Actual vs Budget vs Forecast](screenshots/actualbudget.png)
This section adds an FP&A-style performance monitoring layer.

Users can enter actual monthly results for:

* Revenue
* COGS
* Opex

The model then automatically calculates:

* Gross Profit
* EBITDA
* Net Income
* Variance $
* Variance %
* Latest Estimate

The **Latest Estimate** combines actual results from closed months with remaining budget values for future months.

This provides a simple rolling forecast / latest-estimate framework commonly used in FP&A reporting.

---

## Insights & Recommendations

The workbook also contains an automated **Insights & Recommendations** section.

The analysis dynamically evaluates:

* Revenue growth
* Net Income growth
* Margin development
* Debt / Equity
* Current Ratio
* Cash accumulation
* Scenario sensitivity

The output updates automatically when assumptions or scenarios are changed.

---

## Model Integrity

The model includes two important automated controls:

### Balance Sheet Check

```text
Total Assets - Total Liabilities & Equity = 0
```

### Cash Reconciliation

```text
Balance Sheet Cash - Cash Flow Ending Cash = 0
```

These controls help identify broken links or modelling errors.

---

## Excel Modelling Conventions

The workbook uses consistent modelling conventions:

* **Blue cells** — manual inputs
* **Yellow cells** — key active assumptions
* **Green cells** — links to other worksheets
* Formula-driven forecast outputs
* Separate Actual and Estimate periods
* Centralised assumption management
* Automated reconciliation checks

---

## Skills Demonstrated

This project demonstrates practical experience in:

* Financial Modelling
* FP&A
* Financial Statement Analysis
* Forecasting
* Budgeting
* Scenario Analysis
* Variance Analysis
* Working Capital Analysis
* Financial Ratio Analysis
* Cash Flow Forecasting
* Management Reporting
* Excel Formula Modelling
* Accounting Logic

---

## Workbook Structure

```text
3-Statement-Financial-Model.xlsx

├── Executive Summary
├── Assumptions
├── Income Statement
├── Balance Sheet
├── Cash Flow Statement
├── Ratios & KPIs
├── Monthly Forecast
├── Actual vs Budget vs Forecast
└── Insights & Recommendations
```

---

## Tools Used

**Microsoft Excel**

Key Excel functionality used includes:

* Cross-sheet formulas
* INDEX / MATCH
* IF logic
* Scenario-driven assumptions
* Financial ratios
* Forecast calculations
* Variance calculations
* Automated reconciliation checks
* Charts and management reporting

---

## File

The complete model is available in this repository:

**`3-Statement-Financial-Model.xlsx`**

---

## Disclaimer

This project was created for **portfolio and educational purposes**.

The financial figures and assumptions are illustrative and do not represent the financial statements of a real company.

---

## Author

**Maxim Irinov**

Data Analyst | Financial Analyst | Accounting & Business Intelligence

Interested in combining **financial analysis, accounting, data analytics, and automation** to support better business decision-making.
