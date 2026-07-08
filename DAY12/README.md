

# 🏥 Hospital Web Application Deployment using Docker & Kubernetes

## 📌 Project Overview

This project demonstrates how to containerize and deploy a Python-based Hospital Web Application using Docker and Kubernetes on a Minikube cluster. The application is deployed using Kubernetes resources such as Namespace, Pod, Deployment, Services, Persistent Volume, ConfigMap, and Secret.

---

## 🚀 Technologies Used

* Python (Flask)
* Docker
* Kubernetes
* Minikube
* kubectl
* Ubuntu (AWS EC2)

---

## 📂 Project Structure

```text
hospital-project/
│── app.py
│── Dockerfile
│── namespace.yml
│── pod.yml
│── deployment.yml
│── clusterip.yml
│── nodeport.yml
│── loadbalancer.yml
│── config.yml
│── secret.yml
│── pv.yml
│── README.md
```

---

## 📄 File Description

### app.py

* Main Python Flask application.
* Displays the Hospital Web Application.

### Dockerfile

* Creates a Docker image for the Flask application.
* Defines the runtime environment.

### namespace.yml

* Creates a dedicated Kubernetes Namespace.
* Organizes project resources separately.

### pod.yml

* Creates a single Kubernetes Pod to run the application.

### deployment.yml

* Creates and manages application Pods.
* Supports scaling and self-healing.

### clusterip.yml

* Creates an internal ClusterIP Service.
* Allows communication between Pods inside the cluster.

### nodeport.yml

* Exposes the application using a NodePort.
* Makes the application accessible through the Minikube node IP.

### loadbalancer.yml

* Creates a LoadBalancer Service.
* Provides external access (using Minikube Tunnel or cloud provider).

### config.yml

* Creates a ConfigMap.
* Stores application configuration values.

### secret.yml

* Creates Kubernetes Secrets.
* Stores sensitive information like passwords and API keys securely.

### pv.yml

* Creates a Persistent Volume.
* Provides persistent storage for the application.

---

## 🔄 Project Workflow

1. Developed the Hospital Web Application using Python.
2. Created a Dockerfile.
3. Built the Docker image.
4. Started the Minikube cluster.
5. Created a Kubernetes Namespace.
6. Deployed the application Pod.
7. Created a Deployment for high availability.
8. Configured ClusterIP Service.
9. Configured NodePort Service.
10. Configured LoadBalancer Service.
11. Created ConfigMap for configuration.
12. Created Secret for sensitive data.
13. Created Persistent Volume for storage.
14. Verified all Kubernetes resources using kubectl.

---

## 📌 Kubernetes Resources Used

* Namespace
* Pod
* Deployment
* ReplicaSet
* ClusterIP Service
* NodePort Service
* LoadBalancer Service
* ConfigMap
* Secret
* Persistent Volume (PV)

---

## 📷 Output

* Hospital Web Application successfully deployed on Kubernetes.
* Docker image created successfully.
* Pods running successfully.
* Services created successfully.
* Application accessible through NodePort/LoadBalancer.

---

## 📚 Learning Outcomes

* Docker Image Creation
* Containerization
* Kubernetes Architecture
* Pod Management
* Deployments
* Kubernetes Services
* ConfigMaps
* Secrets
* Persistent Volumes
* Minikube
* kubectl Commands

---
