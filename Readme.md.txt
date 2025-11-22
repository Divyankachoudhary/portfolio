Retail Sales Analysis – SQL + Power BI

A simple end-to-end project analyzing retail sales using SQL and Power BI. It includes KPI calculation, customer insights, category performance, profitability, and sales trends.

📌 Dataset Columns

transaction_id | sale_date | sale_time | customer_id | gender | age | category | quantity | price_per_unit | cogs | total_sale

🎯 Project Goals

Calculate key business KPIs

Analyze sales, customers, and categories using SQL

Build an interactive Power BI dashboard

Identify actionable business insights

📊 KPIs

Total Sales: 912K

Avg Profit

Total Transactions

Unique Customers

Avg Sale per Customer

Total Quantity Sold

🛠 Tools Used

SQL

Power BI

Power Query & DAX

📝 Key SQL Queries

Total Revenue

SELECT SUM(total_sale) FROM retail_sales;


Unique Customers

SELECT COUNT(DISTINCT customer_id) FROM retail_sales;


Category-wise Sales

SELECT category, SUM(total_sale) 
FROM retail_sales GROUP BY category;


Profit

SELECT (total_sale - cogs) AS profit FROM retail_sales;


Peak Sales Hour

SELECT HOUR(sale_time), SUM(total_sale) 
FROM retail_sales GROUP BY 1 ORDER BY 2 DESC;

📈 Insights

Electronics has the highest revenue & profit

46–60 age group purchases the most

Female customers spend slightly more

Q4 shows maximum sales

Beauty is the lowest-performing category

Evening hours have peak sales

📷 Dashboard Screenshot

(Add your dashboard image here)

![Dashboard](dashboard.png)

✔ Summary

A clean SQL + Power BI project showing data cleaning, analysis, dashboards, and business insights — ideal for data analyst portfolios.