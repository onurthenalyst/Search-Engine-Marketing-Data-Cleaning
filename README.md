# 📊 SEM Dirty Campaign Dataset  
SQL Data Cleaning Practice Project

---

## 📌 Overview

This dataset was programmatically generated using Python to simulate a realistic Search Engine Marketing (SEM) campaign export containing both clean and intentionally corrupted data.

The purpose of this dataset is to practice and demonstrate professional SQL-based data cleaning workflows.

File included:


Base rows generated: **1000**  
Final row count may vary due to structural manipulations and duplicates.

---

## 🗂 Dataset Structure

Columns:

- `keyword_text`
- `match_type` (exact / phrase / broad)
- `clicks`
- `impressions`
- `conversions`
- `cost_eur`
- `conversion_value`
- `quality_score`

The dataset simulates real SEM campaign performance metrics including impressions, CTR-driven clicks, CPC-based cost calculation, and conversion values.

---

## 🚨 Intentionally Injected Data Quality Issues

To replicate real-world marketing export problems, the following errors were deliberately introduced:

### 1️⃣ Missing Values
- NULL
- NaN
- Empty strings
- "N/A", "-"

### 2️⃣ Wrong Data Types
- Text instead of numeric values
- Mixed numeric-text values (e.g., `1O0`, `abc`)

### 3️⃣ Absurd / Out-of-Range Values
- `quality_score` = 99, 1000
- `clicks` = 999999
- Negative costs or metrics

### 4️⃣ Format Inconsistencies
- European comma decimals (e.g., `12,50`)
- Mixed decimal formats
- Embedded whitespace

### 5️⃣ Logical Errors
- clicks > impressions
- conversions > clicks

### 6️⃣ Special Character Corruption
- Tabs (`\t`)
- Line breaks (`\n`)
- Semicolons, pipes, hashtags
- Control characters inside values

### 7️⃣ Keyword-Level Issues
- Uppercase transformations
- Extra leading/trailing spaces
- Double spaces
- Underscores instead of spaces
- Empty keyword rows
- "NULL" as literal text
- Extra appended strings (e.g., `;extra`)

### 8️⃣ Structural Errors
- Extra columns
- Missing columns
- Duplicate rows

---

## 🎯 Project Purpose

This dataset is designed for:

- SQL data cleaning practice  
- Marketing analytics preprocessing  
- Data validation rule building  
- ETL testing  
- Junior data analyst portfolio projects  

It intentionally mimics messy exports from platforms like Google Ads.

---

## 🛠 Recommended Workflow

1. Import raw dataset  
2. Validate data types  
3. Detect NULL and malformed values  
4. Fix numeric formatting  
5. Apply logical validation rules  
6. Remove duplicates  
7. Create structured, analysis-ready tables  

---

## ⚠️ Disclaimer

This is a fully synthetic dataset generated using Python (Pandas & NumPy).  
It does not contain real advertising data.

---
