# Docker Compose Services

## Services

### Postgres

Create a `postgres.secrets.env` file under `./env` directory and set the `POSTGRES_PASSWORD` environment variable.

Then execute the following `compose` command to run the postgres service:

```shell
docker compose -f postgres.yml up -d postgresql
```

To stop the service, just execute the command:

```shell
docker compose -f postgres.yml down postgresql
```
