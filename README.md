E-Commerce Sales & Customer Journey Analysis
📌 Project Overview

This project analyzes an e-commerce company's website traffic, customer behavior, product performance, sales, and refund data using Excel, Power Query, Power BI, and DAX. The objective is to transform raw transactional data into meaningful business insights through interactive dashboards.

🎯 Objective
Analyze customer purchase behavior.
Measure sales, revenue, profit, and refunds.
Evaluate marketing campaign performance.
Track website traffic and customer conversion.
Build an interactive Power BI dashboard to support business decisions.
📂 Dataset

Source: Maven Analytics – Maven Fuzzy Factory Dataset

Domain: E-Commerce / Retail Analytics

Timeline: 2012–2015

📥 Download Dataset

Due to GitHub file size limitations, the complete dataset is available on Google Drive.

Google Drive Link:

https://drive.google.com/drive/folders/1ficGs_Zgz2wTRN3o9hLHOR2ddixS_eMS?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto

Dataset Files
Website Sessions
Website Pageviews
Orders
Order Items
Products
Order Item Refunds
🛠 Tools & Technologies
Microsoft Excel
Power Query
Power BI
DAX
🧹 Data Preprocessing
Removed duplicate records.
Handled missing values.
Converted columns into proper data types.
Standardized date and text formats.
Created relationships between tables.
Built Fact and Dimension tables.
Imported cleaned data into Power BI.
📊 Data Model

Relationships:

Orders → Order Items (Order ID)
Order Items → Order Item Refunds (Order Item ID)
Products → Order Items (Product ID)
Website Sessions → Website Pageviews (Website Session ID)

Relationship Type

One-to-Many (1:*)
Single Cross Filter Direction
📈 DAX Measures
Total Revenue
Total COGS
Profit
Profit Margin %
Total Refund Amount
Refund %
Net Revenue
Average Price
Total Sessions
Total Users
New Customers
Repeat Customers
📊 Dashboard Features
KPI Cards
Total Revenue
Total Profit
Total COGS
Total Refund Amount
Profit Margin %
Average Price
Total Sessions
Visualizations
Monthly Revenue Trend
Refund Amount by Product
Revenue by Product
Sessions by Device Type
Revenue by Year and Device
UTM Campaign Analysis
Interactive Features
Drill Down
Cross Filtering
Slicers
Bookmarks
📈 Key Insights
Desktop users generated higher revenue than mobile users.
Google Search contributed the highest website traffic.
Refund percentage was relatively low compared to total revenue.
Profit margin remained around 37.26%.
Revenue showed seasonal trends with peak sales during specific months.
Average product price was approximately 48 USD.
💡 Recommendations
Improve mobile conversion rate.
Increase investment in Google Search campaigns.
Reduce refunds by improving product quality.
Promote high-profit products.
Plan marketing campaigns around seasonal sales trends.
📷 Dashboard Preview

Add your Power BI dashboard screenshots here.

Example:

Dashboard Overview
Sales Analysis
Customer Journey Analysis
📁 Project Structure
E-Commerce-Sales-Customer-Journey-Analysis
│
├── Dashboard Images
│   ├── Dashboard.png
│   ├── Sales Dashboard.png
│   └── Customer Journey.png
│
├── Power BI
│   └── Ecommerce Analysis.pbix
│
├── Dataset
│   └── Available through Google Drive
│
├── README.md
└── LICENSE
🎯 Conclusion

This project demonstrates how Excel, Power Query, Power BI, and DAX can transform raw e-commerce data into meaningful business insights. Interactive dashboards were developed to analyze revenue, profit, customer behavior, refunds, and marketing performance, enabling stakeholders to make informed business decisions.
