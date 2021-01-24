# Airflow

This project is used for running data pipelines. Each pipeline is defined as a DAG (direct acyclic graph) and each job is defined as a task.
All DAGs definitions are under the `dags` directory.

## Usage

Run the project locally as follows:
Create the image
```sh
docker build -t jdaareval/docker-airflow:0.1.0 .
```
Upload the containers
```sh
docker-compose -f "docker-compose.yml" up -d
```
This will run a postgres and airflow containers (ports 5432 and 8080 accordingly)

