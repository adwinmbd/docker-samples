# Docker-Grafana-Loki

This repository contains a docker-compose manifest to deploy a simple system to play around with [Loki](https://github.com/grafana/loki), and [Grafana](https://grafana.com/) for log management.

### Setup

**v1**
To load the stack, from the root directory run `docker-compose up -d --build`
To unload the stack, from the root directory run `docker-compose down`

**v2&3**
There is need for some configuration before projects v2&3 can work.

Install the Loki driver plugin 
`docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions`

To load the stack, from the root directory run `docker-compose up -d --build`
To unload the stack, from the root directory run `docker-compose down`

To uninstall the plugin.
```
docker plugin disable loki
docker plugin rm loki
```

### Access to Grafana

Grafana will be accessible at [localhost:3000](http://localhost:3000), the credentials are the default ones: username `admin`, password `admin`.

### Credits
Special thanks to the Grafana team for the documentation on  [loki driver](https://grafana.com/docs/loki/latest/clients/docker-driver/)

To this [tutorial](http://tjtjtj.hatenablog.com/entry/2019/08/17/145550/) in Japanese from tjtjtj.

