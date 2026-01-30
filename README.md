# PostgreSQL Data Warehouse Project

Welcome to the **PostgreSQL Data Warehouse Project** repository! 🚀

This project showcases a complete data warehousing and analytics solution, including building a PostgreSQL data warehouse and generating insights from integrated data sources. It is intended as a portfolio project and demonstrates practical data engineering and analytics skills.

**Credits:** Project inspired by and based on content from *[Data with Baraa](https://youtu.be/9GVqKuTVANE)*.

---

## 📖 Project Overview

This project encompasses:

1. **Data Architecture**: Architecting a modern data warehouse utilizing the Medallion Architecture, structured into **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from disparate source systems into the warehouse.
3. **Data Modeling**: Crafting fact and dimension tables optimized for analytical querying.
4. **Analytics & Reporting**: Developing SQL-based reports and dashboards to derive actionable insights.
---

## 🛠️ Tools I Used

Everything is free!
- **[Datasets](datasets/)**: Access the project datasets (CSV files).
- **[PostgreSQL](https://www.postgresql.org/download/)**: Open-source relational database for hosting your data warehouse.
- **[VS Code](https://code.visualstudio.com/download)**: A go-to GUI for PostgreSQL database management and executing SQL queries.
- **[Notion Project Steps](https://shorturl.at/yMIZt)**: Access all project phases and tasks.

---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Goal
Build a PostgreSQL data warehouse that combines sales data for reporting and analysis.

### Tasks
- Load data from two CSV sources (ERP and CRM).
- Clean and handle data quality issues before analysis.
- Integrate both sources into a single, analytics-friendly data model.
- Use only the latest dataset (no historical tracking required).
- Document the data model for business users and analytics teams.

---

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver granular insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with critical business metrics, enabling strategic decision-making. 

---

## 🏗️ Data Architecture

The data architecture for this project adheres to the Medallion Architecture, comprising **Bronze**, **Silver**, and **Gold** layers:
1. **Bronze Layer**: Stores raw data in its original form from the source systems. Data is ingested from CSV files into the PostgreSQL database.
2. **Silver Layer**: Involves data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Hosts business-ready data modeled into a star schema for reporting and analytics.

![Data Architecture](docs/data_architecture.png)

---

---

## 📂 Repository Structure
```
PostgreSQL_Data_Warehouse_Project/
│
├── datasets/ # Raw datasets used for the project (ERP and CRM data)
│
├── docs/ # Project documentation and architecture details
│ ├── ETL_process.png # A diagram created in Draw.io showing ETL techniques and methods used in this project
│ ├── data_architecture.png # A diagram created in Draw.io showing the project's architecture
│ ├── data_catalogue.md # Catalog of datasets, including field descriptions and metadata
│ ├── data_flow.png # A diagram created in Draw.io for the data flow diagram
│ ├── data_integration_model.png # A diagram created in Draw.io that shows how tables are related to each other.
│ ├── gold_layer_data_model.png # A diagram created in Draw.io that shows gold layer data model (star schema)
│ ├── naming-conventions.md # Consistent naming guidelines for tables, columns, and files
│
├── scripts/ # SQL scripts for ETL and transformations
│ ├── bronze/ # Scripts for extracting and loading raw data
│ ├── silver/ # Scripts for cleaning and transforming data
│ ├── gold/ # Scripts for creating analytical models
│
├── tests/ # Test scripts and quality files
│
├── README.md # Project overview and instructions
├── LICENSE # License information for the repository
├── .gitignore # Files and directories to be ignored by Git
```
---


## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.
