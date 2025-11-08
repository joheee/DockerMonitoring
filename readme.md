# Docker Monitoring
This repository contains the `docker-compose.yml` and configuration files to deploy a lightweight, self-hosted monitoring and logging stack using **Grafana, Loki, and Promtail** to automatically discover, scrape, and visualize the log output from all running Docker containers on a host machine, providing a powerful and centralized logging solution.

## 💻 Monitoring Stack Tech
* **Grafana:** The dashboard UI for visualizing and querying logs
* **Loki:** The log aggregation database
* **Promtail:** The agent that scrapes logs from Docker containers and ships them to Loki
* **Prometheus:** The time series database for storing all numeric metrics
* **cAdvisor:** An agent that that exposes metrics from all running Docker Containers for Prometheus to pull 
* **Node Exporter:** An agent that exposes hardware metrics from the host VPS for Prometheus to pull

## 📁 Configuration Folder Structure
```
config/ 
├── loki/
|   └── loki.yml
├── prometheus/
|   └── prometheus.yml
└── promtail/
    └── promtail.yml
docker-compose.yml
```
