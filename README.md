# 📊 Sales Trend Analysis Using SQL Aggregations

## 📝 Overview
This project performs monthly sales trend analysis using SQL to extract and summarize **revenue** and **order volume** from a dataset containing online sales data.

- **Database Used**: MySQL (compatible with PostgreSQL and SQLite)
- **Dataset Table**: `online_sales.orders`
- **Objective**: Extract total revenue and order count per month for trend analysis.

---

## 🧩 Dataset Structure

The table `orders` contains the following columns:

| Column Name  | Data Type | Description                      |
|--------------|-----------|----------------------------------|
| `order_id`   | INT       | Unique identifier for each order |
| `order_date` | DATE      | Date when the order was placed   |
| `amount`     | DECIMAL   | Revenue amount for the order     |
| `product_id` | INT       | ID of the purchased product      |

---


    YEAR(order_date),
    MONTH(order_date)
ORDER BY
    YEAR(order_date),
    MONTH(order_date);
