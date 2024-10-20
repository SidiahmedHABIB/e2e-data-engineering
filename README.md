# Realtime Data Streaming | End-to-End Data Engineering Project

## Table of Contents
- [Overview](#overview)
- [System Architecture](#system-architecture)
- [Technologies](#technologies)
- [Getting Started](#getting-started)
- [License](#license)
- [MyLinks](#my-links)

## Overview
In today's fast-paced, data-driven world, real-time data streaming is crucial for handling large volumes of
data efficiently and making time-sensitive decisions. Whether it's live updates, monitoring system events, 
or analyzing clickstreams, businesses rely on the ability to collect, process, and store data as it flows in real time.

To explore this further, I developed an end-to-end data engineering pipeline that automates
the data ingestion, processing, and storage lifecycle using a scalable, modern tech stack. 
This project leverages a variety of technologies to streamline data workflows, making it ideal for 
both real-time and batch processing use cases.

## System Architecture

![System Architecture](pics/architecture.gif)

#### The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Helps in monitoring and schema management of our Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.
- **Doker**: For Containerizing our entire pipeline.

#### We can monitor these messages being sent to Kafka topic using Control Center.
**![Control Center](pics/controlcenter.gif)**


## Technologies

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/SidiahmedHABIB/e2e-data-engineering.git
    ```

2. Navigate to the project directory:
    ```bash
    cd e2e-data-engineering
    ```
3. Install packages:
    ```bash
    pip install airflow
    pip install kafka-python
    pip install spark pyspark
    pip install cassandra-driver
    ```
4. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## My Links
[![FaceBook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/habib.sidiahmed.5)   [![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sidi-ahmed-habib-18163220a/)