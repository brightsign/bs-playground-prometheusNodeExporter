# brightsign-prometheus-playground
Playground for using Prometheus Node Exporter on BrightSign players

## Enable the BrightSign player's Prometheus Node Exporter 

Initialize the Prometheus Node Exporter (PNE) on the BrightSign player. It can be done through a registry,
```bash
registry write networking prometheus-node-exporter-port 9100
```

## Getting Started 

This project will use Docker to create a prometheus server and grafana server in their respective containers.

```bash
docker compose up
```

Navigate to http://localhost:3000/ to view the _Default -> Full Node Exporter_ Dashboard this project includes. 

## Dependencies

This project uses Docker - install from below links if it's not installed on your machine. 

* Install [Docker Desktop](https://docs.docker.com/desktop/) which includes all dependencies. (Recommended)

OR

* Install [Docker Engine](https://docs.docker.com/engine/install)
* Install [Docker Compose](https://docs.docker.com/compose/install/)

