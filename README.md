# AdventureWorks Sales Analysis - Power BI Dashboard

> **End-to-end Power BI sales dashboard | DAX | Star Schema | 56K+ rows | 4 interactive pages**

> **Suggested GitHub Topics:** `powerbi` `dax` `data-analytics` `business-intelligence` `star-schema` `microsoft` `sales-analysis`

---

## Overview

An interactive Power BI dashboard analyzing AdventureWorks sales performance, product trends, and customer behavior across multiple regions. Built using DAX measures, dynamic visuals, and drill-through functionality across 3 years of sales data (2020-2022).

This project simulates a real-world BI scenario where stakeholders need visibility into revenue trends, product returns, and customer segmentation to drive sales strategy decisions.

## Dashboard Pages

- **Executive Summary** - KPIs including Revenue ($3.2M), Profit ($1.3M), Orders (3,218), and Return Rate (2.1%)

- **Map View** - Geographic sales distribution across the USA, UK, Australia, Canada, France, and Germany

- **Product Detail** - Product-level performance with profit trends, return analysis, and price adjustment simulation

- **Customer Detail** - Customer segmentation by income level and occupation, with top customer insights

## Screenshots

[![Executive Dashboard](images/dashboard-overview.png)](images/dashboard-overview.png)

[![Map View](images/dashboard-map.png)](images/dashboard-map.png)

[![Product Detail](images/dashboard-product-detail.png)](images/dashboard-product-detail.png)

[![Customer Analytics](images/dashboard-customers.png)](images/dashboard-customers.png)

## Dataset

| Table | Description | Rows |
|---|---|---|
| Sales 2020 | Transaction data for 2020 | 2,630 |
| Sales 2021 | Transaction data for 2021 | 23,935 |
| Sales 2022 | Transaction data for 2022 | 29,481 |
| Returns | Product return records | 1,809 |
| Customer Lookup | 18,154 unique customers with demographics | 18,154 |
| Product Lookup | Product details including cost and price | 293 |
| Territory Lookup | 10 sales territories across 6 countries | 10 |
| Calendar Lookup | Date dimension table | - |
| Product Categories | 4 product categories | - |
| Product Subcategories | Product subcategory mapping | - |

## Data Model

- **Fact Tables:** Sales Data (2020-2022), Returns Data

- **Dimension Tables:** Customer, Product, Territory, Calendar, Product Categories, Product Subcategories

- **Relationships:** Star schema connecting all dimension tables to fact tables via key fields

## Key Insights

- **$3.2M** total revenue with a **42% profit margin**

- The **United Kingdom** is the top-performing territory

- **Accessories** is the most ordered category with **2,203 orders**

- **Water Bottle - 30 oz.** is the top-selling product with **506 orders**

- **Tires and Tubes** is the most ordered product category

- Average order value of **$996.59**

- **17.4K** unique customers with **$1,431** average revenue per customer

## Key DAX Measures

| Measure | Description |
|---|---|
| Total Revenue | Sum of order quantity x product price |
| Total Profit | Revenue minus total cost |
| Return Rate % | Returns / Total Orders |
| Revenue YoY % | Year-over-year revenue growth |
| Running Total Revenue | Cumulative revenue over time |
| Avg Revenue per Customer | Total Revenue / Unique Customers |

## Skills Demonstrated

- **DAX Measures** - Custom calculations including time intelligence, running totals, and YoY growth
- **Star Schema Modeling** - Designed and connected fact and dimension tables for optimal query performance
- **Power Query / M Language** - Data transformation, cleaning, and shaping of raw CSV files
- **Drill-through Navigation** - Page-level drill-through filters for product and customer deep dives
- **KPI Cards** - Dynamic headline metrics with goal tracking
- **Slicers** - Interactive filtering by date, category, territory, and customer segment
- **Bookmarks** - Used to toggle between views and simulate navigation buttons
- **Conditional Formatting** - Applied to tables and visuals to highlight outliers and performance thresholds

## Tools & Technologies

- **Microsoft Power BI Desktop** (June 2023 or later)
- **DAX** (Data Analysis Expressions) - for calculated columns, measures, and time intelligence
- **Power Query (M Language)** - for data transformation and shaping
- **Data Modeling** (Star Schema)
- **Interactive Visualizations & Drill-through**

## Challenges & Learnings

- Built a custom Calendar Lookup table using DAX CALENDAR() to enable time intelligence

- Resolved many-to-many relationship issues by using a bridge table in the star schema

- Implemented drill-through filters to allow page-level product and customer deep dives

- Used CALCULATE() with filter context to build dynamic YoY and running total measures

## How to Open

1. Download the Territory.pbix file from the report folder

2. Open with **Microsoft Power BI Desktop (June 2023 or later)**

3. Explore the interactive dashboard across all 4 pages

> **Note:** Requires Power BI Desktop June 2023 or later. Download free at https://powerbi.microsoft.com/desktop

## Author

**Manoj Pedarla** | Data Analyst | MetLife | MS Data Engineering @ UNT | PL-300 Certified

[LinkedIn](https://www.linkedin.com/in/manojpedarla)

