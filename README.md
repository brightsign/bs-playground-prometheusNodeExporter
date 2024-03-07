# brightsign-prometheus-playground

Playground for using Prometheus Node Exporter on BrightSign players

## Enable the BrightSign player's Prometheus Node Exporter

Initialize the Prometheus Node Exporter (PNE) on the BrightSign player introduced in BOS 9.0.126. It is currently enabled through a registry,

```bash
registry write networking prometheus-node-exporter-port 9100
```

## Getting Started

1. Enable PNE on the BrightSign player, see [Enable the BrightSign player's Prometheus Node Exporter](#Enable-the-BrightSign-player's-Prometheus-Node-Exporter).
2. Add IP Address of your BrightSign Player on the Local Network to the `prometheus.yml` file under `targets` in the `scrape_configs` section.
3/ Start docker

This project will use Docker to create a prometheus server and grafana server in their respective containers.

```bash
docker compose up
```

4/ Navigate to [http://localhost:3000/](http://localhost:3000/) to view the _Default -> Full Node Exporter_ Dashboard this project includes.

## Dependencies

This project uses Docker - install from below links if it's not installed on your machine.

* Install [Docker Desktop](https://docs.docker.com/desktop/) which includes all dependencies. (Recommended)

OR

* Install [Docker Engine](https://docs.docker.com/engine/install)
* Install [Docker Compose](https://docs.docker.com/compose/install/)
