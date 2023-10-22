# Reddit_Pipeline
A data pipeline designed to collect information from the r/dataengineering subreddit on Reddit. The end result is a Google Data Studio report that offers valuable insights into the official subreddit dedicated to the field of Data Engineering.

# Motivation
My unwavering motivation stems from my burning desire to take the data engineering expertise I've acquired and harness the capabilities of Looker Studio to create insightful visualizations. This drive fuels my determination to make data not just a resource but a powerful tool for informed decision-making.

# Architecture

![image](https://github.com/hamanolla/Reddit_Pipeline/assets/143839865/bde99af0-8d13-4a24-aa8a-ca30fb88064d)

1.Extract data using [RedditAPI](https://www.reddit.com/dev/api/) <br>
2.Load into [AWS S3](https://aws.amazon.com/s3/) <br>
3.Copy into [AWS Redshift](https://aws.amazon.com/redshift/) <br>
4.Transform using [dbt](https://www.getdbt.com/) <br>
5.Create [Google Data Studio](https://lookerstudio.google.com/u/0/navigation/reporting) Dashboard <br>
6.Orchestrate with [Airflow](https://airflow.apache.org/) in [Docker](https://www.docker.com/) <br>
7.Create AWS resources with [Terraform](https://www.terraform.io/)

# Output

<img width="1071" alt="image" src="https://github.com/hamanolla/Reddit_Pipeline/assets/143839865/1d8d3e9b-4458-463f-87dd-92b508a80684">


# Setup

As AWS offer a free tier, this shouldn't cost you anything unless you amend the pipeline to extract large amounts of data, or keep infrastructure running for 2+ months. However, please check AWS free tier limits, as this may change.
 
