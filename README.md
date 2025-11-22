**RetailDashboard**

This project is a complete Power BI sales analytics dashboard built using three datasets: Sales, Customers, and Products.
It includes data cleaning, data modeling, DAX measures, interactive visuals, and final dashboard formatting.

**1. Data Cleaning (Power Query)**

Performed the following data preparation steps:
1.Removed duplicates
2.Removed null values
3.Standardized column names
4.Corrected data types (Date, Text, Decimal, Whole Number)
5.Loaded cleaned data into the Power BI model

**2. Data Modeling (Relationships)**

Created a star schema with the following relationships:

From Table	To Table	Key	Type
Customers	Sales	CustomerID	1 : Many
Products	Sales	ProductID	1 : Many

All relationships are set to single-direction for optimal performance.

**3. DAX Measures**

Created custom measures for deeper business insights:

Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Profit Margin (%) = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Sales])) * 100

Total Orders = COUNT(Sales[OrderID])

Average Order Value = DIVIDE([Total Sales], [Total Orders])

**4.Dashboard Visualizations**
The dashboard contains the following visuals:
1.KPI Cards - Total Sales, Total Profit, Profit Margin (%), Total Orders

2.Charts
Bar Chart – Sales by Region
Donut Chart – Profit by Category
Line Chart – Monthly Sales Trend
Table – Top 10 Customers
Slicers – Region and Category

**5. Formatting & Design**
1.Custom light-blue theme applied
2.Professional spacing and alignment
3.All visuals include titles
4.Added creator name
5.Renamed page to Sales Dashboard
