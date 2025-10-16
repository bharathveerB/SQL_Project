# Target E-commerce Analytics (SQL)

## 🎯 Project Overview

This project is a comprehensive **SQL data analysis** of a large Brazilian e-commerce dataset, designed to extract actionable business intelligence for a retail giant like **Target**. The primary objective was to move beyond basic reporting to answer strategic questions related to **growth trends, logistics performance, economic impact, and customer behavior**.

The analysis focuses on several key performance indicators (KPIs) to provide data-driven recommendations that can inform marketing, logistics, and pricing strategies in the Brazilian market.

## 🛠️ Tech Stack & Tools

* **Database Language:** SQL (Specifically formulated for **Google BigQuery** syntax, as seen in the uploaded queries, but easily adaptable to PostgreSQL/MySQL).
* **Data Source:** 8 distinct CSV files representing various facets of e-commerce operations.
* **Analysis Artifact:** `SQL_TARGET_QUERY.sql` (Contains all the complex queries used for analysis).
* **Visualization (Planned):** Tableau, Power BI, or Python (Matplotlib/Seaborn) for visualizing final results.

## 🗄️ 8 Core Datasets & Schema

The analysis relies on **8 relational tables** that detail the entire e-commerce flow, from product listing to customer review. These tables were loaded from the provided CSV files into a SQL database for querying.

| File Name | Description | Key Columns Used |
| :--- | :--- | :--- |
| `orders.csv` | The main log of all purchases, including timestamps, status, and delivery dates. | `order_id`, `customer_id`, `order_purchase_timestamp` |
| `customers.csv` | Customer demographics and location data. | `customer_id`, `customer_unique_id`, `customer_state` |
| `order_items.csv` | Details on products purchased, item price, and freight costs per item. | `order_id`, `product_id`, `price`, `freight_value` |
| `payments.csv` | Information on payment type, installment count, and total payment value. | `order_id`, `payment_type`, `payment_installments` |
| **`products.csv`** | Product metadata, including category and physical dimensions. | `product_id`, `product_category_name` |
| **`sellers.csv`** | Seller identification and location data. | `seller_id`, `seller_state` |
| **`order_reviews.csv`** | Customer satisfaction ratings and review dates. | `review_id`, `order_id`, `review_score` |
| **`geolocation.csv`** | Mapping of Brazilian zip codes to latitude/longitude coordinates. | `geolocation_zip_code_prefix`, `geolocation_lat`, `geolocation_lng` |

