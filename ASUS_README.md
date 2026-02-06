# ASUS Tech Products Analysis

A comprehensive end-to-end data analysis project focusing on market dynamics, product performance, and pricing sentiment analysis for ASUS computer hardware products. This project combines data cleaning, SQL analytics, and Power BI visualization to deliver actionable business insights across global markets.

## 📊 Project Overview

This project analyzes ASUS product sales data across multiple dimensions including geography, customer segments, product categories, and time periods. The analysis provides strategic insights into market dynamics, customer behavior, product performance, and pricing strategies to support data-driven business decisions.

## 🎯 Project Objectives

### 1. Market Dynamics Analysis
- Understand sales variations across geography, time, and product categories
- Analyze regional demand patterns and seasonal trends
- Evaluate customer demographics and purchasing behavior
- Identify top-performing regions, countries, and cities

### 2. Product Performance Evaluation
- Measure best-selling products and profitability metrics
- Evaluate product popularity and customer ratings
- Assess supply chain consistency and supplier performance
- Analyze stock status and inventory management

### 3. Pricing Sentiment Analysis
- Assess price perception (premium, competitive, or budget)
- Compare average prices across regions and product categories
- Enable mapping of customer feedback to price sensitivity
- Identify optimal pricing strategies by market segment

## 📁 Project Structure

```
Asus_Analysis/
├── Asus_Analysis.pbix              # Power BI dashboard and visualizations
├── Asus_Sales_Cleaning.xlsx        # Cleaned and processed data
├── customers.csv                   # Customer demographic data (296 records)
├── orders.csv                      # Transaction data (900 records)
├── products.csv                    # Product catalog (120 products)
├── Report.docx                     # Data cleaning and analysis documentation
├── SQL_Analysis.docx               # SQL queries and analytics (50+ queries)
└── README.md                       # Project documentation
```

## 📈 Dataset Description

### 1. Customers Dataset (296 records)
**Demographics & Registration:**
- `Customer_ID` - Unique customer identifier
- `Full_Name` - Customer full name (First + Last)
- `Email` - Customer email address
- `Phone_Number` - Contact number
- `Registration_Date` - Account creation date
- `Customer_Tenure_Years` - Years as customer

**Geographic Information:**
- `Street_Address` - Physical address
- `City` - Customer city
- `State/Province` - State/Province code
- `Postal_Code` - ZIP/Postal code
- `Country` - Customer country
- `Region` - Geographic region (North America, Europe, Asia-Pacific, South America)

**Customer Segmentation:**
- `Customer_Segment` - Business type (Enterprise, Retail, Enthusiast)
- `Age_Group` - Age bracket (18-25, 26-35, 36-50, 50+)
- `Preferred_Payment_Method` - Payment preference (COD, Credit Card, PayPal, Wire Transfer)

### 2. Orders Dataset (900 records)
**Order Information:**
- `Order_ID` - Unique order identifier
- `Customer_ID` - Customer reference
- `Product_ID` - Product reference
- `Order_Date` - Transaction date
- `Order_Month` - Month of order
- `Order_Year` - Year of order

**Transaction Details:**
- `Quantity` - Units ordered
- `Payment_Method` - Payment type used
- `Order_Status` - Current status (Delivered, Shipped, In Transit, Pending, Cancelled, Returned)
- `Total_Amount` - Gross order value
- `Discount_Applied` - Discount percentage
- `Net_Amount` - Final amount after discount

**Analytics Metrics:**
- `Profit_Margin` - Profit per order
- `Sentiment_Score` - Customer sentiment rating (-1 to 1)
- `Region` - Order region

### 3. Products Dataset (120 products)
**Product Identification:**
- `Product_ID` - Unique product identifier
- `Product_Name` - Full product name
- `Product_Category` - Category type (Graphics Card, Motherboard, RAM, SSD, HDD, PSU, Fan)
- `Supplier_ID` - Supplier reference

**Pricing & Performance:**
- `Price_Per_Unit` - Unit price in USD
- `Price_Sentiment` - Price positioning (Premium, Competitive, Budget)
- `Performance_Tier` - Performance level (Budget, Midrange, High-End)
- `Avg_Customer_Rating` - Average rating (1-5 scale)

**Inventory Management:**
- `Stock_Status` - Availability (In Stock, Low Stock, Out of Stock)
- `Launch_Year` - Product release year (2018-2024)

## 🔧 Data Cleaning Process

### Initial Data Inspection
- Fixed column naming conventions (CustomerID → Customer_ID)
- Removed trailing spaces using LEN() function
- Applied comprehensive filters to identify data ranges and types
- Identified and documented missing values

### Data Quality Improvements
- **Customers Table**: Standardized name formats, validated email patterns, cleaned phone numbers
- **Orders Table**: Validated date formats, ensured referential integrity, calculated derived metrics
- **Products Table**: Standardized product naming, validated price ranges, categorized products
- **Data Type Validation**: Ensured appropriate data types for all columns
- **Missing Value Treatment**: Applied appropriate strategies for null values
- **Duplicate Detection**: Identified and removed duplicate records

## 💡 SQL Analysis Highlights

The project includes **50+ SQL queries** covering:

### Market Dynamics
- Total sales by region and trend analysis
- Top 10 countries and cities by sales
- Monthly and seasonal sales trends
- Average order value by region
- Geographic performance comparison

