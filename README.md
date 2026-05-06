# 🛒 Zepto Product Analysis — SQL Project

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-blue)
![Status](https://img.shields.io/badge/Status-Completed-green)
![Level](https://img.shields.io/badge/Level-Intermediate-orange)

---

## 📌 Project Overview

This project performs an end-to-end **data exploration, cleaning, and business analysis** on Zepto's grocery product catalog using **PostgreSQL**.

The goal was to extract meaningful business insights from raw product data — including pricing, discounts, stock availability, and inventory weight — to support data-driven decision making.

---

## 🗂️ Dataset

| Column | Description |
|---|---|
| `sku_id` | Unique product ID |
| `category` | Product category |
| `name` | Product name |
| `mrp` | Maximum Retail Price |
| `discountPercent` | Discount percentage |
| `availableQuantity` | Stock available |
| `discountedSellingPrice` | Final selling price |
| `weightGms` | Product weight in grams |
| `outOfStock` | Stock status (true/false) |
| `quantity` | Quantity |

---

## 🧹 Data Cleaning

- Identified and removed products with **zero MRP**
- Checked and handled **NULL values** across all columns
- Converted pricing from **paise to rupees** using UPDATE
- Detected **duplicate product names** with multiple SKUs

---

## 📊 Business Questions Answered

### 🔍 Data Exploration
- How many products are in the dataset?
- Which product categories exist?
- How many products are in-stock vs out-of-stock?
- Which product names appear multiple times?

### 💰 Pricing & Discounts
- Which are the **Top 10 best-value products** by discount %?
- Which **expensive products (MRP > ₹500)** have low discounts (< 10%)?
- Which **Top 5 categories** offer the highest average discounts?

### 📦 Inventory & Stock
- Which **high-MRP products (MRP > ₹300)** are currently out of stock?
- What is the **total inventory weight per category**?

### ⚖️ Weight & Value Analysis
- What is the **price per gram** for products above 100g?
- How are products grouped by weight — **Low / Medium / Bulk**?
- Which products offer the **best value for money** (lowest price per gram)?

### 📈 Revenue
- What is the **estimated revenue potential per category**?

---

## 🛠️ SQL Concepts Used

| Concept | Queries |
|---|---|
| DDL | CREATE TABLE, DROP TABLE |
| DML | INSERT, UPDATE, DELETE |
| Aggregations | SUM, COUNT, AVG, ROUND |
| Filtering | WHERE, HAVING |
| Grouping | GROUP BY, ORDER BY |
| Conditional Logic | CASE WHEN |
| Deduplication | DISTINCT |
| Subsets | LIMIT |

---

## 📁 Project Structure

```
zepto-sql-analysis/
│
├── zepto_analysis.sql    # All SQL queries
└── README.md             # Project documentation
```

---

## 💡 Key Insights

- 📦 Majority of products fall under **Low weight category** (< 1000g)
- 💸 Some high-MRP products have **very low discounts** — pricing opportunity
- 🚫 Several **premium products are out of stock** — potential revenue loss
- 🏷️ Categories with highest avg discounts offer best deals for customers

---

## 👤 Author

**Kartik Saini**
📧 kartiksaini2800@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/kartiksaini28/)

---

## ⭐ If you found this project helpful, give it a star!
