![Sales Pivot](https://github.com/user-attachments/assets/c470ed32-ec5d-48f5-aee6-102eaccc2595)
# LITA CAPSTONE PROJECT-Sale-Analysis-pro1

## Sales Analysis

### Project Overview
--------------
This project analyzes sales data to discover future trends, forcast future sales and provides actionable insights.
The datasets includes  information on customers transaction, products, quantity,total sales,region,unit price and date.
This data analysis project aims to generate insights into the sale performance of products in regions. By analyzing various parameter in the data received,
we seek to gather resonable decisions which then enables us to tell compelling stories around our data and to know the best performance from our data.

### Data Sources
----------------
The primary source of the data used here is Data sales.csv and this is an open source that was downloaded on Incubators hub LMS to carry out our projects.

### Datasets and tools used
--------------------------
The datasets used for this projects includes,region,date,unit price,quantity,total revenue.
1. Microsoft Excel-[Download Here](https://www.microsoft.com)
   for cleaning, for analysis, for data visualization.
3. SQL- [Download Here](https://www.microsoftsqlserver.com)
4. Structured Query Language for Querying the data.
5. PowerBI for data validation, quality and visualization presentation on dashboard.
6. GitHub for portfolio building

### Data Cleaning and Preparations
----------------------------
In the initial phase of the data cleaning and preparation, the following was performed;
1. Data loading and Inspection
2. Removing duplicates
3. Data cleaning and formatting
   ### Exploratory Data Analysis
   ----------------------------
   EDA involved the exploring of the data to answer some questions about the data such as;
   - Which products are the top sellers
   - What are the products on peak sales
   - Calculate monthly sales totals for current year.
   - Retrive the total sales for each product category.

### Analysis
---------------------
Sales trends:monthly,quarterly, and yearly trends
Product performance: Identifying best and worst selling products in each region,total revenue by product
Forecasting: Predict future sales using time series models. This is where we include some basic lines of codes or queries or even some of the DAX expressions used
during my analysis;
SELECT Product, SUM(Total_sales) FROM [sales analysis]
GROUP BY Product


![Sales Pivot](https://github.com/user-attachments/assets/b379bc74-70af-4079-a25a-7df539df2d3b)

