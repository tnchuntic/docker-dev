# Meilisearch

We use the official [Meilisearch](https://hub.docker.com/r/getmeili/meilisearch/) Docker image.


## Installation

Meilisearch is an **optional** service and is **not installed or enabled by default**. To enable it, add the `meilisearch.yml` file to your `COMPOSE_FILE` list in the `.env` file. For example, on Unix systems:

```bash
COMPOSE_FILE=docker-compose.yml:opt/meilisearch.yml
```

After updating the `.env` file, run `docker compose up -d --remove-orphans` to start the service.


## Connecting

| Parameter | Value |
|-------------|---|
| Host | `meilisearch` (from a container)<br>`localhost` (from your computer) |
| Port | `7700` |
| Password | `meilisearch_admin_key` |
