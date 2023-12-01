# Apache Hive Project

This project is a practical workshop for Apache Hive, guiding you through setting up Hadoop, Hive, loading data into Hadoop HDFS, and executing queries. The goal is to find the top 5 airlines with the greatest average DEPARTURE_DELAY.

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
