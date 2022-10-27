# Docker-compose templates

List of current services

- Portainer
- Heimdall (Dashboard)
- Nginx Proxy Manager
- Code-Server
- Vaultwarden
- Guacamole
- Authelia

## Run Services

### Portainer

```bash
docker-compose -f docker-compose.portainer.yaml --env-file <env-file> up -d
```

Sample .env file for the portainer service.

```
DATA_PATH=
HTTP_PORT=
HTTPS_PORT=
```

### Heimdall

```bash
docker-compose -f docker-compose.heimdall.yaml --env-file <env-file> up -d
```

Sample .env file for the heimdall service.

```
PUID=
PGID=
TZ=
CONFIG_PATH=
HTTP_PORT=
HTTPS_PORT=
```

### Nginx Proxy Manager

```bash
docker-compose -f docker-compose.nginxproxymanager.yaml --env-file <env-file> up -d
```

Sample .env file for the nginxproxymanager service.

```
DATA_PATH=
LETS_ENCRYPT_PATH=
PORT=
HTTP_PORT=
HTTPS_PORT=
```

### Code-Server

```bash
docker-compose -f docker-compose.codeserver.yaml --env-file <env-file> up -d
```

Sample .env file for the codeserver service.

```
PUID=
PGID=
TZ=
PASSWORD=
HASHED_PASSWORD= # optional
SUDO_PASSWORD=
SUDO_PASSWORD_HASH= # optional
PROXY_DOMAIN= # optional
DEFAULT_WORKSPACE=/config/workspace
PORT=
HTTP_PORT=
HTTPS_PORT=
CONFIG_PATH=
```

### Vaultwarden

```bash
docker-compose -f docker-compose.vaultwarden.yaml --env-file <env-file> up -d
```

Sample .env file for the vaultwarden service.

```
DATA_PATH=
PORT=
```

### Guacamole

```bash
docker-compose -f docker-compose.guacamole.yaml --env-file <env-file> up -d
```

Sample .env file for the guacamole service.

```
CONFIG_PATH=
PORT=
```

### Authelia

```bash
docker-compose -f docker-compose.authelia.yaml --env-file <env-file> up -d
```

Sample .env file for the authelia service.

```
CONFIG_PATH=
PORT=
TZ=Europe/Madrid
```
