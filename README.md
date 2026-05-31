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

## 🏗️ Architecture

```
Raw Data (CSV)
│
├── credit_card.csv   ← Transaction records
├── customer.csv      ← Customer demographics
├── cc_add.csv        ← Card metadata
└── cust_add.csv      ← Address/location data
│
▼
Power BI Desktop
│
├── Power Query (M)   ← Data ingestion, cleaning, transformation
├── Data Model        ← Star schema: fact + dimension tables
├── DAX Measures      ← KPI calculations (Revenue, WoW %, Rates)
│
▼
Dashboard Pages
│
├── Page 1: Transaction Report   ← Revenue, card tier, category, mode
└── Page 2: Customer Report      ← Demographics, geography, activation
│
▼
Exports & Version Control
├── PDF snapshots → /exports
└── Git → GitHub (this repo)
```

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

### 1. 🏦 The Mid-Tier Monopoly
**Blue and Silver credit card tiers account for 93% of all transactions** — making
premium cards nearly irrelevant to portfolio revenue generation.

Data: Blue & Silver → 93% of transaction volume. Platinum/Gold → remaining 7%.

Implications:
- Premium card positioning does not translate to revenue dominance at scale
- Mid-tier products drive portfolio consistency and transaction frequency
- Upselling strategies must account for behavioral loyalty to existing card tiers

---

### 2. 📅 The Week 53 Surge
**Revenue spiked +28.8% week-over-week in the final week of December**, confirming
strong year-end seasonal spending as a structural, repeatable pattern.

Data: Week 53 (31 Dec) WoW Revenue Change = +28.8%

Implications:
- Q4 / holiday-period revenue volatility must be factored into financial forecasting models
- Targeted promotions in Weeks 50–53 could amplify an already favorable seasonal trend
- Staffing, credit limit, and fraud detection resources should scale up for Q4 peaks

---

### 3. 👥 The Gender Revenue Gap
**Male customers outperform female customers by $5M in total revenue ($31M vs $26M)**,
but the gap's week-on-week movement reveals evolving segment dynamics.

Data: Male Revenue = $31M | Female Revenue = $26M | Delta = $5M

Implications:
- The $5M gap is significant but not insurmountable — female segment has upside potential
- Targeted engagement campaigns could shift this balance over subsequent quarters
- Gender-disaggregated WoW tracking is essential for measuring campaign effectiveness

---

### 4. 🗺️ The Coastal Concentration Risk
**Three states — Texas, New York, and California — generate 68% of total revenue**,
creating a dangerous geographic dependency for the portfolio.

Data: TX + NY + CA = 68% of $57M total revenue

Implications:
- Any regional economic downturn in these three states would materially impact the portfolio
- States outside this cluster represent an underexplored growth opportunity
- Geographic diversification should be a strategic priority in product expansion planning

---

### 5. ⚡ The Activation Ceiling
**With an activation rate of only 57.5%, nearly 1 in 2 issued cards is generating zero revenue**,
representing the portfolio's single largest untapped opportunity.

Data: Activation Rate = 57.5% → 42.5% of issued cards are inactive

Implications:
- A 10-percentage-point improvement in activation rate could add millions in incremental revenue
- Onboarding friction, cardholder education, and incentive design should be audited
- Activation rate is a leading indicator — it should be the #1 KPI in quarterly reviews

---

### 6. 🚨 The Delinquency Signal
**A 6.06% delinquent account rate indicates meaningful credit risk concentration**
that requires proactive portfolio management intervention.

Data: Delinquent Rate = 6.06% of total accounts

Implications:
- Early delinquency detection models (30/60/90 DPD) should be layered into the dashboard
- Collections and outreach workflows need calibration to this segment
- Delinquency segmented by card tier, state, and customer income could isolate risk drivers

---

### 7. 💰 The Interest Income Engine
**Interest income of $8M on $57M total revenue represents a 14% contribution ratio**,
signaling a meaningful reliance on revolving credit behavior.

Data: Interest Earned = $8M | Total Revenue = $57M | Interest/Revenue = ~14%

Implications:
- Revolving balance customers are disproportionately valuable — retention is critical
- Rate sensitivity analysis should inform repricing decisions for this segment
- Cross-selling balance transfer or credit line increase products to revolvers could expand this ratio

---

## 🧭 Executive Summary

The credit card portfolio analyzed in this dashboard reveals a clear strategic picture:

**Revenue drivers are concentrated** — mid-tier card tiers (93%), three coastal states (68%),
and male customers ($31M) dominate the portfolio, creating both predictability and risk.

**The biggest opportunity is activation** — at 57.5%, nearly half of all issued cards
sit idle. Converting even a fraction of inactive cardholders into active spenders
represents the highest-leverage growth lever available.

**Seasonal behavior is structural** — the +28.8% WoW spike in Week 53 is not noise;
it is a repeatable pattern that demands proactive planning in forecasting, risk, and operations.

**Risk signals need watching** — a 6.06% delinquency rate and 14% interest income
dependency indicate the portfolio carries meaningful credit risk that must be actively managed.

These findings provide a foundation for:
- Targeted activation and re-engagement campaigns
- Geographic expansion into underrepresented states
- Seasonal forecasting model refinement
- Credit risk segmentation and early-warning systems
- Gender and demographic segment investment prioritization

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
