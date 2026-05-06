# 🛒 Zepto Product Analysis — SQL + Power BI Project

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-blue)
![PowerBI](https://img.shields.io/badge/Dashboard-Power%20BI-yellow)
![Status](https://img.shields.io/badge/Status-Completed-green)
![Level](https://img.shields.io/badge/Level-Intermediate-orange)

---

## 📌 Project Overview

This project performs an end-to-end **data exploration, cleaning, business analysis, and visualization** on Zepto's grocery product catalog.

The project is divided into two parts:
- **Part 1 — SQL Analysis:** Data cleaning and business insights using PostgreSQL
- **Part 2 — Power BI Dashboard:** Interactive dashboard built on the same dataset

The goal was to extract meaningful business insights from raw product data — including pricing, discounts, stock availability, and inventory — to support data-driven decision making.

---

## 📊 Power BI Dashboard

### Dashboard Preview
![Zepto Dashboard](dashboard.png)

### Key Metrics (KPI Cards):
| Metric | Value |
|---|---|
| 💰 Total Revenue | ₹122.27M |
| 📦 Total Products | 4K |
| 🏷️ Avg Discount % | 7.62 |
| 🚫 Out of Stock Items | 453 |

### Visuals Built:
- 📊 **Bar Charts** — Top Categories by Revenue (product-wise)
- 🔲 **KPI Cards** — Total Revenue, Total Products, Avg Discount, Out of Stock
- 🎛️ **Slicer** — Filter by Category (Chocolates & Candies, Cooking Essentials, Home & Cleaning, Ice Cream & Desserts, Munchies, Paan Corner, Packaged Food, Personal Care)

### Top Products by Revenue:
1. Kellogg's Original Corn Flakes
2. Pedigree Puppy Dry Dog Food
3. Kellogg's Special K Original
4. Whiskas Kitten (2-12 months)
5. Godrej Yummiez Chicken Nuggets

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

## 🧹 Data Cleaning (SQL)

- Identified and removed products with **zero MRP**
- Checked and handled **NULL values** across all columns
- Converted pricing from **paise to rupees** using UPDATE
- Detected **duplicate product names** with multiple SKUs

---

## 📊 Business Questions Answered (SQL)

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
- Which products offer the **best value for money**?

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
├── dashboard.pdf         # Power BI dashboard screenshot
└── README.md             # Project documentation
```

---

## 💡 Key Insights

- 📦 Majority of products fall under **Low weight category** (< 1000g)
- 💸 Some high-MRP products have **very low discounts** — pricing opportunity
- 🚫 **453 products are out of stock** — potential revenue loss
- 🏷️ Categories with highest avg discounts offer best deals for customers
- 🥣 **Kellogg's & Pedigree** are top revenue-generating products

---

## 🔧 Tools Used

- **PostgreSQL** — Data cleaning & analysis
- **Power BI Desktop** — Dashboard & visualization
- **Excel** — Raw data source

---

## 👤 Author

**Kartik Saini**
📧 kartiksaini2800@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/kartiksaini28/)

---

## ⭐ If you found this project helpful, give it a star!
