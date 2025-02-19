# Docker Compose Services

## Services

### Postgres

Create a `postgres.secrets.env` file under `./env` directory and set the `POSTGRES_PASSWORD` environment variable.

Then execute the following `compose` command to run the postgres service:

```shell
docker compose -f compose.yml up -d postgres
```

To stop the service, just execute the command:

```shell
docker compose -f compose.yml down postgres
```

### MINIO

Create a `minio.secrets.env` file under `./env` directory and set the `MINIO_ROOT_PASSWORD` environment variable.

Then execute the following `compose` command to run the minio service:

```shell
docker compose -f compose.yml up -d minio
```

To stop the service, just execute the command:

```shell
docker compose -f compose.yml down minio
```

### Pulsar (standalone)

Execute the `compose` command to start Apache Pulsar in a standalone mode:

```shell
docker compose -f compose.yml up -d pulsar
```

To stop the service, just execute the command:

```shell
docker compose -f compose.yml down pulsar
```