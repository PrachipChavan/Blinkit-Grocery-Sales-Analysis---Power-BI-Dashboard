# Blinkit Grocery Sales Analysis- Power-BI Dashboard
This project is a comprehensive Data Analysis and Visualization exercise using Microsoft Power BI. The goal was to analyze the sales performance of Blinkit (India's quick-commerce grocery delivery service) by developing an interactive dashboard. The dashboard provides actionable insights into sales trends, product performance, outlet efficiency, and customer preferences.

🎯 Business Problem & Objectives
Blinkit needs to understand its sales dynamics across various outlets and product categories to optimize inventory and improve profitability. The primary objectives of this dashboard are:

Track Key Performance Indicators (KPIs): Monitor Total Sales, Average Sales per transaction, Total Items Sold, and Average Customer Rating.
Analyze Product Performance: Understand which item categories (e.g., Fruits, Snacks, Dairy) generate the most revenue and how fat content impacts sales.
Evaluate Outlet Performance: Compare sales across different outlet sizes (Small, Medium, High), location tiers (Tier 1, 2, 3), and establishment years to identify growth trends.
🛠️ Tools & Technologies Used
Microsoft Power BI: For data modeling, DAX calculations, and interactive data visualization.
Power Query Editor: For data cleaning, transformation, and shaping.
Dataset: Simulated Blinkit grocery retail dataset (CSV format).
🔄 Data Pipeline & Transformation (Power Query)
Before visualization, the raw dataset underwent rigorous cleaning in Power Query:

Standardization: Cleaned the Item_Fat_Content column by mapping inconsistent entries (e.g., "LF", "low fat" to "Low Fat", and "reg" to "Regular").
Handling Missing Values: Addressed null values in the Outlet_Size column by applying appropriate logic (e.g., substituting with "Medium" or based on location tier).
Data Type Formatting: Ensured correct data types for accurate calculations (e.g., converting Sales to Currency/Decimal, Ratings to Decimal).
🧮 Data Modeling & DAX Measures
Custom DAX (Data Analysis Expressions) measures were created to build dynamic KPIs:

Total Sales: SUM(Blinkit_Grocery_Sales[Item_Outlet_Sales])
Average Sales: AVERAGE(Blinkit_Grocery_Sales[Item_Outlet_Sales])
Number of Items: COUNTROWS(Blinkit_Grocery_Sales)
Average Rating: AVERAGE(Blinkit_Grocery_Sales[Rating])
📊 Dashboard Visualizations & Features
The dashboard features a sleek, dark-themed UI adhering to Blinkit's brand colors (Vibrant Yellow and Forest Green). Key visuals include:

KPI Cards: Providing an immediate snapshot of high-level metrics.
Donut Chart (Fat Content Breakdown): Highlighting the sales proportion between Low Fat and Regular products.
Horizontal Bar Chart (Sales by Item Type): Ranking the top-performing product categories.
Line Chart (Sales Growth by Year): Illustrating the historical sales trajectory based on when outlets were established.
Interactive Slicers: Allowing users to dynamically filter the entire dashboard by Outlet Location, Outlet Size, and Item Type.

