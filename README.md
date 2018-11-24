# Docker Postgres Boilerplate

A Docker-compose Postgres boilerplate.
Connects to host via a configured docker network named 'dockernet'

A .env file stores variables and values used in the docker-compose.yml file.
The .env file is listed in .gitignore.

## Configure dockernet
docker network create -d bridge --subnet xxx.xxx.0.0/24 --gateway xxx.xxx.0.1 dockernet

The x's in the IPv4 address should be the same as the host machine's.

# Citations:
https://forums.docker.com/t/accessing-host-machine-from-within-docker-container/14248/5