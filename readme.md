# Docker Monitoring
This repository contains the `docker-compose.yml` and configuration files to deploy a lightweight, self-hosted monitoring and logging stack using **Grafana, Loki, and Promtail** to automatically discover, scrape, and visualize the log output from all running Docker containers on a host machine, providing a powerful and centralized logging solution.

## 💻 Monitoring Stack Tech
* **Grafana:** The dashboard UI for visualizing and querying logs
* **Loki:** The main log aggregation database, optimized for log text
* **Promtail:** The agent that scrapes logs from Docker containers and ships them to Loki
* **Docker Compose:** For orchestrating the monitoring stack itself

## 📁 Configuration Folder Structure
```
config/ 
├── loki/
|   └── promtail.yml
└── promtail/
    └── promtail.yml
docker-compose.yml
```
