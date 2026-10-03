# Canadian Consumer Borrowing Analysis

A Python project examining Canadian consumer borrowing trends using monthly Bank of Canada data.

The analysis compares outstanding balances across personal loans, credit cards, personal lines of credit, and residential mortgages.

## Project Objectives

- Compare percentage growth across borrowing categories.
- Examine changes in outstanding balances over time.
- Identify the largest monthly increases and decreases in credit-card balances.
- Use a three-month moving average to examine credit-card trends.

## Tools Used

- **Pandas:** Data cleaning, validation, and analysis.
- **NumPy:** Numerical calculations.
- **Matplotlib:** Charts and trend visualization.

## Dataset

**Source:** Bank of Canada — Chartered Bank Selected Assets, Month-End.

[View the official data source](https://www.bankofcanada.ca/rates/banking-and-financial-statistics/chartered-bank-selected-assets-month-end-formerly-c1/)

**Requested period:** October 2023 to September 2026. Actual coverage reflects the published observations available when the notebook was run.

**Frequency:** Monthly.

Balances were converted from CAD millions to CAD billions.

## Analysis Process

1. Loaded the source data directly into Python.
2. Converted dates and balances into appropriate data types.
3. Checked for missing values, duplicate observations, and missing months.
4. Calculated absolute balance changes and percentage growth.
5. Indexed each borrowing category to 100 to compare growth.
6. Analysed monthly credit-card changes and a three-month moving average.
7. Exported cleaned data, summary results, and charts.

## Outputs

- A cleaned monthly borrowing dataset.
- A summary comparing starting and latest balances.
- Growth comparisons across four borrowing categories.
- Credit-card monthly growth statistics.
- Three charts available in the project files.

## How to Run

Open `notebooks/canadian_consumer_borrowing.ipynb` in Google Colab and run the cells in order.

The notebook downloads data directly from the Bank of Canada. Published revisions may change the results in future runs.

## Limitations

- The data represents aggregate chartered-bank balances, not individual banks or customers.
- Outstanding balances measure debt at a point in time, not new monthly borrowing.
- The selected categories do not represent all Canadian bank lending.
- Values are not adjusted for inflation.
- The analysis identifies trends but does not establish their causes.

## Author

Sri Kovirineni
