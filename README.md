# djp-zaproxy

A [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) jsonnet package (**djp**).

## Description

[Zaproxy](https://www.zaproxy.org/) djp package

## Snippet

- `ddb.yml`

```yaml
cookiecutter:
  templates:
    - template: gh:inetum-orleans/zaproxy
      extra_context:
        zaproxy_version: 'stable'
        port: 8080
        host: 0.0.0.0
```

- `docker-compose.yml.jsonnet`

```jsonnet
ddb.Compose(
  ddb.with(
    import '.docker/zaproxy/djp.libjsonnet'
  )
)
```

## Parameters

| name            | type | description |
|-----------------| ------------- | ------------- |
| zaproxy_version | string  | The tag version of the Docker image of Zap Proxy, ex : ghcr.io/zaproxy/zaproxy:stable
| port            | string  | The port used to connect to Zap Proxy, ex: 8080
| host            | string  | The host used to connect to Zap Proxy, ex: 0.0.0.0

## Usage

Please check [jsonnet feature](https://inetum-orleans.github.io/docker-devbox-ddb/features/jsonnet/#ddb-jsonnet-packages-djp)
to understand how to include a **djp** package inside a [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) project.

Looking for other [djp packages](https://github.com/inetum-orleans?q=djp-) ? Check github repositories starting with `djp-`.
