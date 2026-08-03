<div align="center">

# 🛒 E-Commerce Sales & Customer Insights Dashboard

**An end-to-end data analytics project** — from messy raw data to business-ready dashboards,
built with Python, SQL, Excel, Power BI, and Tableau.

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-SQLite-07405E?logo=sqlite&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-data%20cleaning-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-K--Means-F7931E?logo=scikitlearn&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-Dashboard-217346?logo=microsoftexcel&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Guide-F2C811?logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-Guide-E97627?logo=tableau&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---
# DESCRIPTION 

An end-to-end Data Analytics project that leverages SQL, Python, Excel, and Power BI to analyze e-commerce sales and customer behavior. The project uncovers actionable insights on revenue, profitability, customer retention, product performance, and regional trends through interactive dashboards, KPI tracking, and data-driven storytelling.

### Key Highlights

* 📊 Interactive Sales & Customer Insights Dashboard
* 🛒 Analysis of Revenue, Profit, Orders, and Customer Retention
* 🎯 Customer Segmentation and Behavioral Insights
* 📈 Product and Regional Performance Analysis
* 🐍 Data Cleaning & EDA using Python
* 🗄️ Advanced SQL Queries for Business Analysis
* 📉 KPI Monitoring and Data Visualization in Power BI

### Skills Demonstrated

SQL • Python • Excel • Power BI • Data Cleaning • EDA • Dashboard Development • Business Intelligence • Data Visualization • Data Storytelling

----
## 📊 Overview

This project simulates a real Indian e-commerce business — **1,200 customers,
5,300+ orders, 180 products** — and builds a complete analytics pipeline on
top of it: data cleaning, SQL analysis, exploratory data analysis, **RFM +
K-Means customer segmentation**, and three parallel BI dashboards.

It's built to answer two kinds of questions a real business asks:

- **Sales performance** — revenue trends, seasonality, top products/categories, geography
- **Customer insights** — who are our best customers, who's at risk of churning, which
  acquisition channels are actually worth the spend
  
---

## 🖼️ Preview

<p align="center">
  <img src="https://github.com/hemanthsri879/E-Commerce-Sales-Customer-Insights-Dashboard/blob/a58bcc1caf4cdd8b7e9c820c2a6f6b6d647399e7/ecommerce%201%20image.jpg" width="900" alt="Excel Dashboard">
</p>

<p align="center">
  <em>Excel dashboard — 47,000+ live formulas, zero hardcoded values</em>
</p>

<p align="center">
  <img src="https://github.com/hemanthsri879/E-Commerce-Sales-Customer-Insights-Dashboard/blob/ba266ff17626db69d926218a49d25e0aef248e50/ecommerce%202image.jpg" width="48%" alt="Monthly Revenue Trend">
  <img src="https://github.com/hemanthsri879/E-Commerce-Sales-Customer-Insights-Dashboard/blob/afc0ee9b93ecac194216306caf403c34b80c9036/ecommerce%203image.jpg" width="48%" alt="Customer Clusters">
</p>

<p align="center">
  <em>Left: Revenue seasonality (Diwali/festive spikes) | Right: K-Means customer clusters</em>
</p>

---

## 🧰 Tech Stack

| Layer | Tools |
|---|---|
| Data generation & cleaning | Python (pandas, numpy, Faker) |
| Database | SQLite |
| Analysis | SQL (joins, CTEs, window functions) |
| EDA & visualization | Python (matplotlib, seaborn) |
| Customer segmentation | Python (scikit-learn — K-Means, RFM) |
| Dashboards | Excel, Power BI, Tableau |

---

## 📁 Repository Structure

```
├── data/
│   ├── raw/                   # Messy synthetic source CSVs
│   └── processed/             # Cleaned CSVs + customer_insights.csv
├── sql/
│   ├── 01_schema.sql          # Relational schema, keys, indexes
│   └── 02_analysis_queries.sql # 17 queries: joins, CTEs, window functions
├── python/
│   ├── 01_generate_data.py
│   ├── 02_data_cleaning.py
│   ├── 03_eda_visualization.py
│   ├── 04_customer_segmentation.py
│   └── 05_build_excel_dashboard.py
├── excel/                     # Ecommerce_Sales_Dashboard.xlsx
├── powerbi/                   # DAX + step-by-step build guide
├── tableau/                   # Calculated fields + build guide
├── charts/                    # EDA & segmentation chart exports
├── screenshots/               # Images used in this README
├── docs/                      # Full documentation + logs
└── ecommerce.db               # SQLite database
```

---

## 🚀 How to Run

```bash
pip install pandas numpy faker scikit-learn matplotlib seaborn openpyxl

python python/01_generate_data.py          # generate synthetic data
python python/02_data_cleaning.py          # clean + load into SQLite
python python/03_eda_visualization.py      # EDA charts
python python/04_customer_segmentation.py  # RFM + K-Means
python python/05_build_excel_dashboard.py  # build Excel dashboard
```
Then open `ecommerce.db` in any SQL client and run `sql/02_analysis_queries.sql`,
or follow `powerbi/PowerBI_Build_Guide.md` / `tableau/Tableau_Build_Guide.md`.

---

## 🔍 Key Insights

- Revenue peaks sharply every October/November — Diwali / festive-season seasonality
- Electronics and Mobiles & Accessories drive the largest share of revenue
- **46.6% customer churn rate** (no order in 90+ days) — a clear win-back opportunity
- UPI is the dominant payment method, consistent with the Indian market
- K-Means clustering independently confirms the rule-based RFM segments

---

