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

## Apache Airflow DAG
![carbon](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/54b5d247-3a8b-4dce-ba14-9ba06ee71cc5)
![carbon (1)](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/d84bb462-d1b4-49bc-99cd-16daa0a76fcb)
![carbon (2)](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/e3ea5cc5-4337-4161-bbda-d664328af2be)

## Transformation Append files (Databricks)
![vertopal com_coinlore append data_page-0001](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/1d8130e3-86d8-4733-a744-e9d48e5202e4)
![vertopal com_coinlore append data_page-0002](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/3ed61085-cf65-4e65-9819-36d1a1bd6faf)

## Transformation Processed files (Databricks)
![vertopal com_coinlore processed data_page-0001](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/9500e1d2-1375-475a-84cf-55e5ed49b1a8)
![vertopal com_coinlore processed data_page-0002](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/31b84734-a1d2-4f0c-ba38-a5708d92ea79)

## View ETL
![Screenshot (25)](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/653e91aa-a6c0-459a-9d39-0e7af479ea46)

## Power BI Visualization
![coinlore project_page-0001](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/474f7871-f2f6-486d-a379-fed30c30c2f4)
![coinlore project_page-0002](https://github.com/kingsley-123/Coinlore-Pipeline/assets/63650573/c9729071-fdea-4983-808b-9f39615bb1ea)


## Development Setup
To set up and run the cryptocurrency data pipeline locally, follow these steps:
- Install required Python packages (Pandas, Requests).
- Obtain access to the Coinlore API.
- Configure Kafka broker connection details.
- Set up Power BI for visualization (if not already installed).
- Set up Azure Data Factory for orchestration and scheduling of data pipeline workflows.
- Configure Azure Databricks for scalable data processing and transformations.
- Set up Azure Synapse Analytics for data warehousing and advanced analytics capabilities.
- Execute the Apache Airflow DAG to initiate the pipeline.


## Conclusion
This project aims to provide a comprehensive solution for fetching, transforming, and visualizing cryptocurrency data. By leveraging modern data technologies such as Kafka for streaming and Power BI for visualization, it enables real-time analysis and decision-making based on cryptocurrency metrics. The structured data pipeline ensures scalability and flexibility to accommodate future enhancements or additional data sources.
