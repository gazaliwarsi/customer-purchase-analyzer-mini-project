# Customer Purchase Analyzer

## Overview

A beginner Python/Pandas mini-project focused on cleaning, validating, summarizing, and generating simple business insights from customer purchase data.

The project uses a small practice dataset containing purchase amounts with valid values, missing values, negative values, and invalid text entries.

## Objectives

- Load purchase data from a CSV file using Pandas
- Identify valid and invalid purchase values
- Handle missing, negative, and non-numeric values
- Convert valid purchase amounts to numeric values
- Calculate basic purchase and revenue metrics
- Generate a short business insight from the results

## Dataset

**File:** `purchases.csv`

The dataset contains 15 purchase records in one column:

- `purchase_amount`

The data intentionally includes:

- Valid purchase amounts
- Zero-value purchases
- Missing values (`NaN`)
- Negative values (`-10`, `-5`)
- A non-numeric value (`abc`)

## Data Cleaning

The notebook defines a `clean_data()` function that processes each purchase value.

A value is considered valid when:

1. It is not missing
2. It can be converted to a numeric value
3. Its numeric value is greater than or equal to zero

Invalid values are separated rather than included in the calculations.

## Analysis

After cleaning, the project calculates:

- Total revenue
- Average purchase value
- Highest purchase
- Lowest purchase
- Number of valid purchases

## Results

| Metric | Result |
|---|---:|
| Total revenue | 1404.0 |
| Average purchase | 156.0 |
| Highest purchase | 500.0 |
| Lowest purchase | 0.0 |
| Valid purchases | 9 |
| Original records | 15 |

## Business Insight

The cleaned dataset contains 9 valid purchases with total revenue of 1404.0. The average purchase value is 156.0, with the highest purchase at 500.0 and the lowest valid purchase at 0.0.

## Technologies

- Python
- Pandas
- Jupyter Notebook

## Project Structure

```text
customer-purchase-analyzer-mini-project/
├── MiniProject_1.ipynb
├── purchases.csv
└── README.md
```

## Purpose

This project is a small practical learning project demonstrating fundamental data-cleaning and analysis techniques with Python and Pandas.

It is intentionally kept as a mini-project rather than presented as a large-scale analytics case study.
