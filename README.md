# E-Commerce Customer Intelligence Dashboard
### End-to-end business analytics project using Excel and Power BI

---

## Project Overview

This project simulates a real-world business analyst workflow for **UrbanCart**, a fictional D2C e-commerce brand. Using 100,000+ real orders from the Olist Brazilian E-Commerce dataset, I built a complete analytics pipeline — from raw CSV data to an executive Power BI dashboard — to answer three critical business questions:

- Who are our most valuable customers?
- Why are we losing revenue?
- Which product categories and payment methods drive the most growth?

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Data cleaning, Power Query, RFM segmentation |
| Power BI Desktop | Data modelling, DAX measures, dashboard |
| DAX | Custom KPI measures, calculated columns |
| Git & GitHub | Version control and portfolio hosting |

---

## Dataset

**Olist Brazilian E-Commerce Public Dataset**
- Source: [kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- 99,441 orders across 5 tables
- Period: September 2016 to October 2018
- Tables used: orders, order items, payments, customers, products

---

## What I Built

### Phase 1 — Data Cleaning (Excel + Power Query)
- Imported 5 CSV files into a single master Excel workbook
- Fixed date columns stored as text using Text to Columns
- Added calculated columns — delivery_status, delivery_days, total_revenue
- Consolidated payment data using PivotTable (one row per order)
- Removed irrelevant columns across all 5 tables

### Phase 2 — RFM Segmentation (Excel)
- Built customer-level RFM table using PivotTable and SUMIF formulas
- Calculated Recency (days since last order), Frequency (order count), Monetary (total spend) for all 96,096 customers
- Scored each customer 1-5 on each dimension
- Segmented customers into 4 groups — Champion, Loyal Customer, At Risk, Lost

### Phase 3 — Data Modelling (Power BI)
- Loaded master Excel file into Power BI Desktop
- Built star schema with fact and dimension tables
- Created relationships between all 5 tables
- Wrote DAX measures for KPIs — Total Revenue, Avg Order Value, Avg Delivery Days, segment counts

### Phase 4 — Executive Dashboard (Power BI)
Built a 3-page interactive dashboard:

**Page 1 — CEO Overview**
- 4 KPI cards (Revenue, Orders, Customers, Avg Order Value)
- Monthly revenue trend line chart
- Order status donut chart
- Revenue by customer state bar chart
- Orders by month and day of week
- Revenue vs orders dual axis chart
- Avg delivery days trend
- Year slicer for filtering

**Page 2 — Customer Intelligence**
- 4 segment KPI cards (Champion, Loyal, At Risk, Lost counts)
- Customer count by segment bar chart
- Revenue contribution by segment donut
- RFM score distribution column chart
- Avg recency days by segment
- Avg spend by segment
- Top customer details table

**Page 3 — Product & Payment Analysis**
- Top 6 categories by revenue bar chart
- Payment method breakdown donut
- Avg delivery days by month trend
- Orders by payment installments
- Category performance summary table

---

## Key Findings

### Finding 1 — Customer Retention Crisis
> 50.7% of customers (50,419) are At Risk of churning with an average recency of 286 days. A targeted re-engagement campaign could recover an estimated **R$302K+** in revenue.

### Finding 2 — Champion Customers Are Severely Underserved
> Only 314 customers (0.3%) are Champions but they spend an average of R$1,531 — **19x more than Lost customers**. A VIP loyalty programme targeting this segment could generate **R$480K+** in incremental revenue.

### Finding 3 — Payment Concentration Risk
> 78.34% of all orders are paid by Credit Card. Diversifying payment methods with targeted incentives could reduce processing costs by **R$80K annually**.

---

## Dashboard Screenshots

### Page 1 — CEO Overview
![CEO Overview](dashboard/page1_ceo_overview.png)

### Page 2 — Customer Intelligence
![Customer Intelligence](dashboard/page2_customer_intelligence.png)

### Page 3 — Product & Payment Analysis
![Product Payment](dashboard/page3_product_payment.png)

---

## Skills Demonstrated

- Data cleaning and transformation in Excel and Power Query
- RFM customer segmentation methodology
- Star schema data modelling in Power BI
- DAX measure writing for business KPIs
- Business storytelling and insight communication
- End-to-end analyst project ownership

---



Feel free to connect with me on LinkedIn or reach out if you have any questions about this project.
