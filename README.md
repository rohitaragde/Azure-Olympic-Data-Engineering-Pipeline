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
1. **Data Source**: The source of the data is the 2021 Olympics dataset hosted on Kaggle.
2. Storage Accounts Setups:
3. Resource Groups and Linked Services: 
4. **Data Ingestion (Azure Data Factory)**: Data is ingested from Kaggle to Azure Data Factory, where it is prepared for further processing.
5. **Raw Data Storage (Azure Data Lake Gen2)**: The ingested raw data is stored in Azure Data Lake Gen2 for easy access and management.
6. **Data Transformation (Azure Databricks)**: Data is transformed using Azure Databricks, where various operations are applied to clean and structure the data.
7. **Transformed Data Storage (Azure Data Lake Gen2)**: The transformed data is then stored back in Azure Data Lake Gen2 for further analysis.
8. **Analytics (Azure Synapse Analytics)**: The data is analyzed using Azure Synapse Analytics to generate insights.
9. **Visualization (Power BI and Tableau)**: The final insights are visualized using Power BI and Tableau for better representation and decision-making.

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
The first step in the pipeline is setting up Azure Storage Accounts, which provide a secure and scalable environment for storing large amounts of data.

![Storage Account](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/storage_account.png)
![Storage Container](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/storage_container_final.png)

### Linked Services and Resource Groups
linked services and resource groups are configured in Azure to manage the connections between different services used in the project. Make sure to setup the linked services and resource groups wherver required during the pipeline execution steps:-

![Linked Services](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/linked_services.png)
![Resource Groups](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/resource_groups.png)

### Data Ingestion
Once the storage account is set up, data is ingested from Kaggle to Azure Data Factory. The ingestion process allows for the automated transfer of CSV files to Azure.

![Data Factory Pipeline](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/data_ingestion_pipeline.png)

### Raw Data Storage (Azure Data Lake Gen2)
After ingestion, the raw data is stored in Azure Data Lake Gen2, which serves as a central repository for unstructured and structured data.

![Raw Data Post Ingestion](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/raw_data_post_ingestion.png)

### Data Transformation (Azure Databricks)
The raw data is then processed and transformed using Azure Databricks, where data cleaning, normalization, and other transformation tasks are performed.

![Azure Databricks Transformation Setup](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/azure_databricks_transformation_setup.png)

### Transformed Data Storage (Azure Data Lake Gen2)
The transformed data is stored back in Azure Data Lake Gen2, making it ready for analytics and further processing.

![Transformed Data Post Transformation](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/transformed_data_post_transformation.png)

### Analytics (Azure Synapse Analytics)
The stored data is analyzed using Azure Synapse Analytics, which provides powerful analytics capabilities to derive insights from the data.

![Tokyo Synapse Analytics](https://github.com/rohitaragde/azure-de-olampics-data/blob/master/images/tokyo_synapse_analytics.png)


## Insights and Analytics
## Insights and Analytics

1. **Number of Athletes from Each Country**:
   - This analysis reveals the total number of athletes representing each country at the 2021 Tokyo Olympics, ranked by their participation.
   - **Insight**: Countries with a larger number of athletes may indicate stronger investment in sports and a more robust athletic development infrastructure. This data reflects the country's size, population, and overall sports culture.

2. **Total Medals Won by Each Country**:
   - This analysis aggregates the total number of gold, silver, and bronze medals won by each country, allowing for a comparative understanding of their success in the Olympics.
   - **Insight**: A higher total medal count suggests a country’s strength across various sports. This data can also highlight specific areas where a country excels and may guide future sports funding and development initiatives.

3. **Average Number of Entries by Gender for Each Discipline**:
   - This analysis evaluates the average number of male and female entries for each Olympic discipline, providing insights into gender representation in different sports.
   - **Insight**: Understanding gender participation can identify sports with disparities between male and female athletes, informing efforts to promote inclusivity and gender equity in athletics.

### Summary of Insights:
- The **athlete count** provides a snapshot of the sporting strength and investment level of various countries.
- The **medal tally** serves as a key performance indicator, reflecting each country’s competitive edge in specific sports disciplines.
- The **gender entry averages** highlight participation trends and can guide initiatives aimed at increasing female or male representation in various sports.

## Future Enhancements
### Future Considerations:
- Further exploration could involve examining the relationship between the number of athletes and medal success to uncover patterns in Olympic performance.
- Investigating the impact of funding, training programs, and government support on athlete performance and participation could yield additional valuable insights.

## Steps to execute the project
- Clone the repository
- Make sure to have azure account with all the required access
- Setup the storage account and all the relevant linked services and resource groups
- execute the pipeline and all the other relevant Azure services and finally perform the analysis


## Contributors
Rohit Annasaheb Ragde

## Credits:-
Darshil Parmar
