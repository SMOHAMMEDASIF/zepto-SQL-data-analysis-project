# 📈 SQL Data Analyst Portfolio Project — Zepto E-Commerce Inventory Insights

This is a complete **end-to-end Data Analytics project using SQL** based on an e-commerce inventory dataset from **Zepto (Quick Commerce)**. The project demonstrates real-world analytics skills — from importing raw data to generating insights that support business decision-making.

---

## 📌 Project Objective
To analyze product pricing, discounts, inventory availability and category-level performance to help understand:
- Which products offer the best value
- Which categories generate the highest revenue
- Which high-demand products are out of stock
- How pricing and weight impact consumer value

---

## 📁 Dataset Summary
The dataset represents Zepto’s product inventory across multiple categories.

| Column | Description |
|--------|-------------|
| sku_id | Unique product identifier |
| name | Product name |
| category | Product category |
| mrp | Maximum Retail Price (₹) |
| discountPercent | % discount on MRP |
| discountedSellingPrice | Price after discount (₹) |
| availableQuantity | Quantity in stock |
| weightInGms | Product weight in grams |
| outOfStock | TRUE/FALSE – product availability |
| quantity | Package quantity |

Duplicates occur because the same product exists in different sizes and weights — **common in e-commerce catalogs**.

---

## 🔧 Project Workflow

### 1️⃣ Database Setup
- Created SQL table with correct data types
- Imported the CSV dataset using pgAdmin into PostgreSQL

### 2️⃣ Data Exploration
- Count of records
- Sample preview of data
- Null value search
- Unique category extraction
- Stock vs out-of-stock comparison
- Duplicate product identification

### 3️⃣ Data Cleaning
- Removed records where MRP = 0 (invalid)
- Converted pricing fields from **paise to rupees**
- Checked consistency of numeric fields

### 4️⃣ Business-Focused SQL Insights
| Business Question | SQL Insight Extracted |
|------------------|------------------------|
| Best value products | Highest discount % |
| Expensive products that are unavailable | Potential lost revenue |
| Estimated revenue per category | Selling price × available quantity |
| High-priced low-discount items | Pricing optimization |
| Best discount categories | Highest average discount |
| Value per gram | Price per gram ranking |
| Weight segmentation | Low / Medium / Bulk product categorization |
| Total inventory load | Weight × available quantity |

---

## 🧠 Key Insights
🔹 Some categories offer **very high discounts**, signalling promotional push or excess stock  
🔹 **High-MRP products out of stock** could hurt revenue opportunity  
🔹 **Price-per-gram calculation** helps identify customer value products  
🔹 **Category-level revenue** shows which SKUs are the major contributors

---

## 📜 Tech Stack
| Tool | Purpose |
|------|---------|
| PostgreSQL | Database |
| pgAdmin | SQL Query Execution |
| CSV | Source Data |

---

## 🚀 How to Use This Repository
1. Clone the repository  
2. Create a PostgreSQL database  
3. Import the CSV file  
4. Run the SQL file (`Zepto_SQL_data_analysis.sql`)  
5. Explore and modify the queries for deeper analysis

---

## 👤 About the Author
**Sunkesula Mohammed Asif**  
Data Analyst | SQL | Power BI | Excel | Python

Passionate about deriving insights from data and solving real business problems using analytics.

📌 *If you find this project useful, don’t forget to star ⭐ the repository.*

---

### 📩 Future Scope
- Power BI dashboard for revenue & pricing analytics  
- Excel dashboard for category performance metrics  
- Python automation with PostgreSQL  

---
