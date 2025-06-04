# MySQL Business Intelligence Scripts

This repository contains two MySQL scripts designed to streamline Business Intelligence workflows:

---

## 🔁 1. Fiscal Quarter Function

### 📌 Function Name:
`get_fiscal_quater(date)`

### 📄 Description:
Returns the **fiscal quarter** (Q1–Q4) based on the input calendar date.

### 🗓 Fiscal Year Logic:
- Q1 = Sep–Nov
- Q2 = Dec–Feb
- Q3 = Mar–May
- Q4 = Jun–Aug

---

## 📊 2. Top-N Products Stored Procedure

### 📌 Procedure Name:
`get_top_n_product_per_division_by_sold_qty(in_fiscal_year INT, in_top_n INT)`

### 📄 Description:
Returns the **top N selling products** by quantity in each division for a given fiscal year.

### 🧠 Uses:
- Common Table Expressions (CTEs)
- DENSE_RANK for ranking within each division

### 🔍 Example:
```sql
CALL get_top_n_product_per_division_by_sold_qty(2021, 3);
# mysql-business_intelligence_scripts
MySQL UDF and Stored Procedure for Business Intelligence reporting
