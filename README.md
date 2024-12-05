# Stock-Market-Real-Time-Data-Analysis-Using-Kafka

This repository is an end-to-end data engineering project focused on real-time stock market data analysis. The project utilizes Apache Kafka for real-time data streaming, AWS S3 for data storage, AWS Glue for data cataloging, and Amazon Athena for querying. The goal of the project is to simulate real-time stock market data streaming and perform analysis in an efficient, scalable architecture.

---

## Project Architecture

![Project Architecture](Architecture.jpg "Project Architecture") 

The architecture of this project is designed to handle and process real-time data efficiently using the following steps and technologies:

1. **Data Simulation**: The project starts with a pre-existing dataset, indexProcessed, which is simulated into a real-time streaming format. Using Python, random sampling and looping techniques send individual data points at specified intervals to mimic live data.

2. **Data Ingestion with Kafka**:
   - A **Kafka Producer** sends the simulated data to a **Kafka Broker**.
   - A **Kafka Consumer** reads the streamed messages from the broker for further processing.
   - **Apache Zookeeper** is used to manage the coordination between the producer, broker, and consumer, ensuring stability and fault tolerance.

3. **Data Storage**:
   - Processed and streamed data is stored in an **AWS S3 bucket**, allowing for scalable and cost-effective storage of data.

4. **Data Cataloging and Querying**:
   - An **AWS Glue Crawler** is configured to automatically detect the schema and crawl the data in the S3 bucket.
   - The crawled data is then available for querying through **Amazon Athena**, allowing for real-time insights into stock market trends and data analysis.

---

## Technologies Used

- **Python**: Scripting language used for creating Kafka producer and consumer scripts.
- **Apache Kafka**: Orchestrating real-time data streams
- **Amazon Web Services (AWS) Services**:  
  - **S3** for data storage  
  - **Amazon Athena** for SQL queries on data stored in S3  
  - **Glue Crawler** for data cataloging  
  - **Glue Catalog** as a central repository for metadata  
  - **EC2** for running my application

---

## Contact 

For any questions, feedback, or collaboration opportunities, feel free to contact me.

📧 **Email:** [lahbouchi.hanae@gmail.com](mailto:lahbouchi.hanae@gmail.com)
