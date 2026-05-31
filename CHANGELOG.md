# Changelog

All notable changes to this Power BI report are documented here.

---

## [1.1.0] — 2026-05-31

### Changed
- Rewrote `README.md` **Business Insights** as 7 named analytical sections, each
  with a bold lead finding, supporting data point, and 3 strategic implications:
  - The Mid-Tier Monopoly · The Week 53 Surge · The Gender Revenue Gap ·
    The Coastal Concentration Risk · The Activation Ceiling ·
    The Delinquency Signal · The Interest Income Engine

### Added
- `README.md` **Architecture** section with a CSV → Power BI → Dashboard → Exports data-flow diagram
- `README.md` **Executive Summary** synthesizing portfolio-level findings and strategic priorities

---

## [1.0.0] — 2024-12-31

### Added
- Initial report release: `Credit_Card_Report.pbix`
- Week 53 (31st Dec) dashboard with Week-over-Week change metrics
  - Revenue: +28.8% WoW
  - Transaction Amount & Count: tracked WoW
  - Customer Count: tracked WoW
- YTD Summary KPIs:
  - Overall Revenue: $57M
  - Total Interest: $8M
  - Total Transaction Amount: $46M
  - Male Revenue: $31M / Female Revenue: $26M
  - Blue & Silver card share: 93% of transactions
  - TX + NY + CA revenue share: 68%
  - Activation Rate: 57.5%
  - Delinquent Rate: 6.06%
- Full project folder structure initialized:
  `data/`, `docs/screenshots/`, `exports/`, `sql/`, `dax/`
- `.gitignore` for Power BI, credentials, OS junk, temp files
- `README.md` with full KPI documentation and business insights
- `docs/dax_measures.md` with core DAX formulas
- `data/README.md` with data source documentation
- Source data: `credit_card.csv`, `customer.csv`, `cc_add.csv`, `cust_add.csv`
- Exported snapshots: `Credit_Card_Customer_Report.pdf`, `Credit_Card_Transaction_Report.pdf`
