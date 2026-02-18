# Sql_data_warehouse
A full end-to-end modern data warehouse project built using SQL Server, including ETL, data modeling, quality checks, and analytics.

Designed as a complete practical project to learn how real-world data warehousing works — from raw data ingestion to business data structures and reporting.

🚀 Project Summary

This repository demonstrates:

✔ Building a real, scalable SQL data warehouse
✔ Designing layered architecture
✔ Implementing robust ETL workflows
✔ Modeling data into facts and dimensions
✔ Adding data quality checks and testing
✔ Writing analytical queries for business insights

🧱 Tech Stack

Database: Microsoft SQL Server

Query Language: T-SQL

Optional Tools: Notion (for planning), draw.io (for diagrams), SQL Server Management Studio

🛠️ Architecture Overview

The project implements a layered data architecture:

Bronze — Raw Ingestion

Stores raw source data directly as ingested (e.g., CSV, flat files).

Silver — Cleansed & Transformed

Applies cleansing, formatting, deduplication, and integration logic to prepare data for analysis.

Gold — Business-Ready Schema

Data is modeled into fact tables and dimension tables optimized for analytics and reporting.

🔄 How ETL Works

Extract:
Pulled raw data from multiple sources (CSV files)

Transform:
Clean, normalize, deduplicate, and enrich raw data. Build business-oriented objects.

Load:
Store the cleaned datasets into staged tables and then into the final models (facts/dimensions).

📋 Data Quality Checks

Quality verification scripts are included to:

Identify NULLs

Detect duplicates

Validate date ranges

Check data integrity after each ETL layer

Quality queries are stored separately to keep ETL logic modular and testable.

🧠 Data Modeling

The Gold layer uses dimensional modeling:

✔ Fact tables – store numeric metrics
✔ Dimension tables – store descriptive attributes
✔ Star schema for query performance and easier analytics

Examples:

Fact_Sales (SaleID, DateKey, CustomerKey, ProductKey, Amount)
Dim_Date (DateKey, Year, Month, Day)
Dim_Customer (CustomerKey, Name, Region)
Dim_Product (ProductKey, Category, Price)

📊 Analytics & Queries

This project includes ready-made analytical queries to answer business questions like:

Monthly revenue trend

Top customers by sales

Category performance analysis

Year-over-year growth

These illustrate how to turn warehouse data into business insights.

🧪 Testing & Quality Assurance

Test scripts validate each layer using SQL queries that:

Ensure no missing primary keys

Validate ranges and data types

Confirm relationships between fact and dimension tables

Automated quality checks make your ETL pipelines reliable and repeatable.

📍 Credits
This guide and project structure were inspired by a comprehensive SQL data warehouse tutorial that walks through building a warehouse from scratch, covering architecture, ETL, modeling, testing, and analytics.

📄 License
MIT License
