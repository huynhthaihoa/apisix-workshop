# Hands-on lab Apache APISIX

This is the derived version of [Boburmirzo's Hands-on lab Apache APISIX](https://github.com/Boburmirzo/apisix-workshop). The original guideline is published at [GitHub page](https://boburmirzo.github.io/apisix-workshop/)

## Requirements
- [Docker](https://www.docker.com/)
- [curl](https://curl.se/docs/manpage.html)

## Install

Run the `docker compose` command to install Apache APISIX:

```
docker compose -p docker-apisix up -d
```

Once APISIX is running, send a simple HTTP request to validate if APISIX is working properly:

```
curl "http://127.0.0.1:9081" --head | grep Server
```

if everything is okay, the following response will be displayed:

```
Server: APISIX/Version
```

`Version` refers to the version of APISIX that you have installed.
