# Aidetic_Assesment_Test

# Data Pipeline for Clickstream Analysis

This project implements a data pipeline for ingesting clickstream data from Kafka, storing it in a data store, processing the stored data using Apache Spark, and indexing the processed data in Elasticsearch. The pipeline performs aggregation based on URL and country, calculating the number of clicks, unique users, and average time spent on each URL by users from each country.

## Pipeline Steps
1. **Produce the data from the website:** produce the data from the website using web scraping and send it to the consumer through the kakfa producer. 
2. **Ingest clickstream data from Kafka:** The pipeline consumes clickstream data from a Kafka topic and extracts relevant information such as user ID, timestamp, and URL.

3. **Store the ingested data:** stored the data into RDBMS(postgres).

3. **Periodically process the stored clickstream data:** The stored clickstream data is periodically processed using Apache Spark. The pipeline aggregates the data by URL and country, calculating the number of clicks, unique users, and average time spent on each URL by users from each country.

4. **Index the processed data in Elasticsearch:** The processed data is indexed in Elasticsearch for efficient searching and analysis. The indexed data can be used to generate insights and visualizations.

## Tools and Technologies Used

The following tools and technologies are used to build the data pipeline:

- Apache Kafka: For data ingestion from the clickstream source.
- Data storage and processing: Choose a suitable data store for storing the clickstream data and Apache Spark for data processing and aggregation.
- Elasticsearch: For indexing and searching the processed clickstream data.


## Report

For a detailed summary of the approach, assumptions, and pipeline components, please refer to the [report.md](report.md) file.

