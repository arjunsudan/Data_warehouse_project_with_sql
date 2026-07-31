# Data Warehouse & Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates an end-to-end data warehousing and analytics solution—from building a scalable data warehouse to deriving actionable business insights. Designed as a portfolio project, it showcases industry best practices in data engineering, data modeling, and business intelligence.

---

## 🏗️ Data Architecture

The architecture follows the **Medallion Architecture** pattern across **Bronze**, **Silver**, and **Gold** layers:

![Data Architecture](docs/data_architecture.png)

1. **Bronze Layer**: Stores raw, ingested data as-is from source systems (CSV files ingested into a SQL Server database).
2. **Silver Layer**: Handles data cleansing, standardization, and normalization to prepare data for downstream consumption.
3. **Gold Layer**: Delivers business-ready data modeled into a star schema optimized for reporting and analytics.

---

## 📖 Project Overview

Key components of this project include:

1. **Data Architecture**: Designing a modern data warehouse using the Medallion Architecture pattern.
2. **ETL Pipelines**: Extracting, transforming, and loading data seamlessly across layers.
3. **Data Modeling**: Developing dimensional models (fact and dimension tables) tailored for analytical queries.
4. **Analytics & Reporting**: Writing SQL queries and constructing dashboards to surface key metrics.

🎯 This repository serves as a practical blueprint for mastering and demonstrating skills in:
- SQL Development
- Data Engineering & Architecture
- ETL Pipeline Design
- Data Modeling (Star Schema)
- Data Analytics & BI Reporting

---

## 🛠️ Tools & Resources

All tools used in this project are free to access:

- **[Datasets](datasets/):** Project source datasets (CSV format).
- **[SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads):** Lightweight database engine hosting the data warehouse.
- **[SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16):** Graphical interface for managing database objects and executing queries.
- **[Git & GitHub](https://github.com/):** Version control and repository hosting.
- **[DrawIO](https://www.drawio.com/):** Diagramming tool for architecture, data models, and data flows.
- **[Notion](https://www.notion.com/):** Project management and task tracking.
- **[Notion Project Steps](https://app.notion.com/p/Data-Warehouse-Project-3ac63d1431868045a04dee83e4091783?source=copy_link):** Step-by-step walkthrough of all project phases.

---

## 🚀 Project Requirements

### Data Engineering (Data Warehouse Build)

#### Objective
Build a central data warehouse in SQL Server to consolidate sales data, support analytics, and drive data-informed decision-making.

#### Specifications
- **Data Sources**: Import data from two distinct source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Identify and clean data anomalies prior to analysis.
- **Integration**: Merge source datasets into a unified, user-friendly star schema model.
- **Scope**: Current state only (no historical tracking/SCD required).
- **Documentation**: Document data models thoroughly for both technical teams and business stakeholders.

---

### Data Analysis (BI & Reporting)

#### Objective
Write analytical SQL queries to deliver core metrics across three main domains:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

## 📊 SQL Analytics & Exploratory Data Analysis

Looking for the advanced analytical SQL queries, customer segmentation, and EDA performed on this Gold-layer Star Schema? 

👉 Check out the [SQL Exploratory Data Analysis Project Repository](https://github.com/arjunsudan/SQL_Exploratory_Data_Analysis_Project).

🛡️ License
This project is open-source under the MIT License. Feel free to use, modify, and build upon it with proper attribution.

🌟 About Me
Hi there! I'm Arjun Sudan, a passionate data analyst learner. I love diving into complex datasets, identifying hidden patterns, and translating raw data into meaningful, actionable insights.

---

## 📂 Repository Structure

```text
data-warehouse-project/
│
├── datasets/                 # Raw source datasets (ERP and CRM CSV files)
│
├── docs/                     # Project documentation and architectural diagrams
│   ├── etl.drawio            # ETL techniques and flow diagrams
│   ├── data_architecture.drawio # Data architecture overview
│   ├── data_catalog.md       # Data dictionary and metadata guidelines
│   ├── data_flow.drawio      # Data flow diagrams
│   ├── data_models.drawio    # Star schema data model design
│   └── naming-conventions.md # SQL & object naming standards
│
├── scripts/                  # SQL scripts for ETL transformations
│   ├── bronze/               # Ingestion scripts for raw data
│   ├── silver/               # Cleansing and standardization scripts
│   └── gold/                 # Gold layer modeling scripts
│
├── tests/                    # Data quality checks and testing scripts
│
├── README.md                 # Project introduction and usage guide
├── LICENSE                   # Project license
├── .gitignore               # Git untracked files configuration
└── requirements.txt          # Python/environment dependencies (if applicable)
