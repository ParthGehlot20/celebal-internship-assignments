# 🛒 E-Commerce Sales Data Engineering & Analysis

**Author:** Parth Gehlot  
**Context:** Celebal Technologies Summer Internship 2026 - Week 2 Task  

## 📋 Project Overview
This repository contains a data engineering and business intelligence project focused on analyzing e-commerce sales data. The objective is to ingest raw transactional data (the classic Superstore dataset) into a relational database and perform SQL-based analysis to uncover actionable business insights regarding customer behavior, regional performance, and product profitability.

## 🛠️ Tech Stack & Tools
* **Environment:** Linux (Fedora)
* **Language:** Python 3
* **Workspace:** Jupyter Notebook (`.ipynb`)
* **Database Engine:** SQLite (Local RDBMS)
* **Libraries:** `pandas` (for data ingestion & cleaning), `sqlite3` (for database connection and querying)

## 📁 Repository Structure
* `Task2_DataEngineering.ipynb`: The main Jupyter Notebook containing all Python/SQL code, query results, and markdown-based business insights.
* `Sample - Superstore.csv`: The raw dataset used for analysis (ensure this is in the same directory before running).
* `README.md`: Project documentation.

## 🚀 Key Objectives Achieved
1. **Data Ingestion:** Successfully loaded CSV data into a local SQLite database using Python and Pandas.
2. **Targeted Filtering:** Utilized `WHERE` clauses to isolate high-value segments (e.g., Technology sales in the West region).
3. **Categorical Aggregation:** Grouped data by categories to evaluate overarching metrics like Total Sales, Quantity, and Average Discounts.
4. **Performance Sorting:** Identified top-performing products and sub-categories using `ORDER BY` and `LIMIT`.
5. **Customer Analytics:** Extracted top VIP customers based on total profitability to drive retention strategies.
6. **Data Validation:** Verified data integrity post-ingestion by comparing SQL row counts against the source file.

