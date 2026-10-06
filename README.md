# Superstore Sales Analytics

## Project Overview

This project analyzes Superstore sales data using Power BI to understand sales, profitability, customers, products, regions, and time-based performance.

The dashboard was built to provide interactive business insights through data cleaning, data modeling, DAX measures, and interactive visualizations.

## Tools & Technologies

- Power BI Desktop
- Power Query
- DAX
- Excel
- Data Modeling
- Data Relationships

## Key KPIs

- Total Sales
- Total Profit
- Total Orders
- Profit Margin %
- YoY Growth %

## Key Analysis

- Sales and Profit by Region
- Sales and Profit by Category
- Sales and Profit by Sub-Category
- Top 10 Customers
- Top 10 Products
- Customer-level analysis
- Year-wise performance
- Time-based sales analysis

## Dashboard Features

- Interactive KPI Cards
- Region, Segment and Year Slicers
- Drill-down Analysis
- Interactive Tooltips
- Bookmarks
- Action Buttons
- Page Navigation
- Customer-level Details
- Top 10 Customer Analysis
- Top 10 Product Analysis

## Data Model

A DAX Calendar table was created and connected with the Superstore Order Date field to support time-based analysis and YoY comparison.

## DAX Measures

### Total Sales

```DAX
Total Sales = SUM(Superstore[Sales])
Total Profit = SUM(Superstore[Profit])
Total Orders = DISTINCTCOUNT(Superstore[Order ID])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
YoY Growth % =
DIVIDE(
    [Total Sales] - [Previous Year Sales],
    [Previous Year Sales],
    0
)

Report Pages
1. Superstore Sales Dashboard
Main dashboard containing KPI cards, sales and profit analysis, slicers, regional analysis, category analysis, and Top 10 analysis.
2. Customer Details
Detailed customer-level analysis with interactive filtering.
3. Customer Tooltip
Interactive tooltip page providing additional customer-level information.

screenshots/superstore-dashboard.png
screenshots/customer-details.png
screenshots/customer-tooltip.png