### Customer Analytics
- Orders by customer segment
- Customer distribution by country
- Registration trend analysis
- Customer Lifetime Value (LTV) calculation
- Repeat vs one-time customer analysis
- Customer tenure vs spending correlation
- Age group sales analysis

### Product Performance
- Top 10 best-selling products
- Most profitable products by category
- Average rating by product category
- Stock status distribution
- Supplier performance metrics
- Launch year impact analysis

### Pricing Analysis
- Average price by category and region
- Price sentiment distribution
- Performance tier analysis
- Competitive pricing insights

### Order & Revenue Analysis
- Order status distribution
- Payment method preferences
- Discount effectiveness analysis
- Monthly revenue trends
- Profit margin analysis

## 📊 Power BI Dashboard Features

The interactive dashboard (`Asus_Analysis.pbix`) includes:

### Key Visualizations
- **Sales Performance**: Revenue trends, YoY growth, regional comparisons
- **Geographic Analysis**: Interactive maps, regional heatmaps
- **Product Analytics**: Category performance, top products, ratings distribution
- **Customer Insights**: Segment analysis, demographics, tenure patterns
- **Profitability Metrics**: Margin analysis, discount impact
- **Inventory Overview**: Stock status, supplier performance

### Interactive Elements
- Slicers for region, category, time period
- Drill-through capabilities for detailed analysis
- Dynamic filters for customer segments
- Cross-filtering across all visualizations

## 🛠️ Tools & Technologies

- **Microsoft Excel**: Data cleaning, transformation, and initial analysis
- **SQL**: Advanced analytics and complex querying (50+ queries)
- **Power BI**: Interactive dashboard creation and visualization
- **CSV Processing**: Raw data handling and preprocessing
- **DAX**: Calculated measures and KPIs

## 📌 Key Insights & Findings

### Market Dynamics
- **Regional Performance**: Asia-Pacific dominates with highest order volume
- **Seasonal Trends**: Identified peak sales periods and slow seasons
- **Geographic Expansion**: Opportunities in underperforming regions

### Customer Behavior
- **Segment Analysis**: Enterprise customers generate highest revenue
- **Age Demographics**: 26-35 age group is the primary customer base
- **Payment Preferences**: Credit Card and COD are most popular

### Product Performance
- **Category Leaders**: Graphics Cards and Motherboards lead in revenue
- **Rating Patterns**: Midrange products receive highest customer ratings
- **Stock Optimization**: Identified frequently out-of-stock high-demand items

### Pricing Strategy
- **Competitive Positioning**: Majority of products positioned competitively
- **Premium Opportunities**: High-End tier shows strong profit margins
- **Regional Pricing**: Price sensitivity varies across regions

## 🚀 Getting Started

### Prerequisites
- Microsoft Excel (2016 or later)
- Power BI Desktop (latest version)
- SQL environment (optional, for query execution)

### Usage

1. **Explore Data**:
   - Open CSV files to view raw data
   - Review `Asus_Sales_Cleaning.xlsx` for cleaned datasets
   - Each sheet contains processed data ready for analysis

2. **SQL Analysis**:
   - Open `SQL_Analysis.docx` to view all 50+ SQL queries
   - Use queries for custom analysis or database integration
   - Modify queries based on specific business questions

3. **Interactive Dashboard**:
   - Open `Asus_Analysis.pbix` in Power BI Desktop
   - Connect to cleaned datasets
   - Interact with visualizations for insights
   - Use slicers and filters for custom views

4. **Documentation**:
   - Review `Report.docx` for detailed methodology
   - Understand data cleaning processes
   - Learn about analytical approaches

## 📊 Analysis Categories

### Completed Analyses
✅ Market Dynamics (regional, temporal, categorical)  
✅ Customer Segmentation & Demographics  
✅ Product Performance & Profitability  
✅ Pricing Sentiment Analysis  
✅ Order & Revenue Trends  
✅ Inventory & Supply Chain Analysis  

### Potential Extensions
- Customer feedback sentiment analysis
- Predictive sales forecasting
- Churn prediction modeling
- Price optimization algorithms
- Market basket analysis
- Customer segmentation clustering

## 🎓 Business Value

This analysis enables stakeholders to:
- Make informed pricing decisions based on market sentiment
- Optimize inventory management and reduce stockouts
- Identify high-value customer segments for targeted marketing
- Understand regional market dynamics for expansion planning
- Improve product mix based on performance metrics
- Enhance profitability through data-driven strategies

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to:
- Submit bug reports or feature requests
- Propose new analytical approaches
- Enhance visualizations
- Add new SQL queries

## 📧 Contact

**Aditya Singh**
- GitHub: [@AdityaSingh7764](https://github.com/AdityaSingh7764)

## 📄 License

This project is available for educational and analytical purposes.

---

## 🔍 Technical Highlights

- **Data Volume**: 900+ transactions, 296 customers, 120 products
- **Geographic Coverage**: Global presence across 4 regions
- **Time Period**: Multi-year analysis (2018-2025)
- **Analysis Depth**: 50+ SQL queries covering 6 major categories
- **Visualization**: Comprehensive Power BI dashboard with interactive features
- **Documentation**: Detailed reports on methodology and findings

---

⭐ **If you found this project helpful, please consider giving it a star!**

*Data-driven insights for ASUS tech products market analysis*
