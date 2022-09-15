# docker-squidmin-all-in-one
- https://github.com/39ff/squid-db-auth-web

## Requirements
- docker
- docker-compose

## Setup
```
git clone https://github.com/39ff/docker-squidmin-all-in-one
cd docker-squidmin-all-in-one
git clone https://github.com/39ff/squid-db-auth-web src
git clone https://github.com/39ff/squid-db-auth-ip infra/docker/squid/external_module/squid-db-auth-ip
make init
make fresh
```
