# Global Superstore Sales Analysis

## Project Overview

An interactive Business Intelligence dashboard developed using Microsoft Power BI to analyse Global Superstore sales data and evaluate business performance.

The dashboard provides insights into sales trends, profitability, regional performance, geographical revenue distribution and product category contributions through interactive visualisations and key performance indicators (KPIs).

## Project Objectives

- Analyse overall sales and profit performance.
- Understand monthly sales and profit trends.
- Compare sales and profitability across regions.
- Evaluate geographical sales distribution.
- Analyse category-wise profit contribution.
- Identify the top 10 cities based on total sales.
- Enable interactive business analysis through multiple filters.

## Tools and Technologies

- Microsoft Power BI – Dashboard development and data visualisation
- Power Query – Data preparation and transformation
- DAX – KPI and calculated measure creation
- Global Superstore Dataset – Data source

## Dashboard KPIs

- Total Sales: 12.64M
- Total Profit: 1.47M
- Profit Margin: 11.61%
- Total Customers: 2K
- Total Orders: 25.035K

## DAX Measures

The following DAX measures were used to calculate key performance indicators in the dashboard.

**1. Total Sales**
```DAX
Total Sales = SUM(Orders[Sales])
```

**2. Total Profit**
```DAX
Total Profit = SUM(Orders[Profit])
```

**3. Profit Margin**
```DAX
Profit Margin % =
DIVIDE(
    SUM(Orders[Profit]),
    SUM(Orders[Sales]),
    0
)
```

**4. Total Orders**
```DAX
Total Orders =
DISTINCTCOUNT(Orders[Order ID])
```

**5. Total Customers**
```DAX
Total Customers =
DISTINCTCOUNT(Orders[Customer ID])
```

## Dashboard Analysis and Business Insights

### 1. Revenue Trend Analysis

**Visual:** Combo Chart (Column and Line)

Displays monthly Total Sales and Total Profit to understand business performance throughout the year.

**Key Observations:**
- November and December record the highest sales among the months displayed.
- February records the lowest monthly sales.
- Sales increase notably from May to June and again from July to September.
- July and October show noticeable declines in both sales and profit compared with the preceding months.
- Profit generally follows the sales trend, although the relationship is not identical every month.

**Business Inference:**

The stronger sales performance towards the end of the year suggests an opportunity to plan inventory, marketing campaigns and resource allocation around high-performing periods. The declines in July and October may also be worth investigating to understand changes in demand or profitability.

### 2. Regional Profitability Matrix

**Visual:** Scatter Chart

Compares regional performance using Total Sales and Total Profit.

- X-axis: Total Sales
- Y-axis: Total Profit
- Legend: Region
- Bubble size: Total Sales

**Key Observations:**
- Central records the highest sales and profit among the regions displayed.
- North demonstrates strong profit performance relative to its sales.
- South generates substantial sales and profit but remains below Central.
- Several other regions have comparatively smaller sales and profit values.

**Business Inference:**

Central is a major contributor to overall business performance. The business can study the strategies behind its performance and explore opportunities to improve results in regions with lower sales or profitability.

### 3. Revenue Composition by Geography

**Visual:** Treemap

Displays the geographical distribution of sales across regions and countries.

**Key Observations:**
- Sales are distributed across multiple geographical regions and countries.
- Central, South and North occupy prominent areas in the visual.
- The treemap also highlights contributions from regions such as Oceania, Southeast Asia, North Asia, EMEA, Africa, West and East.

**Business Inference:**

The business has sales activity across a diverse geographical market. Comparing country-level contributions can help identify important markets and opportunities for regional growth.

### 4. Profit Contribution by Category

**Visual:** Donut Chart

Compares the contribution of each product category to total profit.

| Category | Total Profit | Contribution |
|---|---:|---:|
| Technology | 663.78K | 45.23% |
| Office Supplies | 518.47K | 35.33% |
| Furniture | 285.20K | 19.44% |

**Key Observations:**
- Technology contributes the highest share of total profit at 45.23%.
- Office Supplies contributes 35.33%.
- Furniture contributes the lowest share at 19.44%.

**Business Inference:**

Technology is the leading category in terms of profit contribution. The business can examine the factors behind its stronger performance and investigate ways to improve Furniture profitability.

### 5. Top 10 Cities Based on Total Sales

**Visual:** Table

Ranks the top 10 cities based on Total Sales. The table also displays customer and order metrics.

**Top Performing Cities Visible in the Dashboard:**

| City | Total Sales |
|---|---:|
| New York City | 2,56,368.16 |
| Los Angeles | 1,75,851.34 |
| Manila | 1,20,866.95 |
| Seattle | 1,19,540.74 |
| San Francisco | 1,12,669.09 |
| Philadelphia | 1,09,077.01 |

**Key Observations:**
- New York City ranks first in total sales.
- Los Angeles ranks second.
- Manila ranks third among the displayed cities.

**Business Inference:**

New York City and Los Angeles are important sales-performing markets in the displayed ranking. The business can use this information to understand geographical sales concentration and evaluate opportunities in other cities.

## Interactive Dashboard Features

The dashboard includes four interactive dropdown slicers:

- **Year** – Analyse performance across different years.
- **Segment** – Compare customer segments.
- **Region** – Explore regional performance.
- **Category** – Analyse individual product categories.

These filters allow users to dynamically explore the dashboard and compare business performance across different dimensions.

## Overall Business Insights

- Total sales reach 12.64M, generating 1.47M in total profit.
- The overall profit margin is 11.61%.
- Sales performance is strongest towards the end of the year, particularly in November and December.
- Central is the leading region in the displayed profitability matrix.
- Technology contributes the highest share of category-wise profit at 45.23%.
- New York City is the highest-performing city by total sales among the cities displayed.
- Interactive slicers provide flexibility to explore sales and profitability across different business dimensions.

## Dashboard 

<img width="977" height="549" alt="Screenshot 2026-11-19 143052" src="https://github.com/user-attachments/assets/7b84d8eb-88e6-489a-9bc9-f6f0ce40cf7f" />

## Conclusion

This project demonstrates the practical application of **Microsoft Power BI** in transforming sales data into meaningful business insights through interactive dashboards and data visualisation.

It highlights skills in data analysis, KPI development, DAX calculations, geographical analysis, trend analysis and business intelligence reporting.

The dashboard provides a consolidated view of business performance and supports data-driven exploration of sales and profitability across multiple dimensions.
