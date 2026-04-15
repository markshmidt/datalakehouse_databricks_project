# Data Lakehouse Project (Databricks + PySpark)

## Overview
This project implements a modern **Data Lakehouse architecture** using **Databricks and PySpark**, following the **Medallion (Bronze → Silver → Gold) pattern**.

It demonstrates how to build scalable data pipelines using:
- Distributed processing (PySpark)
- Notebook-based development
- Automated workflows (job orchestration)
<img width="784" height="213" alt="image" src="https://github.com/user-attachments/assets/9cdfc626-c018-4713-b13f-c4dd2b6ee583" />

---

## Architecture (Medallion Design)

### Bronze Layer (Raw Ingestion)
- Raw data ingested from source systems
- Stored as-is (no transformations)
- Schema applied minimally
- Supports reprocessing

Example:
```bronze/
Bronze Layer.ipynb
```


---

###  Silver Layer (Clean & Transform)
- Data cleaning and validation
- Handling missing values
- Deduplication
- Standardization of formats

Example:
```
silver/
Silver_crm_cust_info.ipynb
Silver_crm_prd_info.ipynb
Silver_crm_sales_details.ipynb
Silver_erp_cust.ipynb
Silver_erp_px.ipynb
silver_orchestration.ipynb

```
---

### Gold Layer (Business & Analytics)
- Business-level transformations
- Creation of dimension and fact tables
- Star schema modeling

Example:
```
gold/
Gold_customers.ipynb
Gold_products.ipynb
Gold_fact_sales.ipynb
gold_orchestration.ipynb
```

---

## Tech Stack

- Databricks Lakehouse
- PySpark (Data processing)
- Databricks Notebooks
- Databricks Workflows (job orchestration)
- Delta Lake (storage format)

---

## Key Concepts Applied

### Lakehouse Architecture
- Combines data lake + data warehouse
- Supports both analytics and scalability

---

### Medallion Architecture
- Bronze → Silver → Gold data refinement
- Clear separation of responsibilities

---

### ⚡ PySpark Transformations
- Distributed data processing
- DataFrame API usage
- Efficient large-scale data handling

---

### Star Schema Modeling
- Dimension tables (customers, products)
- Fact table (sales)
- Optimized for analytics queries

---

### Workflow Automation
- Orchestrated notebook execution
- Dependency-based pipeline execution:

Bronze → Silver → Gold

---

## Use Cases

- Business reporting
- Data analysis
- Machine learning pipelines
- Dashboarding tools (Power BI / Tableau)

---

## Challenges & Learnings

- Understanding distributed processing with PySpark
- Managing dependencies between notebooks
- Designing clean data pipelines
- Structuring Medallion architecture correctly
- Debugging workflow execution issues

---

## Key Takeaways

- Built scalable **Lakehouse architecture**
- Implemented **real-world ETL pipelines**
- Learned **PySpark transformations**
- Applied **modern data engineering patterns**
- Automated workflows end-to-end

---

## Author
Mariia Shmidt

---

## Inspiration
- Data Engineering best practices
- Medallion Architecture
- Databricks documentation
