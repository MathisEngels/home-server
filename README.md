# Home server
This repository contains all the Docker Compose files used to managed services on my home server.

> [!NOTE]
> This is used has a backup in case something goes wrong.

## Prerequisite
You must create the traefik's network before hand.
```sh
$ docker volume create -d bridge ${TRAEFIK_NETWORK}
```
> [!IMPORTANT]
> ``TRAEFIK_NETWORK`` must be the same as in the ``.env`` file.


## Start / Recover containers
You can start / recover containers by running the following command:
```sh
$ docker-compose -f compose-files/<service-name>.yml up -d
```