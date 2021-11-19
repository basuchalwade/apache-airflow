# Airflow Installation
## Using Production Docker Images
### Building the image
- Refer: https://airflow.apache.org/docs/apache-airflow/2.0.1/production-deployment.html

```
docker build . --tag "my-stable-airflow:0.0.1"
```

```
docker run -itd -p 8089:8080 --env "_AIRFLOW_DB_UPGRADE=true" --env "_AIRFLOW_WWW_USER_CREATE=true" --env "_AIRFLOW_WWW_USER_PASSWORD=admin" --name airflow_prod_02 my-stable-airflow:0.0.1 webserver
docker logs -f airflow_prod_02
docker exec -itd airflow_prod_02 airflow scheduler
docker ps
```

```
curl localhost:8089
# Login using admin/admin
```
