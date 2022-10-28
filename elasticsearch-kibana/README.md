# Elasticsearch-Kibana Template

A simple Elasticsearch-Kibana template with nginx reverse proxy.

## Start Services

### Example .env File

```
ELASTICSEARCH_USERNAME=
ELASTICSEARCH_PASSWORD=
```

After filling up the missing variables in .env file, the command below will create the services and kibana will be ready to use.

```bash
docker-compose --env-file .env up -d --build
./reset_password
```

### Kibana Login

Login kibana dashboard with username 'elastic' and password that is set inside .env file.

## Stop Services and Remove Volumes

```bash
docker-compose down --volumes
```
