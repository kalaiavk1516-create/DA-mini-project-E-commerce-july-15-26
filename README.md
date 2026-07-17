E-Commerce Sales & Customer Journey Analysis
📌 Project Overview

This project analyzes an e-commerce company's sales performance, customer behavior, website traffic, marketing campaigns, and refund trends using Excel, Power Query, Power BI, and DAX. The objective is to transform raw transactional data into interactive dashboards that provide meaningful business insights and support data-driven decision-making.

🎯 Objectives
Analyze customer purchase behavior.
Measure sales, revenue, profit, and refunds.
Evaluate marketing campaign performance.
Track website traffic and customer sessions.
Analyze product performance and profitability.
Build an interactive Power BI dashboard for business reporting.
📂 Dataset

Source: Maven Analytics – Maven Fuzzy Factory Dataset

Domain: E-Commerce / Retail Analytics

Time Period: 2012 – 2015

Dataset Tables
Table	Description
Website Sessions	Customer visit details, traffic source, campaign, device type
Website Pageviews	Customer navigation across website pages
Orders	Order-level information
Order Items	Product-level sales information
Products	Product master details
Order Item Refunds	Refund transactions
🛠️ Tools & Technologies
Microsoft Excel
Power Query
Power BI
DAX (Data Analysis Expressions)
🧹 Data Preprocessing

The following data preparation steps were performed:

Removed duplicate records
Handled missing values
Standardized text and date formats
Corrected data types
Created fact and dimension tables
Established relationships between tables
Built Pivot Tables for preliminary analysis
Imported cleaned data into Power BI
📊 Data Model

Relationships created in Power BI:

Orders → Order Items (Order ID)
Order Items → Order Item Refunds (Order Item ID)
Products → Order Items (Product ID)
Website Sessions → Website Pageviews (Website Session ID)

Relationship Type:

One-to-Many (1:*)
Single Cross Filter Direction
📈 DAX Measures

Some of the key measures used in the project:

Total Revenue =
SUM(order_items[Price USD])

Total COGS =
SUM(order_items[Cost of Goods Sold])

Profit =
[Total Revenue] - [Total COGS]

Profit Margin % =
DIVIDE([Profit],[Total Revenue],0)

Total Refund Amount =
SUM(order_item_refunds[Refund Amount])

Refund % =
DIVIDE([Total Refund Amount],[Total Revenue],0)

Net Revenue =
[Total Revenue]-[Total Refund Amount]

Average Price =
AVERAGE(order_items[Price USD])

Total Sessions =
COUNTROWS(website_sessions)

Total Users =
DISTINCTCOUNT(website_sessions[User ID])

New Customers =
CALCULATE(
DISTINCTCOUNT(website_sessions[User ID]),
website_sessions[Repeat Session]=0
)

Repeat Customers =
CALCULATE(
DISTINCTCOUNT(website_sessions[User ID]),
website_sessions[Repeat Session]=1
)
📊 Dashboard Features
KPI Cards
Total Revenue
Net Revenue
Total Profit
Total COGS
Profit Margin %
Total Refund Amount
Refund %
Average Product Price
Total Sessions
Total Users
Visualizations
Monthly Revenue Trend (Line Chart)
Revenue by Product (Bar Chart)
Refund Amount by Product
Sessions by Device Type (Donut Chart)
Revenue by Year and Device (Matrix)
UTM Campaign Analysis (Treemap)
Marketing Performance
Customer Session Analysis
Interactive Features
Year Filter
Quarter Filter
Device Type Filter
UTM Source Filter
Drill Down
Cross Filtering
Bookmarks
Dynamic Slicers
📌 Business Insights
Desktop users generated higher revenue than mobile users.
Google Search was the largest source of website traffic.
Refund percentage remained low compared to total revenue.
Profit margin averaged approximately 37%.
Revenue showed seasonal peaks during specific months.
Average product price was approximately $48 USD.
Certain products generated significantly higher profits than others.
💡 Recommendations
Improve the mobile shopping experience to increase conversions.
Invest more in high-performing Google Search campaigns.
Reduce refund rates by improving product quality and descriptions.
Increase marketing efforts for high-profit products.
Use seasonal sales trends for inventory and campaign planning.
📷 Dashboard Preview

Add your dashboard screenshots here

Example:

images/dashboard.png

or

assets/dashboard.png
📁 Project Structure
E-Commerce-Sales-Customer-Journey-Analysis
│
├── Dataset
│   ├── Orders.xlsx
│   ├── Order_Items.xlsx
│   ├── Products.xlsx
│   ├── Website_Sessions.xlsx
│   ├── Website_Pageviews.xlsx
│   └── Refunds.xlsx
│
├── Power BI
│   └── Ecommerce Analysis.pbix
│
├── Dashboard Images
│   ├── Dashboard.png
│   ├── Sales.png
│   └── Customer Journey.png
│
├── README.md
└── LICENSE
🚀 Skills Demonstrated
Data Cleaning
Data Transformation
Data Modeling
Power Query
DAX
Business Intelligence
Dashboard Development
Sales Analytics
Customer Analytics
Marketing Analytics
Data Visualization
Business Reporting
📌 Key Business Metrics
Metric	Description
Total Revenue	Total sales generated
Net Revenue	Revenue after refunds
Profit	Revenue minus COGS
Profit Margin	Profit percentage
Refund Rate	Refund percentage of revenue
Total Sessions	Website visits
Total Users	Unique visitors
New Customers	First-time customers
Repeat Customers	Returning customers
🎯 Conclusion

This project demonstrates an end-to-end Business Intelligence workflow using Excel, Power Query, Power BI, and DAX. Raw e-commerce data was cleaned, transformed, modeled, and analyzed to create an interactive dashboard that provides valuable insights into sales performance, customer behavior, marketing effectiveness, refunds, and profitability. The dashboard enables stakeholders to make informed business decisions and supports strategic planning through data-driven insights.
