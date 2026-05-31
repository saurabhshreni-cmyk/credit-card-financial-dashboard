# 📊 Credit Card Financial Dashboard

> Interactive Power BI dashboard analyzing credit card transactions, customer
> demographics, revenue trends, expenditure patterns, and financial KPIs.

[![Power BI](https://img.shields.io/badge/Built%20with-Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![GitHub](https://img.shields.io/badge/GitHub-saurabhshreni--cmyk-181717?style=flat&logo=github)](https://github.com/saurabhshreni-cmyk)

---

## 🔍 Project Overview

This Power BI report delivers a two-page financial intelligence dashboard tracking
credit card portfolio performance across revenue, transactions, customer demographics,
and risk indicators — reported weekly (Week-over-Week) and cumulatively (Year-to-Date).

The dashboard enables business stakeholders to monitor KPIs, identify revenue drivers,
and surface actionable patterns across card tiers, geography, and customer segments.

---

## 📁 Folder Structure

```
credit-card-financial-dashboard/
│
├── Credit_Card_Report.pbix          ← Main Power BI report (open in Power BI Desktop)
│
├── credit_card.csv                  ← Transaction-level source data
├── customer.csv                     ← Customer demographics source data
├── cc_add.csv                       ← Additional credit card metadata
├── cust_add.csv                     ← Additional customer address data
│
├── Credit_Card_Customer_Report.pdf  ← Exported customer report snapshot
├── Credit_Card_Transaction_Report.pdf ← Exported transaction report snapshot
│
├── data/                            ← Reserved for organized source data
│   └── README.md
│
├── docs/                            ← Documentation and reference
│   ├── screenshots/                 ← Dashboard preview images
│   └── dax_measures.md              ← All custom DAX measures documented
│
├── exports/                         ← Exported PDF/PNG snapshots of report pages
├── sql/                             ← SQL scripts (for DB-connected versions)
├── dax/                             ← Standalone .dax query files
│
├── CHANGELOG.md                     ← Report version history
├── .gitignore                       ← Excludes credentials, OS junk, temp files
└── README.md                        ← You are here
```

---

## 📈 Dashboard Insights — Week 53 (31st Dec)

### Week-over-Week Change

| Metric                   | Change      |
|--------------------------|-------------|
| Revenue                  | ▲ +28.8%    |
| Total Transaction Amount | ▲ tracked   |
| Total Transaction Count  | ▲ tracked   |
| Customer Count           | ▲ tracked   |

---

### Year-to-Date (YTD) Summary

| Metric                              | Value              |
|-------------------------------------|--------------------|
| Overall Revenue                     | **$57M**           |
| Total Interest Earned               | **$8M**            |
| Total Transaction Amount            | **$46M**           |
| Male Customer Revenue               | **$31M**           |
| Female Customer Revenue             | **$26M**           |
| Blue & Silver Card Transaction Share| **93%**            |
| TX + NY + CA Revenue Share          | **68%**            |
| Overall Activation Rate             | **57.5%**          |
| Overall Delinquent Rate             | **6.06%**          |

---

## 💡 Business Insights

### 1. 📌 Card Tier Concentration
Blue and Silver credit card tiers drive **93% of all transactions**, confirming
that mid-tier products — not premium cards — are the portfolio's primary revenue engine.
Premium tier cards contribute minimal transaction volume relative to their positioning.

### 2. 👥 Gender Revenue Split
Male customers contribute **$31M** vs female customers at **$26M** in overall revenue.
This $5M gap and its week-on-week movement is a key segment-level KPI tracked in the dashboard.

### 3. 🗺️ Regional Revenue Concentration
Texas, New York, and California combined account for **68% of total revenue**.
This geographic concentration highlights both a dependency risk and an expansion
opportunity in underrepresented states.

### 4. ⚡ Activation vs Delinquency Balance
- **Activation Rate: 57.5%** — significant headroom to convert issued cards into
  active, revenue-generating accounts through targeted engagement campaigns.
- **Delinquent Rate: 6.06%** — a critical credit risk KPI for portfolio health monitoring.

### 5. 📅 Week 53 Revenue Spike (+28.8% WoW)
A near-30% week-on-week revenue surge in the final week of December is consistent
with year-end seasonal spending behavior. Forecasting models should factor in
Q4 / holiday-driven volatility as a structural pattern.

### 6. 💳 Interest-to-Revenue Ratio
With $8M interest earned on $57M revenue, interest income represents ~14% of
total revenue — indicating a meaningful contribution from revolving credit balances.

---

## 🛠 Tech Stack

| Layer            | Technology                          |
|------------------|-------------------------------------|
| Visualization    | Power BI Desktop                    |
| Data Sources     | CSV / Excel (stored in `/data`)     |
| DAX Measures     | Custom KPIs (see `/docs/dax_measures.md`) |
| Version Control  | Git & GitHub                        |

---

## 🚀 How to Open

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone this repo:
   ```bash
   git clone https://github.com/saurabhshreni-cmyk/credit-card-financial-dashboard.git
   ```
3. Open `Credit_Card_Report.pbix` in Power BI Desktop
4. If prompted about data source paths, update them:
   **Home → Transform Data → Data Source Settings → Change Source**
   Point it to the CSV files in the repo.

---

## 📝 Changelog

See [CHANGELOG.md](./CHANGELOG.md) for the full version history.

---

## 👤 Author

**Saurabh Shreni**
B.Tech CSE (AI) — Manipal Institute of Technology, Bengaluru (2023–2027)

[![GitHub](https://img.shields.io/badge/GitHub-saurabhshreni--cmyk-181717?style=flat&logo=github)](https://github.com/saurabhshreni-cmyk)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Saurabh%20Shreni-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/saurabh-shreni-215b5b357)

---

*Data used in this dashboard is for analytical and portfolio demonstration purposes.*
