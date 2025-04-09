# Deployments in Kubernetes

## Overview

Deployments in Kubernetes help manage **rolling updates**, allow you to **rollback updates**, and provide control over **pods** running your applications. A Deployment ensures your desired state for application deployment is maintained and can be updated or reverted when needed.

---

## Key Concepts

### Rolling Updates
- Updates the application gradually without downtime.
- Ensures that some pods are always available during the update.

### Rollbacks
- Easily revert to a previous deployment revision if the new one fails.

### Pods
- The smallest deployable unit in Kubernetes.
- Represents a running instance of your application (e.g., a web app).

### ReplicaSet
- Ensures a specified number of pod replicas are running at all times.
- Automatically created and managed by Deployments.
- Multiple pods from a ReplicaSet may run on the same instance.

### Deployment Features
- Supports rolling updates and rollback.
- Allows pausing and resuming ongoing updates.
- Keeps history of previous configurations.

---

## Useful Commands

```bash
# View all resources including pods, ReplicaSets, and deployments
kubectl get all
