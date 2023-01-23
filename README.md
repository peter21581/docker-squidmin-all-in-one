# docker-squidmin-all-in-one
- https://github.com/39ff/squid-db-auth-web

## Requirements
- docker
- docker-compose

# Ubuntu 22.04 LTS Install
apt update
apt upgrade -y
apt install apt-transport-https ca-certificates curl software-properties-common wget vim nano make cmake -y
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -
add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
apt-cache policy docker-ce
apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin docker-compose -y
systemctl status docker
docker --version
docker-compose --version

## Setup
```
git clone https://github.com/peter21581/docker-squidmin-all-in-one
cd docker-squidmin-all-in-one
git clone https://github.com/peter21581/squid-db-auth-web src
git clone https://github.com/peter21581/squid-db-auth-ip infra/docker/squid/external_module/squid-db-auth-ip
make init
make fresh
```
