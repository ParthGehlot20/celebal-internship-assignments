# Week 6 Spark Assignment - Celebal Technologies 🚀

## Overview
This repository contains the solution for the Week 6 PySpark assignment for the Data Engineering internship at Celebal Technologies. The project demonstrates core Apache Spark concepts, including architecture understanding, data manipulation, schema handling, and performance optimization using different execution modes and file formats.

## Objective
To understand and implement efficient data processing pipelines in Apache Spark by leveraging transformations, actions, and optimized storage formats.

## Key Concepts Covered
* **Spark Architecture:** Understanding the roles of the Driver, Cluster Manager, and Executors.
* **Lazy Evaluation & DAG:** How Spark optimizes execution plans using Lineage Graphs.
* **Data Processing:** Reading/writing files, schema inference, renaming columns, and casting data types.
* **Transformations vs. Actions:** Filtering, column selection, and mathematical operations (e.g., tax calculation).
* **Storage Formats:** Performance comparisons and practical implementation of CSV (row-based) vs. Parquet (columnar) files.
* **Optimization:** Utilizing Predicate Pushdown and avoiding memory bottlenecks (using `.show()` instead of `.collect()`).

## Prerequisites
* Python 3.x
* Apache Spark (PySpark)
* A Kaggle Notebook environment (or local Jupyter setup with PySpark installed)

## Repository Structure
* `Week6_Spark_Assignment.ipynb`: The main Kaggle notebook containing all PySpark code, dummy data generation, and markdown explanations for the 15 assignment questions.
* `data/source.csv`: Generated dummy dataset in CSV format (created programmatically within the notebook).
* `path/to/input/`: Generated dummy dataset in Parquet format.

## How to Run
1. Open the `Week6_Spark_Assignment.ipynb` notebook in Kaggle (or your preferred environment).
2. Run the first cell to install PySpark and generate the necessary dummy data. 
3. Execute the subsequent cells sequentially to view the transformations, filtered results, and schema adjustments.

## Author
**Parth Gehlot** Data Engineering Intern, Celebal Technologies