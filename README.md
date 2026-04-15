# 🍽️ Restaurant Sales Analytics: Big Data End-to-End Project

## Project Overview
This project focuses on building a scalable data pipeline and interactive dashboards to analyze **11 million+ rows** of restaurant transaction data.
Using **Databricks** for high-performance processing and **Power BI** for reporting.

The goal was to move beyond simple charts and create a system that identifies operational bottlenecks, peak performance periods, and customer spending habits across different branches.

This dashboard helps answer key business questions:

* Which branch performs best?
* What are the most popular items?
* When do customers order the most?
* How satisfied are customers?
* What payment methods are preferred?

---

# Dashboard Preview

## Sales Overview Dashboard


![Sales Overview Dashboard](dashboard_page1.PNG)

## Customer & Product Analysis Dashboard


![Customer & Product Analysis Dashboard](dashboard_page2.PNG)

---

#  Dashboard Features

## Sales Overview

### KPIs

* Net Revenue
* Total Orders
* Total Quantity
* Total Customers
* Total Discount
* Average Order Value

### Visualizations

* Branch Performance
* Order Type Per Branch
* Customer Satisfaction Per Branch
* Top 10 Items
* Revenue Per Category
* Order Type Split
* Rating Distribution

---

## Customer & Product Analysis

### Visualizations

* Season Performance
* Monthly Performance
* Daily Performance
* Customer Satisfaction Trend
* Orders Timing
* Payment Preference

---

# Business Insights

* **Regional Leaders:** **Cairo** stands out as the highest-performing branch, significantly driving total revenue.
* **Peak Demand:** Sales consistently peak during **January and October**, with **Fridays and Saturdays** being the busiest days of the week.
* **Rush Hour Management:** The **Evening and Afternoon** slots account for the bulk of order volume, highlighting key periods for staff optimization.
* **Customer Preferences:** **Cash** is the preferred payment method (50% of transactions), and **Kebab & Tajines** are the most popular product categories.

---

# Tools & Technologies

* Databricks
* SQL
* Delta Lake
* Power BI
* Data Modeling
* Data Visualization

---
# Challenges & Solutions
* **Performance Scaling:** To prevent dashboard lag with 11M rows, I implemented pre-aggregation strategies within Databricks before importing data into Power BI.
* **Data Integration:** Unified inconsistent data structures from JSON and Excel into a single, clean reporting layer.

---
# Business Value

This dashboard helps:

* Improve sales performance
* Understand customer behavior
* Optimize operations
* Increase profitability
