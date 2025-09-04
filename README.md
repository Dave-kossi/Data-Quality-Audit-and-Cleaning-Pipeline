# 🧹 Data Quality Audit and Cleaning Pipeline

## 📌 Overview
This project implements a **Data Quality Audit and Cleaning Pipeline** designed to help data analysts, data scientists, and engineers quickly **assess and improve the quality of their datasets**.  

It performs two main tasks:
1. **Audit (Profiling)** – Generates a detailed HTML report *before and after cleaning* using [ydata-profiling](https://github.com/ydataai/ydata-profiling).  
2. **Cleaning** – Automatically removes duplicates, fixes column names, handles missing values, and standardizes data types.  

With this pipeline, users can **compare dataset quality before and after cleaning** and obtain both a cleaned dataset and two audit reports.  

---

## ⚙️ Features
- 📂 **Multi-format support**: CSV, Excel, JSON, Parquet, TXT  
- 🧾 **Audit reports**: interactive HTML reports before and after cleaning  
- 🧹 **Automated cleaning**:
  - Remove duplicates  
  - Normalize column names  
  - Convert data types (numeric, datetime)  
  - Handle missing values (median for numeric, `"unknown"` for text)  
- 💾 **Save cleaned dataset** in the same format as input  
- 🌐 **Automatic browser opening** for reports  

---

## 📊 Example on the *Online Retail* Dataset  

The pipeline was tested on the **Online Retail dataset**.  

### 🔍 Audit Before Cleaning  
[👉 View Report (HTML)](version_2_avant.html)  

Key observations before cleaning:
- Presence of **missing values** in several columns (e.g. `CustomerID`)  
- Multiple **duplicated rows** in the dataset  
- **Mixed or incorrect data types** (dates stored as strings, numeric columns with text noise)  
- **Inconsistent column naming conventions**  

### ✅ Audit After Cleaning  
[👉 View Report (HTML)](version_2_apres.html)  

Key improvements after cleaning:
- **Duplicates removed** → thousands of redundant rows dropped  
- **Missing values handled** → imputation strategies applied  
- **Column names normalized** → unified snake_case format  
- **Data types corrected** → e.g. `InvoiceDate` converted to datetime  

### ✨ Summary of Improvements
- Dataset size reduced with duplicates removed  
- Column naming consistency improved → easier for analysis and modeling  
- Missing values systematically treated  
- Profiling alerts significantly reduced, leading to **higher data quality**  

