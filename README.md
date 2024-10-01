# Azure Olympic Data Engineering Project

## Introduction
This project implements a comprehensive data engineering pipeline for Olympic data using Microsoft Azure services. It demonstrates the end-to-end process of data ingestion, storage, transformation, analysis, and visualization of Olympic-related datasets.

## Project Overview
This project utilizes data from the 2021 Olympics in Tokyo, sourced from Kaggle. The dataset provides comprehensive information about the Tokyo Olympics, including details on athletes, coaches, events, and medal outcomes.

## Architecture
![Project Architecture](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/architecture.png)

The project leverages the following Azure services:
- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Databricks
- Azure Synapse Analytics
- Power BI

Data flows through the following stages:
1. Data Source
2. Data Ingestion (Azure Data Factory)
3. Raw Data Storage (Azure Data Lake Gen2)
4. Data Transformation (Azure Databricks)
5. Transformed Data Storage (Azure Data Lake Gen2)
6. Analytics (Azure Synapse Analytics)
7. Visualization (Power BI and Tableau)

## Technologies Used
- Microsoft Azure
- Python
- SQL
- Power BI
- Azure Data Factory
- Azure Databricks
- Azure Synapse Analytics

## Data Source
This project utilizes the following dataset from Kaggle:

- **Dataset**: [2021 Olympics in Tokyo](https://www.kaggle.com/datasets/arjunprasadsarkhel/images/2021-olympics-in-tokyo)

The dataset includes multiple CSV files covering various aspects of the Olympic Games:
- Athletes information
- Coaches details
- Gender-wise entries
- Medal statistics
- Team compositions

This rich dataset allows for in-depth analysis of the Tokyo Olympics, including performance metrics, country-wise comparisons, and gender distribution across events.

## Data Ingestion Pipeline (Kaggle to Azure Data Factory)
The data ingestion pipeline in Azure Data Factory includes the following datasets:
- Athletes
- Coaches
- EntriesGender
- Medals
- Teams

### Storage Accounts
![Storage Account](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/storage_account.png)
![Storage Container](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/storage_container_final.png)

![Data Factory Pipeline](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/data_ingestion_pipeline.png)

### Raw Data Storage (Azure Data Lake Gen2)
![Raw Data Post Ingestion](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/raw_data_post_ingestion.png)

### Data Transformation (Azure Databricks)
![Azure Databricks Transformation Setup](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/azure_databricks_transformation_setup.png)

### Transformed Data Storage (Azure Data Lake Gen2)
![Transformed Data Post Transformation](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/transformed_data_post_transformation.png)

### Analytics (Azure Synapse Analytics)
![Tokyo Synapse Analytics](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/tokyo_synapse_analytics.png)

### Linked Services and Resource Groups
![Linked Services](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/linked_services.png)
![Resource Groups](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/resource_groups.png)



