# Elasticsearch Cluster with Traefik Load Balancer

This project contains a Docker Compose configuration file that launches an Elasticsearch cluster with 3 master nodes and a Traefik load balancer.

## Prerequisites

Before running the Docker Compose file, make sure you have the following prerequisites installed:

- Docker: [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)
- Docker Compose: [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/)

## Usage

To start the Elasticsearch cluster with Traefik load balancer, follow these steps:

1. Clone this repository

2. Navigate to the project directory

3. Start the Docker containers:

  ```shell
  docker compose up -d
  ```

4. Access Elasticsearch:

  - Elasticsearch master node 1: [http://localhost:9200](http://localhost:9200)

  Note: The Traefik load balancer will automatically distribute the requests to the Elasticsearch master nodes.

5. Access Kibana:

  - Kibana: [http://localhost:5601](http://localhost:5601)

## Configuration

You can customize the Elasticsearch cluster configuration by modifying the `compose.yml` file. Refer to the Elasticsearch and Traefik documentation for more information on available configuration options.