
# LITA CAPSTONE PROJECT-Sale-Analysis-pro1

## Project Title- Sales Analysis
[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Datasets and tools used](#datasets-and-tools-used)

[Data Cleaning and Preparation](#data-cleaning-and-preparation)

[Exploratory Data Anaysis](#exploratory-data-analysis)

[Analysis](#analysis)


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
   - Find the sales transaction in each region.
   - Calculate the percentage of total sales contributed by each region.
     

### Analysis
---------------------
Sales trends:monthly,quarterly, and yearly trends
Product performance: Identifying best and worst selling products in each region,total revenue by product
Forecasting: Predict future sales using time series models. This is where we include some basic lines of codes or queries or even some of the DAX expressions used
during my analysis;
  ```SQL
SELECT * FROM [sales data lita]

  SELECT Product, SUM(Total_sales) FROM [sales data lita]
  GROUP BY Product

SELECT SUM(Total_sales) AS Sales_Transaction FROM [sales data lita]
GROUP BY Region

SELECT Product, MAX(Total_sales) AS Popular_product FROM [sales data lita]
GROUP BY Product

SELECT SUM(Total_sales) AS Total_Revenue FROM [sales data lita]
GROUP BY Product

SELECT SUM(Total_sales) AS Current_Yearsales FROM [sales data lita]
WHERE OrderDate >= '2024-01-01' AND OrderDate <= '2024-12-31'

SELECT Region,SUM(Total_sales) AS Region_sales, (CAST(SUM(Total_sales) AS float))/(SELECT SUM(Total_sales) FROM [sales data lita])* 100 AS Percentage
FROM [sales data lita]
GROUP BY Region

SELECT TOP 5(Customer_Id), SUM(Total_sales) AS Total_purchase
FROM [sales data lita]
GROUP BY Customer_Id
ORDER BY Total_purchase

```


![Sales Pivot](https://github.com/user-attachments/assets/b379bc74-70af-4079-a25a-7df539df2d3b)

![Sales Pivot](https://github.com/user-attachments/assets/c470ed32-ec5d-48f5-aee6-102eaccc2595)

![Sales Chart 1](https://github.com/user-attachments/assets/58c1ba5a-00f9-4fbc-b4dc-8be6da2b7992)

![Screenshot 2024-10-29 161023](https://github.com/user-attachments/assets/b3857dfb-5d6e-4088-b51b-97febec00615)


