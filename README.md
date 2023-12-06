# Project Name: Realtime-Data-Processing-ETL-Pipeline
## Table of Contents
- [Introduction](#introduction)
- [Architecture Overview](#architecture-overview)
- [Key Learning Points](#key-learning-points)
- [Getting Started](#getting-started)

## Introduction

Welcome to the Realtime Data Processing Pipeline project, a comprehensive guide to building a robust end-to-end data engineering solution. This project will take you through the entire process, from data ingestion to processing and storage, utilizing a powerful technology stack including Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, Cassandra, and PostgreSQL. To simplify deployment and enable scalability, the entire system is containerized using Docker.

## Architecture Overview

![System Architecture](https://github.com/AbdellahAmini/Realtime-Data-Processing-ETL-Pipeline/blob/main/Architecture-Diagram.jpg)

The project encompasses the following components:

- **Data Source**: Utilizes the `randomuser.me` API to generate random user data, serving as our data source.
- **Apache Airflow**: Orchestrates the pipeline and stores fetched data in a PostgreSQL database.
- **PostgreSQL Database**: Stores original data to provide backup and safeguards against potential data loss or in the event of changes to the expected output of the project.
- **Apache Kafka and Zookeeper**: Facilitates real-time data streaming from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Enables monitoring and schema management of Kafka streams.
- **Apache Spark**: Employs data processing capabilities with master and worker nodes.
- **Cassandra**: Serves as the storage solution for processed data.

## Key Learning Points

Throughout this project, you will gain valuable experience in:

- Setting up a data pipeline using Apache Airflow.
- Implementing real-time data streaming with Apache Kafka.
- Utilizing distributed synchronization with Apache Zookeeper.
- Applying data processing techniques with Apache Spark.
- Leveraging data storage solutions with Cassandra and PostgreSQL.
- Containerizing the entire data engineering environment with Docker.



## Getting Started

Follow these steps to kickstart your journey with the Realtime Data Processing Pipeline project:

1. Clone the project repository:
    ```bash
    git clone https://github.com/your-username/realtime-data-processing-pipeline.git
    ```

2. Navigate to the project directory:
    ```bash
    cd realtime-data-processing-pipeline
    ```

3. Deploy the services using Docker Compose:
    ```bash
    docker-compose up
    ```

