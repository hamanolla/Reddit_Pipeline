# Overview

The primary goal of this pipeline is to serve as a learning experience and skill development opportunity while also providing assistance to others. Here's how the pipeline operates:

1.A single DAG (pipeline) is executed to fetch data from Reddit's API using Python's PRAW API wrapper. It collects data from the past 24 hours and stores it in a CSV file with various fields like post ID and author name. <br>

2.This CSV file is then loaded into an AWS S3 bucket, which is a cloud storage service. From there, it is transferred to AWS Redshift, a cloud-based data warehouse. <br>

3.The entire process is automated and managed by Apache Airflow, an orchestration tool, which is running within a Docker container. This eliminates the need for manual setup of Airflow. <br>

4.Two additional components of the project operate independently of Airflow. First, dbt is used to connect to the data warehouse and perform data transformations. This is primarily for skill-building and gaining familiarity with dbt. <br>

5.Second, a business intelligence (BI) tool is connected to the data warehouse, allowing for the creation of visualizations. Google Data Studio is recommended for this purpose, but other BI tools can be used if preferred. <br>
