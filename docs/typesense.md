# Typesense

We use the official [Typesense](https://hub.docker.com/r/typesense/typesense/) Docker image.


## Installation

Typesense is an **optional** service and is **not installed or enabled by default**. To enable it, add the `typesense.yml` file to your `COMPOSE_FILE` list in the `.env` file. For example, on Unix systems:

```bash
COMPOSE_FILE=docker-compose.yml:opt/typesense.yml
```

After updating the `.env` file, run `docker compose up -d --remove-orphans` to start the service.


## Connecting

| Parameter | Value |
|-------------|---|
| Host | `typesense` (from a container)<br>`localhost` (from your computer) |
| Port | `8108` |
| Password | `typesense_admin_key` |
