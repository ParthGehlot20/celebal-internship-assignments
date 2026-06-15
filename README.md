# Superstore Sales Analytics: Advanced SQL Queries

## 📌 Project Overview
This project involves a comprehensive data analysis of the Superstore dataset, demonstrating advanced SQL querying techniques. The assignment is built within a Jupyter Notebook environment using Python's `sqlite3` and `pandas` to act as an end-to-end data pipeline—transforming a flat CSV into a normalized relational database and extracting business insights.

## 🛠️ Tech Stack & Concepts
* **Environment:** VSCode, Jupyter Notebook
* **Languages/Libraries:** Python, Pandas, SQLite
* **Core SQL Concepts Used:**
  * Common Table Expressions (CTEs)
  * Window Functions (`RANK()`, `ROW_NUMBER()`, `PARTITION BY`)
  * Subqueries & Nested Queries
  * Data Normalization (`SELECT DISTINCT`)
  * `JOIN` operations and Aggregate Functions

## 🚀 Execution Steps
1. Clone this repository or download the project files.
2. Ensure you have the `Sample - Superstore.csv` file in the same directory as the notebook.
3. Open the `.ipynb` file in VSCode.
4. Run the cells sequentially. The first cell sets up an in-memory SQLite database, effectively bypassing the need to configure external database servers.

## 📊 Project Structure

### Step 1: Data Normalization
Imported the flat Superstore CSV and separated it into three distinct relational tables to ensure data integrity:
* `customers`
* `products`
* `orders`

### Step 2: Analytical Queries
Executed complex queries to uncover specific trends, including:
* Identifying orders exceeding average sales.
* Isolating the highest sales order per customer.
* Assigning sequence numbers to customer orders chronologically.
* Ranking the top customers utilizing `OVER()` and `PARTITION BY` clauses.

### Step 3: Final Combined View
A synthesized query utilizing `JOIN`, CTEs, and Window Functions simultaneously to output a clean ranking of all customers by their total lifetime sales volume.

### Mini Project: Customer Sales Insights
Derived specific business intelligence metrics:
* Top 5 and Bottom 5 revenue-generating customers.
* Identification of one-time buyers (single order customers).
* High-value clients (those consistently performing above the average sales threshold).