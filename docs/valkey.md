# Valkey

We use the official [Valkey](https://hub.docker.com/r/valkey/valkey/) Docker image. It aims to be fully compatible with Redis.

> In March 2024, Redis announced that they will be [changing their BSD license](https://redis.com/blog/redis-adopts-dual-source-available-licensing/) to ones that are not open-source. As a result, we have swapped to using the open source fork of Redis, called Valkey.


## Installation

Valkey is an **optional** service and is **not installed or enabled by default**. To enable it, add the `valkey.yml` file to your `COMPOSE_FILE` list in the `.env` file. For example, on Unix systems:

```bash
COMPOSE_FILE=docker-compose.yml:opt/valkey.yml
```

After updating the `.env` file, run `docker compose up -d --remove-orphans` to start the service.


## Connecting

| Parameter | Value |
|-------------|---|
| Host | `valkey` (from a container)<br>`localhost` (from your computer) |
| Port | `6379` |
| Password | `` |

> For backwards compatibility we've added a `redis` alias. You can either hostname in your application.
