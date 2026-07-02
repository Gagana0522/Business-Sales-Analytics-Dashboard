#Business-Sales-Analytics-Dashboard

[Dashboard Preview](dashboard_screenshot.jpeg)
[Download Dashboard (.pbix)](Sales_Revenue_Dashboard.pbix)
[SQL View (.sql)](https://github.com/user-attachments/files/29092453/SQL.View.sql)
[Executive Summary View (.sql)](https://github.com/user-attachments/files/29092447/executive_summary.sql)
[Cleaned Executive Summary (.csv)](clean_executive_summary.csv)

## Project Overview
This project demonstrates an end-to-end data analytics pipeline. It takes raw transactional data from isolated tables, cleans and models it using advanced SQL concepts, and visualizes key performance indicators (KPIs) in an interactive Power BI executive dashboard.

## The Business Insights & Visuals
- **Gross Revenue & Country Performance:** Displays total gross revenue across orders, broken down by country (India vs. USA)
- **Geographic Market Distribution:** Identifies India as the dominant revenue driver, outperforming USA across order volume and value
- **Revenue Rank Trend:** Tracks how each order ranks by revenue over time, surfacing top and bottom performers at a glance

## Tech Stack & Skills Used
- **Database Management:** MySQL Workbench (Star Schema architecture using Fact & Dimension models)
- **Data Engineering & Analytics:** Advanced SQL (INNER JOINs, Reusable Views, Aggregate Functions, and Window Functions like `LEAD()`)
- **Business Intelligence:** Power BI Desktop (KPI cards, donut and bar charts, line trend charts, interactive filtering)

## Database Architecture
Built on a Star Schema with a central fact table and supporting dimension tables, enabling efficient querying and clean separation between transactional data and descriptive attributes.

## Key SQL Views
- `v_executive_summary` — aggregates gross revenue and revenue rank by order and country using CTEs and window functions
- `v_customer_churn_risk` — flags at-risk customers based on transaction recency and frequency
