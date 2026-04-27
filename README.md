# Kubernetes Monitoring Stack

[![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)](https://prometheus.io/)
[![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)](https://grafana.com/)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)

## 📋 Project Overview

A complete, production-grade observability stack for Kubernetes using **Prometheus** for metrics, **Grafana** for visualization, and **Loki** for log aggregation. Includes a sample Flask application instrumented with Prometheus metrics and an automatic load generator.

## 🏗️ Architecture



## 📊 Components

| Component | Purpose | Port |
|-----------|---------|------|
| **Prometheus** | Metrics collection and storage | 9090 |
| **Grafana** | Visualization and dashboards | 3000 |
| **Loki** | Log aggregation | 3100 |
| **Alertmanager** | Alert routing | 9093 |
| **Sample App** | Flask app with Prometheus metrics | 8000 |

## 🚀 Quick Start

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop/) (4GB+ memory allocated)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/) (v1.34+)
- [kubectl](https://kubernetes.io/docs/tasks/tools/)
- [Helm](https://helm.sh/docs/intro/install/) (v3.0+)

### 1. Start Minikube

```bash
minikube start --driver=docker --cpus=2 --memory=4096