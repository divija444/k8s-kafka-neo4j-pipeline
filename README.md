# k8s-kafka-neo4j-pipeline
Scalable real-time data processing pipeline using Apache Kafka, Kafka Connect, and Neo4j, orchestrated with Kubernetes (Minikube) for streaming ingestion and graph analytics.

---

## Repo contents
- `zookeeper-setup.yaml`        — Kubernetes Deployment + Service for Zookeeper  
- `kafka-setup.yaml`           — Kubernetes Deployment + Service for Kafka broker  
- `kafka-neo4j-connector.yaml` — Kafka Connect deployment using Neo4j connector image  
- `neo4j-values.yaml`          — Helm values for Neo4j (passwords, GDS enabled)  
- `data_producer.py`           — (optional) producer script that writes example messages to Kafka  
- `tester.py`                  — (optional) test/validation script (consumes topic + checks Neo4j)  
- `README.md`                  — this file  

---

## Quick prerequisites
- Docker installed  
- Minikube (>= latest stable)  
- kubectl (matches your minikube)  
- Helm 3  
- Python 3 (if using `data_producer.py` / `tester.py`)  

---
