# Docker Tools

Simple tools for launching development services, such as `mysql`, `postgres` etc.

## Services

- [MongoDB](https://www.mongodb.com) as `mongo` (host port `27017`) 
- [PostgreSQL](https://www.postgresql.org) as `psql` (host port `5432`)
- [PipelineDB](https://www.pipelinedb.com) as `pipeline`(host port `5432`)
- [MySQL](https://www.mysql.com) as `mysql` (host port `3306`)
- [RabbitMQ](https://www.rabbitmq.com) as `rabbit` (host port `5672` and `15672`)
- [Redis](https://redis.io) as `redis` (host port `6379`)
- [InfluxDB](https://www.influxdata.com/products/influxdb-overview/) as `influx` (host port `8086` and `8083`)
- [NSQ](https://nsq.io) as `nsqd`, `nsqlookupd` and `nsqadmin` (host port `4160`, `4161`, `4150`, `4151` and `4171`)
- [Timescale](https://www.timescale.com/) as `ts` (host port `5432`)

## Usage

Credentials are set in a special `.env` file. Copy from `.env.dist` skeleton. Next launch the necessary services with the 
following command

```bash
docker-compose up -d --build [SERVICES]
```

If you do not specify services, all services will be launched.

Services available via host port.
