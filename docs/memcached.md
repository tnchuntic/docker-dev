# Memcached

We use the official [Memcached](https://hub.docker.com/_/memcached) image.


## Installation

Memcached is an **optional** service and is **not installed or enabled by default**. To enable it, add the `memcached.yml` file to your `COMPOSE_FILE` list in the `.env` file. For example, on Unix systems:

```bash
COMPOSE_FILE=docker-compose.yml:opt/memcached.yml
```

After updating the `.env` file, run `docker compose up -d --remove-orphans` to start the service.


## Connecting

| Parameter | Value |
|-------------|---|
| Host | `memcached` (from a container)<br>`localhost` (from your computer) |
| Port | `11211` |
