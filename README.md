<div align="center">

#  E-Commerce Sales & Customer Insights Dashboard

**An end-to-end data analytics project** — from messy raw data to business-ready dashboards,
built with Python, SQL, Excel, Power BI, and Tableau.

</div>

---

## 📊 Overview

This project simulates a real Indian e-commerce business — **1,200 customers,
5,300+ orders, 180 products** — and builds a complete analytics pipeline on
top of it: data cleaning, SQL analysis, exploratory data analysis, **RFM +
K-Means customer segmentation**, and three parallel BI dashboards.

It's built to answer two kinds of questions a real business asks:

- **Sales performance** — revenue trends, seasonality, top products/categories, geography
- **Customer insights** — who are our best customers, who's at risk of churning, which
  acquisition channels are actually worth the spend

**Headline finding:** 46.6% of customers hadn't placed an order in 90+ days —
a concrete, quantified churn signal, not just a pretty chart.



---

## 🖼️ Preview

<p align="center">
  <img src="C:\Users\SIVA PRASAD\Pictures\ecommerce 1 image.jpg"/>
</p>
<p align="center"><em>Excel dashboard — 47,000+ live formulas, zero hardcoded values</em></p>

<p align="center">
  <img src="screenshots/01_monthly_revenue_trend.png" alt="Monthly Revenue Trend" width="48%"/>
  <img src="screenshots/10_customer_clusters.png" alt="Customer Clusters" width="48%"/>
</p>
<p align="center"><em>Left: revenue seasonality (Diwali/festive spikes) &nbsp;|&nbsp; Right: K-Means customer clusters</em></p>

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


