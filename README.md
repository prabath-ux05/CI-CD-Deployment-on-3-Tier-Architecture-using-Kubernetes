# ☸️ CI/CD Deployment on 3-Tier Architecture using Kubernetes

![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-D24939)
![AWS](https://img.shields.io/badge/AWS-Cloud-FF9900)
![Python](https://img.shields.io/badge/Python-Flask-3776AB)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1)

---

## 📌 Overview

This project demonstrates the deployment of a containerized 3-tier web application using Kubernetes, Docker, Jenkins, and AWS.

The solution automates the entire software delivery lifecycle, from source code management and container image creation to Kubernetes deployment and application updates.

A complete CI/CD pipeline is implemented using Jenkins to automatically build Docker images, push them to Docker Hub, and deploy them to a Kubernetes cluster running on AWS infrastructure.

The deployed application consists of:

- Frontend Layer
- Backend API Layer
- MySQL Database Layer

The architecture follows cloud-native deployment principles and demonstrates modern DevOps practices using container orchestration and infrastructure automation.

---

## ✨ Key Features

### ☸️ Kubernetes Orchestration

- Kubernetes Cluster Provisioning
- Deployment Management
- Service Discovery
- Load Balancer Exposure
- Container Orchestration

### 🐳 Containerization

- Frontend Docker Image
- Backend Docker Image
- Image Versioning
- Docker Hub Integration

### 🔄 CI/CD Automation

- Jenkins Pipelines
- Automated Builds
- Automated Deployments
- GitHub Integration
- Webhook Triggering

### 🗄️ Database Management

- MySQL Deployment
- ConfigMap Initialization
- Persistent Storage
- PVC Integration

### ☁️ AWS Infrastructure

- EC2 Instances
- S3 State Storage
- IAM Configuration
- Kubernetes Cluster Hosting

---

## 🏗️ System Architecture

```text
Developer
    │
    ▼

GitHub Repository
    │
    ▼

GitHub Webhook
    │
    ▼

Jenkins Pipeline
    │
    ▼

Docker Build
    │
    ▼

Docker Hub
    │
    ▼

Kubernetes Cluster
    │
    ├── Frontend Pod
    ├── Backend Pod
    └── MySQL Pod
    │
    ▼

LoadBalancer Service
    │
    ▼

End Users
```

---

<details>
<summary><strong>⚙️ Tech Stack</strong></summary>

### ☸️ Container Orchestration

- Kubernetes
- Kops
- kubectl

### 🐳 Containerization

- Docker
- Docker Hub

### 🔄 CI/CD

- Jenkins
- GitHub Webhooks
- Jenkins Pipelines

### ☁️ Cloud Platform

- AWS EC2
- AWS S3
- AWS IAM

### 🖥️ Backend

- Python
- Flask
- Flask-CORS
- bcrypt

### 🎨 Frontend

- HTML
- CSS
- JavaScript

### 🗄️ Database

- MySQL
- ConfigMap
- Persistent Volume Claims

</details>

---

## 🔄 CI/CD Workflow

```text
Code Commit
      →
GitHub Repository
      →
Webhook Trigger
      →
Jenkins Pipeline
      →
Docker Build
      →
Docker Push
      →
Kubernetes Deployment
      →
Application Update
```

---

## 📊 Deployment Pipeline

```text
Developer
      →
GitHub
      →
Jenkins
      →
Docker Images
      →
Docker Hub
      →
Kubernetes Cluster
      →
Frontend + Backend + Database
```

---

## 🖼️ Project Preview

### Jenkins Automation

<p align="center">
  <img src="docs/jenkins-pipeline.png" width="90%">
</p>

### Docker Image Deployment

<p align="center">
  <img src="docs/docker-images.png" width="90%">
</p>

### Kubernetes Pods

<p align="center">
  <img src="docs/kubernetes-pods.png" width="90%">
</p>

### Student Registration Application

<p align="center">
  <img src="docs/student-registration.png" width="90%">
</p>

---

<details>
<summary><strong>📁 Project Structure</strong></summary>

```text
k8s-3-tier-architecture/
│
├── backend/
│   ├── Dockerfile
│   └── src/
│       ├── app.py
│       └── requirements.txt
│
├── frontend/
│   ├── Dockerfile
│   ├── index.html
│   ├── backend.html
│   └── student.html
│
├── k8s/
│   ├── frontend-deployment.yaml
│   ├── backend-deployment.yaml
│   └── db-deployment.yaml
│
├── Jenkinsfile
├── docs/
└── README.md
```

</details>

---

## 🧩 Application Architecture

### 🎨 Frontend Layer

Responsible for:

- User Registration
- User Login
- Student Registration Form
- Student Listing

### ⚙️ Backend Layer

Responsible for:

- Authentication APIs
- Student Management APIs
- Database Operations
- Business Logic

### 🗄️ Database Layer

Responsible for:

- User Storage
- Student Records
- Persistent Data Management

---

## ☸️ Kubernetes Components

### Deployments

- Frontend Deployment
- Backend Deployment
- MySQL Deployment

### Services

- Frontend LoadBalancer
- Backend LoadBalancer
- MySQL ClusterIP

### Configurations

- ConfigMaps
- Environment Variables
- Container Images

---

## 💾 Persistent Volume Claims (PVC)

To prevent data loss during pod recreation, Persistent Volume Claims are used.

### Benefits

- Persistent MySQL Storage
- Pod Failure Recovery
- Data Durability
- Stateful Workload Support

### PVC Workflow

```text
MySQL Pod
      →
Persistent Volume Claim
      →
Persistent Storage
      →
Data Retention
```

---

## 🚀 Jenkins Pipeline Stages

### 1️⃣ Source Checkout

Pull source code from GitHub.

### 2️⃣ Docker Build

Build backend and frontend images.

### 3️⃣ Docker Push

Push images to Docker Hub.

### 4️⃣ Kubernetes Deployment

Apply Kubernetes manifests.

### 5️⃣ Rolling Update

Update running workloads with latest images.

---

## 🚀 Local Setup

### Clone Repository

```bash
git clone https://github.com/yourusername/k8s-3-tier-arch.git

cd k8s-3-tier-arch
```

### Build Docker Images

```bash
docker build -t backend-app ./backend

docker build -t frontend-app ./frontend
```

### Deploy to Kubernetes

```bash
kubectl apply -f k8s/db-deployment.yaml

kubectl apply -f k8s/backend-deployment.yaml

kubectl apply -f k8s/frontend-deployment.yaml
```

### Verify Resources

```bash
kubectl get pods

kubectl get svc

kubectl get pvc
```

---

## 🔐 Prerequisites

Before running the project:

- AWS Account
- Kubernetes Cluster
- Jenkins Server
- Docker Installed
- kubectl Installed
- Docker Hub Account
- GitHub Repository

---

## 🛠️ Engineering Highlights

- Kubernetes Cluster Administration
- Jenkins Pipeline Automation
- Dockerized Microservices
- Container Image Versioning
- Automated Deployment Workflows
- GitHub Webhook Integration
- Persistent Storage Management
- Kubernetes LoadBalancer Services
- Infrastructure Automation
- Cloud-Native Deployment Architecture

---

## 🎯 Learning Outcomes

This project demonstrates practical experience with:

- Kubernetes Administration
- Container Orchestration
- Docker Image Management
- Jenkins CI/CD Pipelines
- Cloud-Native Applications
- Persistent Storage Design
- Service Exposure Strategies
- Application Deployment Automation
- DevOps Best Practices

---

## 🔮 Future Enhancements

### Kubernetes

- Helm Charts
- Horizontal Pod Autoscaling
- Ingress Controller
- Namespace Isolation

### DevOps

- GitHub Actions
- ArgoCD
- GitOps Workflow
- Automated Rollbacks

### Observability

- Prometheus Monitoring
- Grafana Dashboards
- Centralized Logging
- Alert Management

### Security

- Kubernetes Secrets
- RBAC
- Network Policies
- Image Scanning

---

## 📄 License

This project is intended for educational, learning, and portfolio demonstration purposes.

---

## 👨‍💻 Author

**Prabath D**
