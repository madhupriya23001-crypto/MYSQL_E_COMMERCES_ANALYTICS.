# MYSQL_E_COMMERCES_ANALYTICS.
Analyzed 20,000 e-commerce records using MySQL, applying normalization, joins, CTEs, window functions, and data cleaning to uncover sales trends and customer insights.
E-commerce Sales Analysis Using SQL
Project Overview
This project analyzes an e-commerce dataset containing 20,000 records using MySQL. It demonstrates SQL skills from beginner to advanced level and explores sales performance, customer purchasing patterns, product categories, order status, discounts, and ratings.
Dataset
The main table is orders and contains: order_id, customer_id, customer_name, city, product_name, category, quantity, unit_price, discount_percent, payment_method, order_date, order_status, and rating.
The dataset includes selected NULL values for data-cleaning practice.
Tools
MySQL 8.0+
MySQL Workbench
SQL
SQL Concepts Covered
SELECT, WHERE, ORDER BY, DISTINCT, and LIMIT
Filtering with LIKE, IN, and BETWEEN
NULL handling with IS NULL, IS NOT NULL, IFNULL, and COALESCE
String, numeric, and date functions
Aggregate functions, GROUP BY, and HAVING
CASE expressions and conditional aggregation
INNER JOIN, LEFT JOIN, RIGHT JOIN, SELF JOIN, and CROSS JOIN
UNION and UNION ALL
Subqueries and correlated subqueries
Common Table Expressions (CTEs), including recursive CTEs
Window functions: ROW_NUMBER(), RANK(), DENSE_RANK(), LAG(), and LEAD()
Views, temporary tables, indexes, and EXPLAIN
Transactions and data-quality checks
Database normalization concepts: 1NF, 2NF, and 3NF
Files
ecommerce_20000.sql — creates the database and populates the orders table with 20,000 records.
ecommerce_sql_project_queries.sql — contains 120 numbered SQL questions, queries, and practice challenges.
How to Run
Install MySQL 8.0+ and open MySQL Workbench.
Connect to your MySQL server.
Open and execute ecommerce_20000.sql.
Open ecommerce_sql_project_queries.sql.
Run the queries section by section. Some sections create supporting tables, views, or indexes; run those sections once or check whether the objects already exist.
Verify the dataset:
USE ecommerce_project;

SELECT COUNT(*) AS total_rows
FROM orders;
Expected result: 20000.
Database Normalization
For a normalized design, separate customer, product, category, order, and order-item data into related tables with primary and foreign keys. The supplied dataset starts as one denormalized orders table for SQL practice; data migration is required to turn it into a fully normalized schema.
Example Business Questions
Which product categories have the highest estimated net value?
Which cities have the most delivered orders?
Which payment methods are most common?
What percentage of orders are cancelled?
How do order volume and estimated net value change by month?
Which customers place the most orders?
Learning Goals
Practice SQL, improve relational database design skills, handle missing data, and generate business insights from e-commerce records.

