# djp-template

A [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) jsonnet package (**djp**).

## Description

Write a short description of this **djp** package.

## Snippet

- `ddb.yml`

```yaml
cookiecutter:
  templates:
    - template: gh:inetum-orleans/djp-template
```

- `docker-compose.yml.jsonnet`

```jsonnet
ddb.Compose(
  ddb.with(
    import '.docker/djp/djp.libjsonnet',
    params={param1: 'value1', param2: ['value2']}
  )
)
```

## Parameters

| name  | type | description |
| ------------- | ------------- | ------------- |
| param1  | string  | Description of first parameter
| param2  | string[]  | Description of second parameter

## Usage

Please check [jsonnet feature](https://inetum-orleans.github.io/docker-devbox-ddb/features/jsonnet/#ddb-jsonnet-packages-djp)
to understand how to include a **djp** package inside a [ddb](https://inetum-orleans.github.io/docker-devbox-ddb) project.

Looking for other [djp packages](https://github.com/inetum-orleans?q=djp-) ? Check github repositories starting with `djp-`.
