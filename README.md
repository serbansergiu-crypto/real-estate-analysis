# real-estate-analysis# 🏠 Global & Romania Real Estate Analysis
### A Data Portfolio Project · Three Global Cycles · Romania Macro · Bucharest Deep Dive · 2000–2026

[![Real Estate](https://img.shields.io/badge/Sector-Real_Estate-0F3460?style=flat)](/)
[![Romania](https://img.shields.io/badge/Focus-Romania_%26_Bucharest-E94560?style=flat)](/)
[![Data](https://img.shields.io/badge/Data_Current-March_2026-10B981?style=flat)](/)
[![SQL](https://img.shields.io/badge/SQL-PostgreSQL_14+-336791?style=flat&logo=postgresql&logoColor=white)](/)

---

## 📌 Project Overview

A comprehensive real estate market analysis covering three global cycles since 2000, Romania's EU convergence story, and a street-level Bucharest neighborhood investment map. The project combines macro cycle analysis, country-level comparisons, local market data, and an affordability model into a single analytical stack.

> **Core thesis:** Romania is one of the last undervalued real estate markets in the EU — 4th cheapest by €/sqm, rental yields 2× the EU average, and still 3× below Western European price levels. The current headwinds (high BNR rate, inflation, fiscal consolidation) are temporary. The structural tailwinds (EU convergence, supply shortage, wage growth) are multi-decade.

---

## 📁 Project Structure

```
real-estate-analysis/
│
├── README.md
│
├── dashboard/
│   └── real_estate_dashboard.html       ← Interactive 6-tab HTML dashboard
│
├── data/
│   └── real_estate_global_romania.xlsx  ← Excel workbook (6 sheets)
│
└── sql/
    ├── 01_schema_and_seed.sql           ← Full database schema + all seed data
    └── 02_05_queries.sql                ← 12 analytical queries across 4 topics
```

---

## 🗄️ Database Schema — 6 Tables

| Table | Rows | Description |
|---|---|---|
| `global_price_index` | 65+ | Annual HPI (2000=100) for 6 major markets |
| `global_market_events` | 14 | Key events driving each cycle phase |
| `romania_annual_data` | 18 | Full macro + real estate annual series 2009–2026 |
| `romania_city_prices` | 8 | Major Romanian cities: price, yield, affordability |
| `bucharest_neighborhoods` | 20 | Street-level neighborhood data across 6 sectors |
| `interest_rates` | 22 | Central bank rates by country and year |

---

## 📊 Excel Workbook — 6 Sheets

| Sheet | Contents |
|---|---|
| **KPI Dashboard** | At-a-glance KPI cards, Romania vs EU comparison table, global cycle summary |
| **Global Market Cycles** | 24 rows across US, UK, Germany, Spain, Ireland, Australia, Romania — boom/bust/recovery data |
| **Romania Macro** | 18-year price history with GDP, inflation, BNR rate, transactions + city comparison table |
| **Bucharest Deep Dive** | 20 neighborhoods across 6 sectors: €/sqm, yield, 5-yr appreciation, investment profile |
| **Rates & Affordability** | 8-country rate comparison + Bucharest mortgage affordability calculator (7 scenarios) |
| **Outlook & Scenarios** | 4 global scenarios + 4 Romania scenarios + buy/wait decision framework |

---

## 🌐 Interactive Dashboard — 6 Tabs

| Tab | Charts & Analysis |
|---|---|
| **Overview** | 5 KPI cards, Romania price history line chart, cities bar chart, Romania vs EU radar |
| **Global Cycles** | Indexed global HPI since 2000, GFC crash depth bar, post-COVID boom bar, 3 key lessons |
| **Romania** | HPI vs GDP dual bar chart, inflation/rates/mortgage line, cities comparison table |
| **Bucharest Map** | 12 neighborhood cards with €/sqm, yield, 5yr gain + full neighborhood bar chart |
| **Rates & Affordability** | Central bank rates line, full mortgage affordability table by property type |
| **Outlook 2030** | Scenario probability donut, buy/wait radar chart, 4 scenario insights, bottom-line analysis |

---

## 🔍 SQL Query Library — 12 Queries

### `01_schema_and_seed.sql` — Database setup
Complete schema creation and all seed data. Run this first.

### `02_05_queries.sql` — Analytics

**Global Cycle Analysis:**
- Cycle performance comparison: peak, trough, recovery by country
- GFC crash severity ranking
- Annual leaders and laggards globally

**Romania Deep Dive:**
- Price growth vs macro correlation (GDP, CPI, BNR rate)
- EU convergence calculator — years to reach EU average at current growth
- City investment ranking (composite score: yield + growth + affordability)

**Bucharest Neighborhoods:**
- Full neighborhood ranking by total investment return (yield + appreciation)
- Sector-level aggregates (avg price, yield, appreciation by sector 1–6)
- Best neighborhoods by budget tier (€80K, €120K, €180K, €300K, €500K)
- Mortgage affordability by neighborhood (annuity formula, 30% DTI rule)

**Rates & Outlook:**
- Rate cycle analysis: peaks, troughs, duration by central bank
- Romania rate vs price correlation
- Price scenario projections 2026–2030 (4 scenarios)
- Weighted buy/wait decision framework

---

## 📈 Key Data Points (March 2026)

### Romania at a Glance
| Metric | Romania | EU Average | Verdict |
|---|---|---|---|
| **Avg €/sqm** | €1,710 | €3,200 | 4th cheapest EU |
| **YoY price growth** | +14% | +5.2% | Top 5 EU |
| **Rental yield** | 6–7.7% | 3–4% | 2× EU average |
| **Price-to-income** | 8.8 yrs | 10.2 yrs | More affordable |
| **Mortgage rate** | ~5.55% | ~3.8% | Above EU avg |
| **Inflation** | 9.7% | 3.1% | Highest EU |
| **Homeownership** | 96% | 70% | Highest EU |

### Bucharest Neighborhoods — Top Picks 2026
| Strategy | Neighborhood | Entry | Yield | 5yr Gain |
|---|---|---|---|---|
| **Max Yield** | Titan / Berceni | €1,300–1,500/sqm | 8–9% | +35–55% |
| **Best Balance** | Militari / Drumul Taberei | €1,500–1,550/sqm | 7–8% | +45–50% |
| **Highest Momentum** | Timpuri Noi | €2,200/sqm | 7.5% | +90% |
| **Premium** | Aviației / Floreasca | €2,800/sqm | 6.5% | +80% |

---

## 🛠️ How to Run the SQL

```sql
CREATE DATABASE real_estate_analysis;
\i sql/01_schema_and_seed.sql
\i sql/02_05_queries.sql
```

---

## ⚠️ Disclaimer

This project is for **educational and portfolio purposes only**. Real estate markets are location-specific and data-dependent. Nothing here constitutes investment or financial advice. Always conduct local due diligence, consult licensed agents, and verify current regulatory conditions before making property investment decisions.

---

## 👤 Author

**[Serban Sergiu]** · Data Analyst
[LinkedIn](www.linkedin.com/in/sergiu-serban-48043313b) · [GitHub](https://github.com/serbansergiu-crypto)

*Last updated: March 2026 · Data sources: Imobiliare.ro, Investropa, Colliers Romania, Global Property Guide, Deloitte Property Index, IMF, ECB, BNR*
