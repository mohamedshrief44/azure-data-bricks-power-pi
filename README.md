# 🧾 Retail Data Analytics using PySpark & Power BI

This project performs end-to-end retail data analysis using **PySpark** for data processing and **Power BI** for interactive visualization.  
The goal is to analyze transactions, products, stores, and customers to extract key business insights.

---

## 🚀 Project Overview

The notebook connects to **Azure Data Lake**, reads data from multiple parquet files, cleans and transforms it using **PySpark**, and then visualizes the results in **Power BI**.

---

## 🧩 Dataset Description

| Table | Description |
|--------|--------------|
| `transactions.parquet` | Contains sales transactions including product IDs, quantities, and total amounts |
| `stores.parquet` | Store information such as store name and location |
| `products.parquet` | Product details like name, category, and price |
| `customers.parquet` | Customer details such as ID, full name, email, and country |

All data is stored in Azure Data Lake and loaded using secure connection keys.

---

## ⚙️ Technologies Used

- 🐍 **PySpark** – for big data processing  
- ☁️ **Azure Data Lake Storage** – for storing parquet files  
- 📊 **Power BI** – for dashboard visualization  
- 🧮 **Python Libraries:**  
  - `pyspark.sql`
  - `pandas`
  - `matplotlib` (optional for local analysis)

---

## 🧠 Notebook Summary

File: `Untitled Notebook 2025-10-24 16_16_01.ipynb`

### Steps:
1. Configure Azure access using Spark configuration.
2. Load parquet data:
   ```python
   df_transaction = spark.read.parquet(".../transactions.parquet")
   df_store = spark.read.parquet(".../stores.parquet")
   df_product = spark.read.parquet(".../products.parquet")
   df_customer = spark.read.parquet(".../customers.parquet")


📈 Power BI Dashboard

The Power BI dashboard presents the summarized results from the PySpark analysis.

🔹 Dashboard Insights:

Smartwatch and Dumbbell Set are the top-performing products.

High Street Store achieved the highest total sales.

Most sales come from Egypt and Saudi Arabia.

The Electronics category dominates total revenue.
