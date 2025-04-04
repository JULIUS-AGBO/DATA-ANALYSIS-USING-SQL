# DATA-ANALYSIS-PROJECT-USING-SQL
This report analyzes the sales performance of a company's products across different regions and time periods.

## PROJECT OVERVIEW 

#### This project aims to provide actionable insights into a company's sales performance, customer behavior, and product trends. Leveraging SQL queries, we will analyze a comprehensive dataset to answer critical business questions. The insights gained from this analysis will enable data-driven decision-making, optimize business strategies, and drive growth. By exploring key metrics, trends, and correlations, we will uncover opportunities to enhance customer satisfaction, improve sales performance, and increase revenue.

## DATA SOURCES

#### The primary data source is the "Sample_Superstore.csv" file, containing sales transactions with variables like sales amounts, profits, product info, customer demographics, geographical details, e.t.c. This dataset will be analyzed to uncover insights into sales trends, customer behavior, and product performance.

## TOOL/DATA CLEANING & PREPARATIONS

#### SQL Server

## INSIGHTS TO BE QUERIED

 - Total Revenue by Region: What is the total revenue generated by each region?
 - High-Value Products: Which products have a sales amount greater than 10,000?
 - Average Order Value by Segment: What is the average order value for each customer segment?
 - Frequent Customers: Which customers have placed more than 5 orders?
 - Product Sales Ranking: What is the ranking of products by sales amount?
 - Multicategory Customers: Which customers have purchased products from multiple categories?
 - Sales Region Performance: What is the total revenue generated by each sales region, including the region name and sales amount?
 - High-Performing Products: Which products have a higher sales amount than the average sales amount of all products?
 - Segment Revenue: What is the total revenue generated by each customer segment, including the segment name and revenue amount?
 - High-Value Orders: Which customers have placed orders with a total value greater than 10,000?

## DATA ANALYSIS 

### Total Revenue by Region: What is the total revenue generated by each region?

#### To analyze the total revenue by region, the following SQL statement will be used; 

#### SELECT region, SUM(Profit) AS Total Profit FROM Superstore GROUP BY region and Round to one decimal place.

```sql

use sales_data;
select * from superstore;

SELECT Region, round(sum(Profit), 1) AS `Total Profit`
FROM Superstore
GROUP BY region;

```

### RESULTS/FINDINGS

#### The SQL query SELECT region, SUM(profit) AS Total Profit FROM Superstore GROUP BY region; reveals the total profit per region. 
The results shows each profit as
- West: $106,021.10 (highest profit)
- East: $90,672.00
- South: $46,035.70
- Central: $40,128.90 (lowest profit)

This analysis provides valuable insights into regional profit distribution, highlighting the West as the most profitable region and the Central region as the least profitable.

## RECOMMENDATIONS

## CONCLUSION

