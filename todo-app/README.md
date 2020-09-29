# Docker-Todo

This repository contains a docker-compose manifest to deploy a simple todo app. One app is run as a container and the other as a service.

### Setup

**Container**
To run the container `docker build -t todos .`
To start the container `docker run -dp 3000:3000 todos`
To stop the container `docker stop 3000:3000 container_id_or_name`

**Service**
To load the stack, from the root directory run `docker-compose up -d --build`
To unload the stack, from the root directory run `docker-compose down`

### Access container or service

It will be accessible at [localhost:3000](http://localhost:3000)

### Credits

Special thanks to the Docker team for their  [tutorial](https://github.com/docker/getting-started)
