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

### Cleaned Dataset
`canadian_borrowing_cleaned.csv`

Contains monthly observations for personal loans, credit cards, personal lines of credit, and residential mortgages. Balances are expressed in CAD billions. Additional columns show monthly credit-card growth and a three-month moving average.

### Category Summary

Compares each borrowing category using:
- Starting and latest outstanding balances.
- Absolute balance changes in CAD billions.
- Percentage growth over the observed period.

Categories are ranked by percentage growth to highlight differences in borrowing trends.

### Borrowing Growth Chart

Indexes each category to 100 in the first observed month. This allows growth to be compared across categories with substantially different balance sizes.

### Latest Balances Chart

Compares outstanding balances across the four categories in the latest available month, with values expressed in CAD billions.

### Credit-Card Trend Chart

Displays monthly credit-card balances alongside a three-month moving average, making the overall trend easier to distinguish from short-term fluctuations.

### Notebook Statistics

The notebook also reports:
- Average monthly percentage change in credit-card balances.
- The month with the largest percentage increase.
- The month with the largest percentage decrease.
- The category with the highest percentage growth over the observed period.
  
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
