# Multi-Entity Financial Variance & FP&A Pipeline

## Overview
This project builds an automated financial tracking system in Python and DuckDB to evaluate multi-entity business performance against planned budgets. By joining raw general ledger entries with chart-of-accounts metadata and budget targets, the pipeline calculates revenue, COGS, operating expenses, and net margins across operating sites.

## Data Source
The raw financial dataset (`Chart of Accounts.xlsx`, `Income Statement.xlsx`, `Budget.xlsx`) was sourced from the **[Finance Data Sample of Furniture Company](https://www.kaggle.com/datasets/zhoumeixing/finance-data-sample-of-furniture-company)** dataset by Zhoumeixing on Kaggle to simulate multi-entity operational accounting and general ledger transactions for FP&A modeling.

## Features
- **Consolidated P&L Analysis:** Modeled full-year financial actuals across 6 operating entities.
- **Budget vs. Actuals (BvA) Tracking:** Built SQL CTE queries to track monthly spending variances ($ and %).
- **Cost Overrun Alerts:** Automated variance logic to flag operational cost overruns exceeding 15% above budget.

## Tech Stack
- **Language:** Python
- **Database Engine:** DuckDB (In-Memory SQL)
- **Data Manipulation:** Pandas
- **Environment:** Jupyter Notebook / Anaconda
