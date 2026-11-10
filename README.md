# Sales-Performance-Dashboard-Power-Bi-
Interactive sales performance dashboard built with HTML, CSS, JavaScript and Chart.js. Features KPI cards, dynamic filters (date, city, category, sales rep), 9 interactive charts, top/bottom product insights and drill-down detail pages. Responsive and loads data from Excel/CSV.
Sales Performance Dashboard | FY 2025 (Power BI)

A Power BI version of the Sales Performance Dashboard, built on the same 1,287-order sales dataset. It is a single-page report with KPI cards, slicers and 10 visuals.
What's in this folder:
File	Purpose:
Sales_Data_2025.xlsx	Source data
PowerQuery_Sales.m	Power Query (M) script: loads the data and sets data types
DAX_Measures.dax	Date table and all measures
SalesTheme.json	Blue colour theme (View > Themes > Browse for themes)
Build steps (about 20 minutes, Power BI Desktop)
Load data: Home > Transform data > New Source > Blank Query > Advanced Editor. Paste PowerQuery_Sales.m, change the file path, name the query Sales, then Close & Apply.
Date table: Modeling > New table. Paste the Calendar table from DAX_Measures.dax. Mark it as the date table, relate Calendar[Date] to Sales[Order_Date], and sort Month by Month No.
Measures: Create the measures from DAX_Measures.dax (Total Sales, Total Profit, Total Orders, Average Order Value, Profit Margin %).
Theme: View > Themes > Browse for themes > SalesTheme.json.
Enable cross-filtering (default) so every visual responds to the slicers, and add tooltips with Total Profit and Profit Margin %.
Tools:
Power BI Desktop, Power Query, DAX.
