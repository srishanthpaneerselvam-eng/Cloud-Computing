
# Deploying a Microservices Architecture Application using Kubernetes, GitHub Actions, Argo CD, Prometheus and Grafana

## 📌 Project Overview

This project demonstrates the deployment of a cloud-native microservices application using Kubernetes. The application used is Google's **Online Boutique**, which consists of multiple independent services communicating with each other.

The project was deployed on an AWS EC2 Ubuntu instance using **K3s (Lightweight Kubernetes)** and **Helm**. The frontend service was exposed using **NodePort** to allow external access through a web browser.

The project also explains how modern DevOps tools such as **GitHub Actions**, **Argo CD**, **Prometheus**, and **Grafana** can be integrated into a Kubernetes-based deployment workflow.

---

## 🎯 Objectives

- Deploy a microservices application on Kubernetes.
- Learn Kubernetes fundamentals.
- Deploy applications using Helm.
- Configure Kubernetes Services.
- Expose applications using NodePort.
- Understand CI/CD concepts.
- Learn GitOps using Argo CD.
- Understand Kubernetes monitoring with Prometheus.
- Visualize metrics using Grafana.

---

## 🛠️ Technologies Used

- AWS EC2
- Ubuntu 22.04
- Docker
- Kubernetes (K3s)
- kubectl
- Helm
- GitHub
- GitHub Actions
- Argo CD
- Prometheus
- Grafana

---

## 🏗️ Project Architecture

```
Developer
     │
     ▼
GitHub Repository
     │
     ▼
GitHub Actions
(Build Docker Images)
     │
     ▼
Docker Hub
     │
     ▼
Argo CD
     │
     ▼
Kubernetes Cluster
     │
     ▼
Online Boutique Microservices
     │
     ▼
Prometheus
     │
     ▼
Grafana Dashboard
```

---

## 📂 Project Workflow

1. Launch an AWS EC2 Ubuntu instance.
2. Configure Security Groups.
3. Install Docker, K3s, kubectl, and Helm.
4. Deploy the Online Boutique application using Helm.
5. Verify Kubernetes nodes, pods, and services.
6. Expose the frontend service using NodePort.
7. Access the application through the EC2 Public IP.
8. Test the shopping cart and checkout process.
9. Integrate GitHub Actions for CI (concept).
10. Use Argo CD for GitOps deployment (concept).
11. Monitor the cluster using Prometheus.
12. Visualize metrics using Grafana.

---

## 🚀 Deployment Commands

### Install K3s

```bash
curl -sfL https://get.k3s.io | sh -
```

### Verify Cluster

```bash
kubectl get nodes
```

### Install Helm

```bash
helm version
```

### Deploy Online Boutique

```bash
helm install boutique . -n boutique
```

### View Services

```bash
kubectl get svc -n boutique
```

### Expose Frontend

```bash
kubectl patch svc frontend -n boutique -p '{"spec":{"type":"NodePort"}}'
```

---

## 📊 Features

- Cloud-native microservices architecture
- Kubernetes-based deployment
- Helm package management
- NodePort service exposure
- CI/CD workflow concepts
- GitOps deployment concepts
- Kubernetes monitoring
- Dashboard visualization
- Scalable and modular architecture

---

## 📈 Results

- Successfully deployed Online Boutique on Kubernetes.
- Verified Kubernetes nodes, pods, and services.
- Frontend exposed using NodePort.
- Application accessed successfully through browser.
- Checkout workflow tested successfully.
- Demonstrated modern DevOps workflow using Kubernetes.

---

## ✅ Advantages

- High scalability
- Independent service deployment
- Better fault isolation
- Easy maintenance
- Automated deployment support
- Easy monitoring
- Improved reliability
- Cloud-native architecture

---

## 🔮 Future Enhancements

- Deploy on Amazon EKS.
- Fully automate CI/CD using GitHub Actions.
- Integrate Argo CD with GitHub repository.
- Deploy Prometheus and Grafana in the cluster.
- Configure Ingress Controller and Load Balancer.
- Implement Horizontal Pod Autoscaling (HPA).
- Add security scanning in the CI/CD pipeline.

---

## 📚 Learning Outcomes

Through this project, I gained practical knowledge of:

- Kubernetes fundamentals
- Microservices architecture
- Helm deployments
- Kubernetes networking
- NodePort services
- Cloud-native application deployment
- CI/CD concepts
- GitOps workflow
- Kubernetes monitoring and visualization

---



---

## 📄 License

This project is developed for academic learning and educational purposes.
````

This README is suitable for a GitHub repository and aligns with the scope of your project report.
