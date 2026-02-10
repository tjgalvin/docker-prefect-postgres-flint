# docker-prefect-postgres-flint

A simple docker compose build file to establish a prefect server with a postgres database backend. Pgbouncer is also included to act as a connection pooler, which is than the sqlalchemy tooling.

## How to run

It should be

```
docker composer up -d
```

to run in a dettached mode. Logs can be examined via `docker compose logs`. Optionally the name of the service may be added. 

Should you need to modify the set up you will first need to shutdown the docker composition via

```
docker compose down
```

## Database location

The database will stored in the working directory where the `docker compose up` command is issued.

