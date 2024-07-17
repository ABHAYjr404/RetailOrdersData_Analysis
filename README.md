# Retail Orders Data Analysis

## About

This project involves extracting, transforming, and loading (ETL) data using Python and its libraries , followed by loading the processed data into Microsoft SQL Server. Subsequent analysis is performed to answer specific business questions as specified in the provided SQL file. This project aims to explore the Order data to understand top performing branches and products, sales trend of of different products, customer behaviour. The aims is to study how sales strategies can be improved and optimized. The dataset was obtained from the [Kaggle Retail Orders](https://www.kaggle.com/datasets/ankitbansal06/retail-orders).

## Purposes Of The Project

The major aim of this project is to:

* Efficiently extract and transform data.
* Load the transformed data into Microsoft SQL Server using SQLAlchemy library.
* Perform analysis to answer predefined business questions.

## Business Questions To Answer

1. find top 10 highest reveue generating products
2. find top 5 highest selling products in each region
3. find month over month growth comparison for 2022 and 2023 sales eg : jan 2022 vs jan 2023
4. for each category which month had highest sales
5. which sub category had highest growth by profit in 2023 compare to 2022

## Code

For the rest of the code, check the 'sql_queries.sql' file

```sql
-- Create table
create table df_orders (
	[order_id] int primary key,
	[order_date] date,
	[ship_mode] varchar(20),
	[segment] varchar(20),
	[country] varchar(20),
	[city] varchar(20),
	[state] varchar(20),
	[postal_code] varchar(20),
	[region] varchar(20),
	[category] varchar(20),
	[sub_category] varchar(20),
	[product_id] varchar(50),
	[quantity] int,
	[discount] decimal(7,2),
	[sale_price] decimal(7,2),
	[profit] decimal(7,2))
```
