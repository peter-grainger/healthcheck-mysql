# healthcheck mysql

Can be used to rebuild image petergrainger/healthcheck-mysql:5.7

## Synopsis

Docker image and accompanying script to wrap the [mysql:5.7](https://github.com/docker-library/mysql/blob/bb7ea52db4e12d3fb526450d22382d5cd8cd41ca/5.7/Dockerfile) docker image adding the [healthcheck](https://docs.docker.com/engine/reference/builder/) directive to verify mysql is running.

## Motivation

This image is not required using docker compose, this file can define a healthcheck directly.  This image can be used for codeship as a healthcheck is not required.  The healthcheck images provided by docker (healthcheck/mysql) use the latest version of mysql and won't work if version 5.7 is needed.

## Usage

```
docker pull petergrainger/healthcheck-mysql:5.7
```

## Build

```
docker build . -t petergrainger/healthcheck-mysql:5.7
```
