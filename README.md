# Tokyo Olympic Data Engineering Project

This data engineering project focuses on processing and transforming Tokyo Olympic datasets using Azure Data Factory (ADF) for initial data loading and Azure Databricks for subsequent transformations. The project involves loading datasets from GitHub to Azure Data Lake Storage Gen2, performing various data transformations in Databricks, and then loading the transformed data back to Azure Data Lake Storage Gen2.

## Project Overview

- **Data Sources:**
  - Original datasets are sourced from [GitHub repository](https://github.com/your-username/your-repository).
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
   - Calculated gender ratios and medal ratios for further analysis.

3. **Data Storage:**
   - Transformed DataFrames were repartitioned and stored back to Azure Data Lake Storage Gen2.

## Project Structure

- **Notebooks:**
  - `01_Data_Loading_with_ADF.ipynb`: ADF pipeline for initial data loading.
  - `02_Data_Transformation_with_Databricks.ipynb`: PySpark transformations in Databricks.
  - `03_Data_Storage_and_Quality_Checks.ipynb`: Storing transformed data and quality checks.

- **Scripts:**
  - `adf_pipeline.json`: ADF pipeline definition for data loading.
  - `databricks_job.py`: PySpark script for running transformations in Databricks.

- **Configuration:**
  - `configs.json`: Configuration settings used in ADF and Databricks.

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/your-repository.git
