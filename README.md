# Coinlore-Pipeline

## Purpose
This project aims to build a comprehensive data pipeline for gathering cryptocurrency data from the Coinlore API. The dataset encompasses various metrics including rank, price, volume, market cap, etc. The gathered data will be transmitted to Kafka via the Coinlore topic, then consumed and stored in Azure Blob Storage. Using Azure Data Factory, the data will be moved from the blob storage to the data lake for further processing. Data transformation tasks will be performed with Databricks, after which the transformed data will be moved to Synaptics as a data warehouse. Additionally, the project leverages Power BI for intuitive data visualization, facilitating insightful analysis and informed decision-making processes.

## Architecture
![coinlore architecture](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/d6cf94ae-652b-4383-939e-2eca8ac7faa6)

## Data Flow
1. **Data Extraction:** Gather cryptocurrency data from the Coinlore API.
2. **Data Transmission:** Transmit the gathered data to Kafka via the Coinlore topic.
3. **Data Storage:** Store the transmitted data in Azure Blob Storage.
4. **Data Movement:** Utilize Azure Data Factory to move data from blob storage to the data lake.
5. **Data Transformation:** Perform data transformation tasks using Databricks.
6. **Data Warehousing:** Move transformed data to Synaptics as a data warehouse.
7. **Data Visualization:** Utilize Power BI for intuitive data visualization and analysis.

## Technologies Used
- **Coinlore API:** Source of cryptocurrency data.
- **Kafka:** Streaming platform for transmitting data in real-time.
- **Azure Blob Storage:** Storage solution for storing transmitted data.
- **Azure Data Factory:** Orchestration tool for data movement tasks.
- **Databricks:** Platform for performing data transformation tasks.
- **Synaptics:** Data warehouse for storing transformed data.
- **Power BI:** Business intelligence tool for data visualization and analysis.

## Data Model
![Untitled](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/bd102de7-ed35-47d4-98e7-bce9fb8326cf)

## SQL Query
N/A

## Apache Airflow DAG
N/A

## View ETL
![Screenshot (25)](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/653e91aa-a6c0-459a-9d39-0e7af479ea46)

## Power BI Visualization
![coinlore project_page-0001](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/474f7871-f2f6-486d-a379-fed30c30c2f4)
![coinlore project_page-0002](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/c9729071-fdea-4983-808b-9f39615bb1ea)


## Development Setup
N/A

## Conclusion
N/A
