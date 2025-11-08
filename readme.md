# Docker Monitoring
This repository contains the `docker-compose.yml` and configuration files to deploy Grafana for both **centralized logging** and **system metrics** to discovers and monitors all services running on your Docker host.

## 💻 Tech Stack
### Visualization
* **Grafana:** The unified dashboard for visualizing, querying, and alerting on all your logs (from Loki) and metrics (from Prometheus) in one place.

### Logging
* **Loki:** The log aggregation database, built for efficiently storing and searching log text.
* **Promtail:** The agent that discovers, collects, and **"pushes"** Docker container logs to Loki.

### Metrics
* **Prometheus:** The time-series database for collecting and storing all numeric metrics by pulling scraping data from exporters.
* **cAdvisor:** An agent that **"exposes"** real-time performance metrics (CPU, RAM, network) from all running **Docker containers** for Prometheus to **"pull"**.
* **Node Exporter:** An agent that **"exposes"** hardware and OS metrics from the **host VPS** (CPU, RAM, and disk usage) for Prometheus to **"pull"**.

## 📁 Structure
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
