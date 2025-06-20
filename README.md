# 🚖 NYC Taxi Data Engineering Pipeline (Azure + Databricks)

📌 **Architecture Diagram**:  
![Architecture Diagram](https://github.com/shubhamsahu03/azure-nyc-taxi-pipeline/blob/main/architecture_design.png)


This project demonstrates a complete, production-grade Data Engineering pipeline using the **NYC Green Taxi dataset**, built with **Azure Data Factory**, **Azure Databricks**, **Delta Lake**, and **Power BI**. It’s designed to teach real-world skills including dynamic ingestion, medallion architecture, PySpark transformations, and secure cloud integration.

## 🔧 Tech Stack

- **Azure Data Factory** – Dynamic, parameterized pipelines
- **Azure Databricks** – PySpark transformations, Delta Lake
- **Azure Data Lake Gen2** – Scalable storage (bronze/silver/gold)
- **Delta Lake** – ACID compliance, versioning, time travel
- **Power BI** – Visualization layer for curated data
- **Azure AD + Service Principal** – Secure access management

## 🏗️ Architecture Overview

- **Bronze**: Raw `.parquet` data ingested from public API via ADF
- **Silver**: Cleaned & transformed data using PySpark
- **Gold**: Delta Lake tables with ACID properties and query support
- **Power BI**: Connected to gold tables for final analytics

## 📌 Key Features

- 📥 Real-time API ingestion (no manual uploads)
- 🔁 Looping & dynamic pipelines (months Jan–Dec)
- 📂 Recursive file reads & custom schemas
- 🧠 Delta Lake for schema enforcement, time travel, updates
- 🔐 Secure access using Managed Identity & Service Principal
- 📊 Integration with Power BI for reporting

## 🧪 What You’ll Learn

- Build dynamic data pipelines in ADF
- Perform efficient transformations in PySpark
- Manage Delta Lake version control and rollback
- Set up secure access with Azure Active Directory
- Serve data to BI tools from cloud-native environments

## 🗂️ Data Sources

- NYC Green Taxi Trip Records (via public API)
- Trip Type & Zone lookup CSVs (manually uploaded once)

---

