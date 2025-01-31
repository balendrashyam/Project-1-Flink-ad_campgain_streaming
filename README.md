# Ad Tech Real-Time Data Analysis

## Overview
This project demonstrates a real-time data processing pipeline in the Ad Tech domain, utilizing a range of AWS services and technologies. The system processes streaming data using Apache Flink, performs transformations with Spark Streaming in AWS Glue, and stores results in Apache Iceberg tables on S3. The project is designed to process ad campaign data in real-time and enable analytics using AWS Athena.

### Tech Stack
- **Python**
- **Kinesis**
- **AWS Managed Flink**
- **Glue**
- **Spark Streaming**
- **Iceberg**
- **S3**
- **Glue Catalog**
- **Athena**

## Project Structure
The project includes the following key files and directories:
- **assembly/**: Contains files related to Flink job packaging.
- **target/**: Directory where compiled and packaged artifacts are stored.
- **application_properties.json**: Configuration file for application settings.
- **dependency-reduced-pom.xml**: POM file with reduced dependencies for Maven.
- **main.py**: Main Python script where the Flink application logic is defined.
- **mock_data_gen.py**: Script to generate mock data for testing purposes.
- **pom.xml**: Maven project configuration file.

## Features
- **Real-Time Data Processing**: Utilizes Apache Flink on AWS Managed Flink to ingest, process, and output real-time data streams.
- **Data Transformation with Spark**: AWS Glue jobs are used to consume, transform, and store data in Apache Iceberg tables.
- **Data Analysis with Athena**: AWS Athena is used to perform aggregation and analytics on transformed data stored in Glue Catalog.
- **Scalability**: The system is built for scalability using AWS services to handle large volumes of streaming data.

## Installation and Setup

### Prerequisites
- AWS account with necessary services (Kinesis, Flink, Glue, S3, Athena) configured.
- Python 3.x
- Maven installed locally for building Flink application.
- AWS CLI configured with appropriate access permissions.

### Steps to Set Up Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/balendrashyam/AdTech-RealTime-Data-Analysis.git
