# ASUS Tech Products Sales, Product Performance & Pricing Sentiment Analysis

## Project Overview
This project focuses on analyzing ASUS tech product sales data to uncover insights related to market dynamics, product performance, and pricing sentiment. Using SQL driven analysis and Power BI for visualization, the project evaluates regional demand, customer behavior, product profitability, supplier performance, and price perception to support data driven business decisions.

The repository demonstrates end to end analytical thinking from data cleaning and validation to insight generation and dashboard ready outputs aligned with real business objectives.

## Project Objectives

### 1. Market Dynamics
- Analyze sales performance across regions, countries, and cities
- Identify seasonal and monthly sales trends
- Understand customer demographics and segmentation
- Track customer growth and registration trends

### 2. Product Performance
- Identify best selling and slow moving products
- Measure product revenue contribution and lifecycle performance
- Evaluate supplier wise sales performance
- Analyze stock availability and demand patterns
- Compare performance across product categories

### 3. Pricing Sentiment Analysis
- Classify products as Premium, Competitive, or Budget
- Compare average prices by region and category
- Analyze discount impact on sales and profitability
- Study customer sentiment scores vs pricing
- Evaluate profit margin trends

## Dataset Description
The analysis is based on three cleaned and standardized datasets:

### 1. Customers Table
Customer_ID, Full_Name, Email, Phone_Number,
Registration_Date, Street_Address, City, State/Province,
Country, Customer_Segment, Region, Age_Group,
Customer_Tenure_Years, Preferred_Payment_Method

### 2. Orders Table
Order_ID, Customer_ID, Order_Date, Product_ID,
Quantity, Payment_Method, Order_Status, Total_Amount,
Order_Month, Order_Year, Region, Discount_Applied,
Profit_Margin, Sentiment_Score, Net_Amount

### 3. Products Table
Product_ID, Product_Name, Product_Category, Supplier_ID,
Price_Per_Unit, Launch_Year, Stock_Status,
Avg_Customer_Rating, Performance_Tier, Price_Sentiment

## Data Cleaning & Preparation
Significant preprocessing was performed before analysis:

- Standardized column names across datasets
- Fixed inconsistent data types
- Handled missing, blank, and negative values
- Corrected geographical mismatches (City, State, Country)
- Derived calculated fields such as Net Amount
- Standardized categorical fields for dashboard readiness
- This ensures high data quality and reliable insights.

## Key Analyses Performed

1. Sales & Market Analysis
- Total sales by region and country
- Top cities by revenue
- Monthly and yearly sales trends
- Average order value by region
- Customer registration growth

2. Customer Behavior Analysis
- Customer lifetime value (LTV)
- Repeat vs one time customers
- Segment wise order distribution
- Tenure based spending patterns

3. Product Performance
- Best selling & high-revenue products
- Slow moving products identification
- Category level performance comparison
- Supplier contribution analysis
- Product lifecycle trends

4. Pricing & Sentiment
- Price perception by region & segment
- Discount impact on sales
- Profit margin analysis by product
- Sentiment score relationship with pricing

## Power BI Dashboard
Power BI will be used to:

- Build interactive dashboards
- Visualize regional, product, and customer trends
- Enable drill down analysis across time, geography, and categories
- Present insights using KPI cards, charts, and slicers

## Tools & Technologies

SQL - Core analysis & data exploration
Excel - Data cleaning and validation
Power BI - Interactive dashboards & business insights
GitHub - Version control & project documentation

## Key Business Insights

- Clear identification of high value regions and products
- Recognition of premium vs competitive pricing strategies
- Detection of stock risks and supplier dependencies
- Understanding of customer purchasing behavior and loyalty
- Actionable insights for pricing optimization and inventory planning

## Repository Structure

📦 ASUS Sales Analysis
 ┣ 📄 SQL_Analysis.docx
 ┣ 📄 Report.docx
 ┣ 📄 README.md
 ┗ 📊 PowerBI_Dashboard.pbix (to be added)

### Author
Aditya Singh
Data Analyst | SQL | Power BI | Business Intelligence
