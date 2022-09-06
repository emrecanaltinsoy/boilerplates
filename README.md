## MLFlow Template

A simple mlflow template using pymsql and nginx.

After filling up the missing variables in .env file, the command below will create the services and mlflow will be ready to use.

```bash
docker-compose --env-file .env up -d --build
```
