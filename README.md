# Retail_sales
Uncovering sales trends and customer behavior from transactional data using MySQL
# Retail Sales Analysis — Uncovering sales trends and customer behavior from transactional data using MySQL

## 📌 Overview
Retail businesses need to know which categories drive revenue, who their highest-value customers are, and when their busiest sales periods fall in order to plan inventory and staffing. This project uses SQL to clean a raw retail transactions dataset and answer 10 concrete business questions about sales patterns, customer segments, and timing.

## 📊 Dataset
- **Source:** [where the data came from — e.g. Kaggle retail transactions dataset]
- **Size:** Transaction-level data with customer demographics, product category, quantity, pricing, and total sale value
- **Period covered:** [fill in the date range covered by your dataset]

## 🛠️ Tools & Techniques
- **Tool:** MySQL
- **Key techniques:** Joins, CTEs, Window Functions (RANK), CASE statements, GROUP BY aggregations

## 🔍 Approach
1. Fixed column naming issues (encoding artifacts, typos) and validated the dataset for null values across all fields.
2. Standardized `sale_date` and `sale_time` column types for accurate date/time-based querying.
3. Wrote 10 business-driven SQL queries — segmenting sales by category, gender, and month, and ranking best-selling periods using window functions.
4. Used a CASE-based CTE to bucket transactions into Morning/Afternoon/Evening shifts for time-of-day analysis.

## 💡 Key Insights
- **Electronics generated the highest total sales** (₹3,28,400), narrowly ahead of Clothing (₹3,11,070), with Beauty trailing at ₹2,71,850 despite reaching almost as many unique customers (143 vs. 148–150) — pointing to smaller basket sizes rather than weak demand.
- **The top 5 customers** — CUST-1041, CUST-0982, CUST-1120, CUST-0764, CUST-0899 — together account for ₹1,69,850 in sales, roughly 19% of total revenue from just 5 of 155 customers.
- **Afternoon (12–17h) is the busiest shift** with 810 orders, ahead of Morning (620) and Evening (570).
- **The best-selling month shifted year over year** — December in 2022, February in 2023 — suggesting a seasonal or promotional driver worth investigating.
- **Average customer age in the Beauty category is 40.2 years**, giving a demographic anchor for targeted marketing.

> ⚠️ **Note:** the figures above are placeholder/illustrative values. Run the queries in `sql/retail_sales.sql` against your dataset and replace them with the actual output — these are the exact numbers an interviewer will ask you to explain.

## 📷 Dashboard Preview
Add a screenshot of a key query result (e.g. the top-5-customers or monthly-trend output) here — even a plain results table adds credibility.

## 📁 Repository Structure
```
├── README.md
├── sql/
│   └── retail_sales.sql   # full analysis script
└── images/                # screenshots for this README
```

## ▶️ How to Reproduce
MySQL:
```bash
mysql -u root -p < sql/retail_sales.sql
```
Then run individual `SELECT` queries from a MySQL client (MySQL Workbench, DBeaver, or the CLI) to reproduce each result.

## 👤 Author
**Shubham Kumar Gupta**
Data Analyst | [LinkedIn](https://www.linkedin.com/in/shubham-kumar-gupta-a4551b191) | [GitHub](https://github.com/shubamkumargupta-123)
