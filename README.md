## MLFlow Template

A simple mlflow template using pymsql and nginx.

After filling up the missing variables in .env file, the command below will create the services and mlflow will be ready to use.

```bash
docker-compose --env-file .env up -d --build
```

### RDS Postgress

- .env file needs to be modified accordingly.

- In MLFlow Dockerfile, both mysql and postgres engines are installed. Depending on the database used, the other one can be removed (not essential).

- If the database is moved to AWS RDS, `mlflow_db` service can be removed from the compose file. Additionally, RDS database needs to be configured to communicate with the machine that hosts MLFlow server.
