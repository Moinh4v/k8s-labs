# Kubernetes Setup

## **Setting Up Kubernetes**

### In Local Environments
- **Minikube**: Lightweight Kubernetes for local development and testing.  
- **MicroK8s**: Minimal, lightweight Kubernetes distribution.  
- **kubeadm**: Tool to bootstrap Kubernetes clusters.

### In Cloud Environments
- **GCP (Google Cloud Platform)**  
- **Azure**  
- **AWS (Amazon Web Services)**

---

## **Pods in Kubernetes**

A **Pod** is a single instance of an application, encapsulated in a Kubernetes object.  
Pods usually have a **one-to-one relationship** with containers.

### **Types of Pods:**
- **Single-Container Pods:** Most common, running a single application container.  
- **Multi-Container Pods:** A single pod can have multiple containers, including **helper containers** for sidecar tasks.

---

## **Basic `kubectl` Commands**

- **Run an NGINX Pod:**  
  ```bash
  kubectl run nginx --image=nginx

`kubectl run nginx --image nginx` - run nginx image
`kubectl get pods` - display the list of pods

A note about creating pods using kubectl run.

To create a pod from the command line, use the command:

Create an NGINX Pod
```bash
kubectl run nginx --image=nginx
```
As of version 1.18, kubectl run (without any arguments such as --generator ) will create a pod instead of a deployment.

To create a deployment using imperative command, use kubectl create:

kubectl create deployment nginx --image=nginx

Kubernetes Concepts – https://kubernetes.io/docs/concepts/

Pod Overview- https://kubernetes.io/docs/concepts/workloads/pods/pod-overview/
