### Kubernetes Beginners Guide

## 1. Docker Overview
- Introduction to Docker
- Basics of containerization
- Docker images and containers
- Docker commands

## 2. Docker Orchestration
- Importance of orchestration
- Overview of Docker Compose
- Introduction to Kubernetes as an orchestration tool

## 3. Kubernetes Architecture

### Cluster
A **Cluster** is a set of nodes (ranging from 1 to n) that work together to run containerized applications.

### Master Node
- Watches and monitors the worker/slave nodes
- Responsible for the actual orchestration of worker/slave nodes

### Components of Kubernetes
- **API Server**: Acts as the frontend for Kubernetes to interact with the cluster.
- **etcd Service**: A distributed and reliable key/value store for all data used to manage the cluster. Responsible for implementing logs within the cluster to prevent conflicts with the master.
- **Scheduler**: Distributes work across multiple nodes.
- **Controllers**: Handles node, container, and endpoint failures, bringing back failed or new resources as needed.
- **Container Runtime**: The underlying software used to run containers (e.g., Docker).
- **Kubelet**: An agent that runs on each node in the cluster to manage container operations.

### Master and Worker Nodes

| Master Nodes             | Worker Nodes          |
|--------------------------|-----------------------|
| API Server               | Kubelet               |
| etcd                     | Container Runtime     |
| Controller               |                       |
| Scheduler                |                       |

### Worker Node / Minions
- **Container Runtime (Docker)**: Runs the containers.

## Managing Kubernetes with kubectl
`kubectl` is used to deploy and manage applications within a Kubernetes cluster.

### Example Commands
```bash
kubectl run <image-name>       # Deploy an application
kubectl cluster-info           # Display cluster information
kubectl get nodes              # List all nodes in the cluster