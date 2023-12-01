# Apache Hive Project

This project is a practical workshop for Apache Hive, guiding you through setting up Hadoop, Hive, loading data into Hadoop HDFS, and executing queries. The goal is to find the top 5 airlines with the greatest average DEPARTURE_DELAY.

## Special attention

I was unable to upload the dataset here, so before starting the project, download the dataset from the Kaggle website

* (https://www.kaggle.com/datasets/usdot/flight-delays)

or via the link:

* (https://drive.google.com/file/d/1bHBFvkoPMj3MMNfJRh2rZVYXXWJaiCSc/view?usp=drive_link)

Next, move this dataset to the directory with this project.

## Prerequisites

- [Docker](https://www.docker.com/) installed
- [docker-compose](https://docs.docker.com/compose/install/) installed

## Getting Started

1. Clone this repository:

    git clone https://github.com/vladimirovich124/BD_Lab4_1

## Set up Docker containers:

    docker-compose up -d

This command downloads and launches Docker containers for Hadoop and Hive. Be patient; the setup may take some time.

## Run the project:

    ./run.sh
    
This script handles data loading, Hive table creation, and query execution to find the top 5 airlines with the greatest average DEPARTURE_DELAY.

## Project Structure
data/: Dataset for the workshop.
queries/: Hive query (top_airlines_query.hql)
scripts/: Bash script (copy_to_hdfs.sh) for copying data to HDFS.
docker-compose.yml: Docker Compose configuration.
run.sh: Bash script for project execution.

## Docker Configuration
docker-compose.yml: Defines services for Namenode, Datanode, Hive Server, Hive Metastore, and Postgresql Metastore.

## Environment Configuration
hadoop-hive.env: Environment variables for Hadoop and Hive configurations.
