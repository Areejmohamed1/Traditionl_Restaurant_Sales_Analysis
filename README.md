# 🍽️ Restaurant Sales Analytics | End-to-End Data Pipeline

## Project Overview

A production-grade data pipeline and interactive BI solution built on **11 million+ restaurant transactions**, covering 6 branches across Egypt from 2020 to 2025.

The system was designed to answer real operational questions — not just display numbers — by combining high-performance batch processing in **Databricks** with rich, executive-ready dashboards in **Power BI**.

---

## Dashboard Preview

### Page 1 — Sales Overview
![Sales Overview](dashboard_page1.PNG)

### Page 2 — Customer & Product Analysis
![Customer & Product Analysis](dashboard_page2.PNG)

---

## Key Business Questions Answered

| Question | Answer |
|---|---|
| Which branch leads in revenue? | Cairo — **1.01bn EGP** |
| When do customers order most? | Friday & Saturday evenings |
| Top-selling item? | Kebab — **505M EGP** |
| Preferred payment method? | Cash — **50% of transactions** |
| Peak months? | January & October |
| Customer satisfaction? | **64% Excellent** ratings |

---

## Dashboard Features

### Page 1 — Sales Overview
**KPIs:** Net Revenue · Total Orders · Total Quantity · Total Customers · Total Discount · Avg Order Value

**Visuals:**
- Branch Performance (horizontal bar)
- Order Type Per Branch (stacked bar — Delivery / Dine-in / Takeaway)
- Customer Satisfaction Per Branch
- Top 10 Items by Revenue
- Revenue Per Category (treemap)
- Order Type Split (donut)
- Rating Distribution (donut)

### Page 2 — Customer & Product Analysis
**Visuals:**
- Season & Monthly & Daily Performance (area line charts)
- Customer Satisfaction Trend over time
- Orders by Time of Day
- Payment Preference (donut)

---

## Business Insights

** Cairo dominates** — contributes ~35% of total network revenue, nearly double the next branch (Alexandria & Giza at 0.58bn each).

** Demand is highly seasonal** — Q3 and Q4 consistently outperform, with January and October as monthly peaks. Staff and inventory planning should reflect this.

** Evening & Afternoon are critical** — these two slots alone account for ~83% of all orders (8.9M each), making them the highest-priority windows for operations.

** Cash still dominates** — 50% cash vs. 30% card vs. 20% wallet. Opportunity to push digital payment adoption, especially for delivery orders.

** Strong satisfaction baseline** — 64% Excellent ratings, but the gap between branches is worth monitoring to protect brand consistency.

---

## Architecture & Tech Stack

```
Raw Data (JSON + Excel)
        ↓
   Databricks (PySpark)
        ↓
   Delta Lake (pre-aggregated tables)
        ↓
   Power BI (DirectQuery / Import)
        ↓
   Executive Dashboards
```

| Layer | Tool | Purpose |
|---|---|---|
| Processing | Databricks + PySpark | Handle 11M rows at scale |
| Storage | Delta Lake | ACID transactions, versioning |
| Modeling | SQL / Data Modeling | Star schema, measures |
| Visualization | Power BI | Interactive reporting |

---

## Challenges & Solutions

**Performance at scale** — 11M rows caused direct-query lag in Power BI. Solved by pre-aggregating at the Databricks layer before import, reducing model size by ~90%.

**Data unification** — Source data came in inconsistent formats (JSON exports + Excel files). Built a unified ingestion layer in Databricks to normalize structure before loading to Delta.

---

## Business Value

This solution enables restaurant management to:
- Identify underperforming branches before problems compound
- Align staffing with actual demand patterns (time of day, day of week)
- Track customer satisfaction trends in real time
- Make category and menu decisions backed by revenue data
