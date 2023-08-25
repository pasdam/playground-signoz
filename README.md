# playground-signoz

This repo contains a docker compose playground to test
[SigNoz](https://github.com/SigNoz/signoz).

Freely inspired by
[this](https://github.com/SigNoz/signoz/blob/develop/deploy/docker/clickhouse-setup/docker-compose.yaml).

## Components

### Clickhouse

[Clickhouse](https://github.com/SigNoz/signoz) is the DB where all the data is
stored. Given this is just a playground Clickhouse is deployed in a standalone
mode, without external Zookeeper, but it rather uses
[clickhouse-keeper](https://clickhouse.com/docs/en/guides/sre/keeper/clickhouse-keeper).

## Usage

```shell
docker compose up
```

This will start all the services, after all are up and running you can point the
browser to [localhost:3301](http://localhost:3301/).
