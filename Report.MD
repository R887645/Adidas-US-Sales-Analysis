# Introduction

In the modern retail landscape, data-driven insights are essential for strategic decision-making.
The goal of this project is to uncover performance trends, regional strengths, and growth opportunities across Adidas’ U.S. sales data.

The project demonstrates proficiency in data cleaning, modeling, DAX measure creation, and visualization storytelling within Power BI.
Beyond building the dashboard, this analysis explores what the data reveals about Adidas’ sales performance and provides actionable recommendations for business improvement.

# Project Objectives
The core objectives of this project include:

- To analyze Adidas’ sales data and identify key performance drivers.

- To uncover regional strengths and weaknesses across the U.S. market.

- To evaluate product category performance and sales channels.

- To measure year-over-year (YoY) growth, profitability, and margin trends.

- To develop a comprehensive, interactive Power BI dashboard for insight visualization.

# Data Overview

The dataset contains transactional records of Adidas sales across various dimensions such as retailers, regions, product categories, and time periods.

## Data Sources
The data was provided as a structured Excel file containing:

- **Fact Table:** Sales transactions (sales value, profit, units sold, date, etc.)

- **Dimension Tables:** Retailers, Products, Regions, and Dates

## Data Fields

Key variables include:

- Date, Region, State, and Retailer

- Product Category and Model

- Units Sold, Total Sales, Operating Profit, and Margin

# Data Preparation

The dataset was imported into Power BI Desktop for transformation and cleaning using Power Query Editor.

The following steps were performed:

- Removed about 12 Null Values from both the Fact and Dimension tables to ensure data integrity.

- Verified Data Types (ensuring numeric, date, and text fields were properly formatted).

- Created a Standardized Schema by renaming columns for consistency.

- Validated Relationships across tables by checking for duplicate or missing keys.

- After transformation, the cleaned data was loaded into Power BI for modeling and analysis.

# Data Modeling

The data model followed a Star Schema Design with a central Fact Table (Sales) connected to four Dimension Tables:

- Dim_Date

- Dim_Product

- Dim_Retailer

- Dim_Region

A Date Table was created using DAX to enable time intelligence functions such as YoY growth and monthly comparisons.

# DAX Analysis

Several DAX Measures were created to perform calculations and dynamic analysis:

## Anchor Measures

These represent base metrics used in other calculations.

- **Total Sales** = SUM(Fact_Sales[Sales])

- **Total Profit** = SUM(Fact_Sales[Profit])

- **Units Sold** = SUM(Fact_Sales[Units])

## Time Intelligence Measures

Used to track performance across time:

- SalesYTD
- ProfitYTD
-UnitSoldYTD
-TransactionCountYTD

## Variance Analysis

To measure performance differences:

- YoY Sales Growth

- YoY Profit Growth

- YoY Transaction Count

- Month-over-Month Change

- MoM Sales Growth

- MoM Profit Growth

- MoM Transaction Count

These DAX measures provided the foundation for all key metrics and insights displayed on the dashboard

# Data Visualization

The visualization phase focused on creating an interactive and storytelling-oriented dashboard.
Three report pages were developed:

## Home Page

- Overview of product button, deep insight button, and trend Insight button as well.

- A dynamic map visualization showing sales distribution by state.

- images of different adidas products.

## Product Deep Dive

- Performance by product category (Footwear, Apparel, Accessories).

- Profitability breakdown by product and gender segment.

- Category-level contribution to total sales.

## Trend Analysis

- Monthly sales and profit trends over time.

- Year-over-year comparisons highlighting seasonal peaks and dips.

- Time series visualization to detect cyclical patterns.

A state-level tooltip was added for geographic insights, allowing users to hover over a state and instantly view sales, profit, and growth metrics.

# Key Metrics

- The dashboard revealed a strong overall performance for Adidas’ U.S. operations.
Total sales reached approximately $899.9 million, marking a steady improvement in year-over-year revenue.
From this, the company generated a total profit of $332.1 million, reflecting efficient cost and margin management.

- Over 2.5 million units were sold across all channels — including in-store, outlet, and online — showcasing Adidas’ wide market reach.
The average profit margin stood at 42.3%, indicating a healthy balance between revenue and operational expenses.

- In terms of growth, the company recorded a year-over-year increase of 2.94%, a positive trend that highlights post-pandemic recovery and consistent market demand.

- A deeper look into yearly performance shows that 2021 accounted for nearly 80% of total sales ($717.8 million), demonstrating a sharp rebound from 2020’s $182.1 million.
This surge reflects strong consumer confidence and effective retail and marketing strategies following a challenging economic year.

**[View My Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNGJjMjM4OGItNTNiMy00MmI0LWJjOTgtODZmNGQwZmUwYWUwIiwidCI6ImZjY2Y0MmRmLTE2ZDktNGU4Ny1hNmUwLWU0OTYyMjAxN2Y3NCJ9)**

# Insights and Findings
## Channel Performance

- In-store sales led with **$356.6M**, confirming the continued relevance of physical retail.

- Online **($247.7M)** and Outlet **($295.6M)** channels are growing rapidly, indicating the success of Adidas’ omnichannel approach.

## Regional Performance

- The West Region recorded the highest revenue ($269.9M).

- The Midwest underperformed, revealing opportunities for targeted campaigns and partnerships.

## Product Analysis

- Men’s Street Footwear **($208.8M)** and Women’s Apparel **($179M)** were top-selling categories.

- Women’s Apparel had the highest profit margin, showing strong potential in performance and athleisure lines.

## Time-Based Trends

- Sales peaked in July and December, driven by summer and holiday demand.

- Slower months were February and October, suggesting room for seasonal promotions.

# Recommendations

Based on the insights derived, the following strategic actions are proposed:

- **Enhance Online Engagement:**
Launch exclusive online collections and promotional campaigns to boost e-commerce performance.

- **Focus on Women’s Segment:**
Expand marketing and product development in women’s performance and athleisure wear due to high margins and growing demand.

- **Regional Marketing Strategy:**
Implement localized campaigns and collaborations in the Midwest to improve regional performance.

- **Seasonal Promotion Planning:**
Introduce discount campaigns and loyalty rewards during off-peak months (Feb & Oct) to balance revenue trends.

- **Retail Partnerships:**
Continue leveraging high-performing retailers like Foot Locker and West Gear for exclusive product launches.

# Tools Used
- Excel
- Power BI Desktop
- Dax Analysis
- Powr Query Editor

# Challenges Faced

- Handling missing and inconsistent data during cleaning.

- Designing an intuitive and responsive dashboard layout.

- Optimizing DAX calculations for better performance.

These challenges improved my understanding of data modeling efficiency and visualization clarity in Power BI.

# Conclusion

This Adidas U.S. Sales Dashboard project deepened my understanding of data storytelling, DAX modeling, and performance analysis using Power BI.
Through this project, I demonstrated how analytics can uncover valuable insights — from channel optimization to regional marketing strategies.

The process also reinforced the importance of turning raw data into actionable business intelligence, bridging the gap between analytics and strategy.

