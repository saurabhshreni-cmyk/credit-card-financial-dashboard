# /data — Source Data Files

This folder is reserved for organized source data used by the Power BI report.
The current source CSVs live in the repo root (so the existing `.pbix` data-source
links keep working); move them here only if you also re-point the queries.

## File Descriptions

| Filename              | Description                                           |
|-----------------------|-------------------------------------------------------|
| `credit_card.csv`     | Transaction-level data: amount, category, card type   |
| `customer.csv`        | Customer demographics: gender, job, income, state     |
| `cc_add.csv`          | Additional credit card metadata                       |
| `cust_add.csv`        | Additional customer address/location data             |

## Notes

- Do NOT commit files containing real PII, API keys, or connection strings.
  Add them to `.gitignore` before staging.
- Preferred formats: `.csv` (UTF-8), `.xlsx`
- After cloning, update Power BI data source paths:
  **Home → Transform Data → Data Source Settings → Change Source**
  and point to the CSV files.
