# 🧹 Data Quality Audit and Cleaning Pipeline

## 📌 Overview
This project implements a **Data Quality Audit and Cleaning Pipeline** designed to help data analysts, data scientists, and engineers quickly **assess and improve the quality of their datasets**.  

It performs two main tasks:
1. **Audit (Profiling)** – Generates a detailed HTML report *before and after cleaning* using [ydata-profiling](https://github.com/ydataai/ydata-profiling).  
2. **Cleaning** – Automatically removes duplicates, fixes column names, handles missing values, and standardizes data types.  

This allows users to **compare dataset quality before and after cleaning** and obtain both a cleaned dataset and two audit reports.  

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

## 📊 Example Audit Reports  

The pipeline was tested on the **Online Retail dataset**.  

### 🔍 Before Cleaning  
[👉 View Before Cleaning Report (HTML)](version_2_avant.html)  

### ✅ After Cleaning  
[👉 View After Cleaning Report (HTML)](version_2_apres.html)  

### ✨ Key Improvements (Online Retail dataset)  
- **5,678 duplicates** removed  
- **3 columns** with missing values imputed  
- Column names normalized (e.g., `CustomerID` → `customer_id`)  
- Data types corrected (e.g., `InvoiceDate` converted to datetime)  


