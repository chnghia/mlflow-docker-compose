# mlflow-docker-compose

Deploy an MLflow tracking server with docker compose.
MinIO S3 is used as the artifact store and MySQL server is used as the backend store.

## How to run

1. Clone (download) this repository

    ```bash
    git clone https://github.com/chnghia/mlflow-docker-compose.git
    ```

2. `cd` into the `mlflow-docker-compose` directory

3. Build and run the containers with `docker-compose`

    ```bash
    docker-compose up -d --build
    ```

4. Access MLflow UI with http://localhost:5000

5. Access MinIO UI with http://localhost:9000

## Containerization

The MLflow tracking server is composed of 4 docker containers:

* MLflow server
* MinIO object storage server
* MySQL database server

## Example

Following https://github.com/chnghia/mlflow-examples

## Thanks

Inprised https://github.com/sachua/mlflow-docker-compose