# 🚀 AdventureWorks Azure Data Engineering Project  
## End-to-End Cloud Data Pipeline | ADF | ADLS Gen2 | Databricks | PySpark | Synapse | Medallion Architecture

This project is a complete **modern data engineering pipeline** built using Microsoft Azure services.  
It demonstrates real-world ingestion, transformation, and analytics modeling based on the **AdventureWorks** dataset (Kaggle).

The solution follows the **Medallion Architecture** (Bronze → Silver → Gold) and uses technologies such as:  
**Azure Data Factory, Data Lake Gen2, Azure Databricks, PySpark, Synapse Analytics Serverless SQL, and Power BI.**

---

## 🏗️ **Architecture Overview**
### ✔ End-to-End Cloud Data Engineering Pipeline


---

## 🛠️ **Technologies Used**
- **Azure Data Factory (ADF)** – Data ingestion & orchestration  
- **Azure Data Lake Storage Gen2 (ADLS)** – Secure data storage  
- **Azure Databricks (PySpark)** – Transformations & processing  
- **Apache Spark** – Big data computation  
- **Azure Synapse Analytics** – SQL modeling & analytics  
- **Parquet Format** – Optimized storage format  
- **Python / SQL** – ETL logic  
- **Power BI (optional)** – Reporting layer  

---

## 📂 **Dataset Used**
Taken from Kaggle (Adventure Works Sales Dataset):


---

# 🥇 **Medallion Architecture Implementation**

## **1️⃣ Bronze Layer – Raw Data**
- Data is ingested directly into ADLS using **ADF pipelines**.
- No transformations performed.
- Files stored in `.csv` format.

**Purpose:** Preserve raw, unmodified source data.

---

## **2️⃣ Silver Layer – Cleaned & Transformed Data**
Transformations performed using **Azure Databricks + PySpark**:

- Schema correction & enforcement  
- Handling null & missing values  
- Derived columns (Month, Year, Date keys)  
- Joining product, subcategory, and category data  
- Combining 3-year sales files  
- Filtering invalid customer & product records  
- Writing using **Parquet format** (optimized)

**Purpose:** Create clean, analytics-ready datasets.

---

## **3️⃣ Gold Layer – Final Business-Ready Tables**


Purpose: Provide ready-to-consume models for BI & analytics.
