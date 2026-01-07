# Chocolate-Sales-Analysis
This project provides a detailed evaluation of chocolate product performance, examining trends and variations across regions, countries, time periods, seasonal patterns, and product categories.

# Project Overview

This project analyzes chocolate sales transaction data to understand sales performance across **regions, countries, time periods, seasons, and product categories**. An interactive Power BI dashboard is used to transform raw sales data into actionable insights that support business decision-making.

# Business Objectives
- Analyze overall chocolate sales performance by revenue and quantity sold
- Identify top- and underperforming products and product categories
- Compare sales performance across regions and countries
- Examine sales trends over time and identify seasonal patterns
- Evaluate sales representative contributions to overall performance
- Enable interactive analysis through filters and dynamic visuals


## Characteristics of the Data 

The dataset includes five tables that collectively capture sales personnel details, calendar attributes, geographic dimensions, product and sales record.

## Tools used 
PowerBI

## Data Cleaning and Wrangling 

Data was fit for analysis as shown by preliminary investigation of the dataset, however in other to create a clean and precise dashboard it is mandatory we create some new measures to show specific visuals and KPIs.

- Total Sales Amount
  
```DAX
Total Sales = SUM(Sales[Revenue])
```
- Total Cost of products sold
```DAX
Total Cost of Products Sold = SUMX(Sales, Sales[Boxes] * RELATED(products[Cost per box])
```
- Gross Profit
```DAX
Gross Profit = [Total Sales Amount] - [Total Cost of Products Sold]
```



Other DAX measures used such as Average sales per day, Profit Margin, Salesperson performance Score are recorded in the DAX measures section of the project.

## Creating a model in power BI that connects all the five tables given in the dataset.

<img width="1342" height="840" alt="image" src="https://github.com/user-attachments/assets/3c2f3dd7-fe1a-462e-9ffa-5306ee4df09e" />

# Dashboard Pages
  * Sales Analysis and KPIs

<img width="2058" height="1159" alt="image" src="https://github.com/user-attachments/assets/ed5d4326-fa75-4cf5-b046-844931ea02f9" />


The dashboard shows the Total sales, Gross Profit, Total cost, Total sales by Region and countries and a general overview of sales by product with filters for individual month, product and country.

  * Trend Analysis

<img width="2078" height="1172" alt="image" src="https://github.com/user-attachments/assets/a6d3f7a6-2e0b-425a-9d02-1ea481aa40a4" />

The dashboard highlights trends in Total sales amount, Boxes Sold and profit over time. It helps identify month-to-month, yearly and seasonal variation in sales(if any) and how that can be used in making informed business decisions.

  * Product Performance
<img width="2066" height="1168" alt="image" src="https://github.com/user-attachments/assets/d11cd6fb-3ba1-4385-84af-b26bba1601d7" />

Shows gross profit from products and sales volume


  * Salesperson Performance

<img width="2056" height="1160" alt="Screenshot 2026-01-06 155939" src="https://github.com/user-attachments/assets/1dcea1dc-a5a0-4b23-b388-a67b27ad222e" />

It shows Top-performing sales representatives and team


 In Summary, the dashboards reveal that chocolate sales performance is primarily driven by strong regional demand in APAC, high-margin bar products, and pronounced seasonal peaks toward year-end. While sales personnel performance is generally consistent, opportunities exist to optimize underperforming regions and product categories. This analysis supports data-driven decisions around product focus, regional strategy, and seasonal planning.

# Key Insights
- Strong Profitablility: Total sales of approximately $46.1M generated a gross profit of about $26.6M , indicating a strong and healthy profit
margin. Year over year analysis also shows consistent growth.

- Top Markets: APAC is the highest-performing region, with the UK and USA emerging as the strongest individual country markets.
  
- Product Performance: Bars dominate sales and profit contribution, while other categories contribute significantly less.
  
- Seasonal Trends: Sales peak between October and December indicating a strong seasonal demand toward year-end, with a noticeable decline during mid-year (May–June).
  
- Sales Team Impact: A small group of top sales representatives contributes a large share of total revenue, with relatively consistent performance among them.
  
- Pricing vs Volume: Some products achieve high revenue through premium pricing, while others rely on higher sales volumes.



# Recommendation
- Inventory planning and marketing spend should be increased ahead of Q4, while demand-stimulation strategies may be needed during mid-year periods.
  
- Bars should remain the core product focus, while underperforming categories may benefit from pricing optimization, repositioning, or promotional strategies.
  
- APAC represents the primary revenue driver and should be prioritized for expansion and targeted campaigns, while Europe may require strategic review to improve market penetration.
  
- Top-performing sales representatives can be used as benchmarks for training and incentive programs to uplift lower-performing staff.







