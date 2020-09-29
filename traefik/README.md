# Docker-Traefik

This repository contains a docker-compose manifest to deploy a simple system to play around with [Traefik](https://doc.traefik.io/traefik/) and [Whoami](https://hub.docker.com/r/containous/whoami/) to show edge routing in action. One project uses HTTP while the other HTTPS.

### Setup

To load the stack, from the root directory run `docker-compose up -d --build`
To unload the stack, from the root directory run `docker-compose down`
Further instructions on accessing the services are in the docker-compose files.
