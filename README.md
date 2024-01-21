# Tokyo Olympic Data Engineering Project

This data engineering project focuses on processing and transforming Tokyo Olympic datasets using Azure Data Factory (ADF) for initial data loading and Azure Databricks for subsequent transformations. The project involves loading datasets from GitHub to Azure Data Lake Storage Gen2 using ADF, performing various data transformations in Databricks, and then loading the transformed data back to Azure Data Lake Storage Gen2.

## Project Overview

- **Data Sources:**
  - Original datasets are sourced from [GitHub repository](https://github.com/thapaSujit/Data-Engineering-Project-in-Azure---Olympic-Data/tree/main/Datasets).
  - Datasets include information on athletes, coaches, entriesgender, medals, and teams for the Tokyo Olympics.

- **Tools Used:**
  - Azure Data Factory (ADF) for initial data loading.
  - Azure Databricks for data transformation and analysis.
  - Azure Data Lake Storage Gen2 for storing both raw and transformed data.

## Project Workflow

1. **Data Loading with Azure Data Factory:**
   - Utilized Azure Data Factory to load raw datasets from GitHub to Azure Data Lake Storage Gen2.

2. **Data Transformation with Azure Databricks:**
   - Mounted data from Azure Data Lake Storage Gen2 to Azure Databricks.
   - Performed various transformations using PySpark in Databricks notebooks.
   - Cleaned data, handled null values, removed duplicates, and engineered new features.

3. **Data Storage:**
   - Transformed DataFrames were repartitioned and stored back to Azure Data Lake Storage Gen2.

## Scripts:
  - `adf_pipeline.json`: ADF pipeline definition for data loading.
  - `databricks_job.ipynb`: PySpark script for running transformations in Databricks.

