# Panorama360 data collection architecture

This project deploys all the required services for the Panorama360 data collection on a single machine, using container technologies with Docker (https://www.docker.com/) and Docker Compose (https://docs.docker.com/compose/).

The current configuration of the services requires authentication on RabbitMQ, but all the other services are open and exposed on external traffic from the host machine. Feel free to edit the _docker-compose.yml_ and the other config files in order to restrict access.

_Username_: panorama
_Password_: panorama

## Prerequisites

On the machine we want to deploy the services the following software has to be installed and configured.
- Docker (https://docs.docker.com/install/)
- Docker Compose (https://docs.docker.com/compose/install/)

Spawning the services
----------------------
Change to the directory where you've cloned this repository and execute the following docker-compose command

```
docker-compose up -d
```

Terminating the services
-------------------------
In order to terminate the services, from whithin the same directory execute the following docker-compose command

```
docker-compose down
```
