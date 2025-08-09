# Sandea Operations Analytics – Cleaned Data & Dashboard

This bundle includes:
- **Cleaned Excel files** (empty rows/columns removed, column names standardized).
- **Unified analytics Excel**: `Sandea_analytics_dashboard.xlsx` with:
  - `transactions_sample` (first 2,000 rows of relevant fields)
  - `kpis` (revenue by month, top customers/products, revenue by region – if present in source)
  - `data_dictionary` mapping original → standardized columns
  - `dashboard` sheet showing embedded charts

## What I cleaned
- Removed fully empty rows/columns
- Standardized column names to lowercase with underscores
- Computed a `__revenue` metric from amount or quantity × price when available

## How to use
- Upload the cleaned files and the dashboard Excel to your GitHub repo (e.g., `sandea-operations-analytics/data/` and `.../reports/`).
- Open `Sandea_analytics_dashboard.xlsx` → **dashboard** tab for the charts.
- Use `kpis` and `transactions_sample` for further analysis.

## Notes
- Only relevant columns are kept (date, customer, product, qty, price, amount, region, computed revenue) when detected.
- Some source files may not include all fields; charts will appear only for available metrics.