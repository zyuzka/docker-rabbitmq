# RabbitMQ

## Description

Extends official RabbitMQ image to compile with HiPE (High performance Erlang) enabled in order to increase performance.

* Based on: Official `RabbitMQ 3.7.14` and `Alpine 3.8`
* `HiPE` (High performance Erlang) is enabled in order to significantly increase performance in runtime.
* A non-recent version of `RabbitMQ` (3.7.14) is used due to fact `RabbitMQ` 3.7.15+ uses `Erlang` 22 without `HiPE` support.

> Note: Provided images require additional configuration for development, staging and production use.

## Tags

| Tag     | RabbitMQ version     | Details     | Dockerfile     |
| :------------- | :------------- | :------------- | :------------- |
| [spryker/rabbitmq:latest](https://hub.docker.com/r/spryker/rabbitmq/tags) | 3.7.14 | [![](https://images.microbadger.com/badges/image/spryker/rabbitmq:latest.svg)](https://microbadger.com/images/spryker/rabbitmq:latest "Get your own image badge on microbadger.com") | [:link:](https://github.com/spryker/docker-rabbitmq/blob/master/3.7.14/Dockerfile) |
| [spryker/rabbitmq:3.7.14](https://hub.docker.com/r/spryker/rabbitmq/tags)  | 3.7.14 | [![](https://images.microbadger.com/badges/image/spryker/rabbitmq:3.7.14.svg)](https://microbadger.com/images/spryker/rabbitmq:3.7.14 "Get your own image badge on microbadger.com") | [:link:](https://github.com/spryker/docker-rabbitmq/blob/master/3.7.14/Dockerfile) |

## How to use

### Pull image
```bash
$ docker pull spryker/rabbitmq:3.7.14
```

### Dockerfile
```dockerfile
FROM spryker/rabbitmq:3.7.14
```

### docker-compose.yml
```yaml
broker:
    image: spryker/rabbitmq:3.7.14
```


## More information
* [RabbitMQ official images](https://github.com/docker-library/rabbitmq)
* [RabbitMQ with High Performance Erlang](https://www.cloudamqp.com/blog/2014-03-31-rabbitmq-hipe.html)
