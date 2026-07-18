# 🚀 Automated CI/CD Pipeline for a Dockerized 3-Tier Application

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5?logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Cloud-FF9900?logo=amazonaws&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Linux-Ubuntu-E95420?logo=ubuntu&logoColor=white)

> 🚧 **Project Status:** Ongoing

---

# 📌 Project Overview

This project demonstrates an automated **CI/CD pipeline** for a Dockerized **3-tier web application** using **GitHub Actions, Docker, Kubernetes, and AWS EC2**.

The primary objective is to automate the complete software delivery lifecycle—from source code management to deployment—by following modern DevOps practices.

The application consists of a frontend, backend, and MySQL database. Every code push automatically triggers a Continuous Integration (CI) workflow that builds Docker images and publishes them to Docker Hub. A Continuous Deployment (CD) workflow then deploys the latest version of the application to an AWS EC2 instance.

This repository is maintained as an **ongoing DevOps learning project**, with continuous improvements in automation, container orchestration, and deployment strategies.

---

# ✨ Project Highlights

- Automated CI/CD pipeline using GitHub Actions
- Dockerized three-tier application
- Multi-stage Docker builds
- Docker Compose deployment
- Kubernetes deployment manifests
- AWS EC2 deployment
- Docker Hub integration
- Secure GitHub Secrets management
- Infrastructure automation following DevOps best practices

---

# 🛠️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| CI/CD | GitHub Actions |
| Containers | Docker, Docker Compose |
| Orchestration | Kubernetes (Kind) |
| Cloud | AWS EC2 |
| Backend | Go (Gin Framework) |
| Frontend | HTML, CSS, JavaScript, Nginx |
| Database | MySQL |
| Version Control | Git & GitHub |
| Operating System | Ubuntu Linux |

---

# 🏗️ Solution Architecture

<p align="center">
<img src="architecture/architecture.png" width="100%" alt="CI/CD Pipeline Architecture">
</p>

The following architecture illustrates the complete CI/CD workflow. Every code push triggers GitHub Actions to build Docker images, publish them to Docker Hub, and automatically deploy the latest version to AWS EC2. The repository also includes Kubernetes manifests for deploying the application on a local Kind cluster.

---

# 📂 Project Structure

```text
CI-CD-Pipeline-Docker-Kubernetes
│
├── .github/
│   └── workflows/
│       ├── ci.yml
│       └── cd.yml
│
├── application/
│   ├── backend/
│   ├── frontend/
│   └── mysql/
│
├── docker/
│   └── docker-compose.yml
│
├── kubernetes/
│   ├── kind-config.yaml
│   ├── namespace.yaml
│   ├── backend.yaml
│   ├── frontend.yaml
│   └── mysql.yaml
│
├── architecture/
│   └── architecture.png
│
├── screenshots/
│
├── docs/
│
├── README.md
└── .gitignore
```

---

# 🔄 CI/CD Workflow

```text
Developer
      │
      ▼
Git Push
      │
      ▼
GitHub Repository
      │
      ▼
GitHub Actions (CI)
      │
      ├── Checkout Source Code
      ├── Build Backend Image
      ├── Build Frontend Image
      ├── Tag Docker Images
      └── Push Images to Docker Hub
                │
                ▼
           Docker Hub
                │
                ▼
GitHub Actions (CD)
                │
                ├── SSH into AWS EC2
                ├── Pull Latest Docker Images
                ├── Docker Compose Up -d
                └── Health Check
                │
                ▼
      Running Dockerized Application
```

---

# 🚀 Deployment Flow

```text
Developer
      │
      ▼
Git Push
      │
      ▼
GitHub Repository
      │
      ▼
GitHub Actions (CI)
      │
      ▼
Docker Hub
      │
      ▼
GitHub Actions (CD)
      │
      ▼
AWS EC2 Instance
      │
      ▼
Docker Compose
      │
      ▼
Frontend (Nginx)
      │
      ▼
Backend (Go + Gin)
      │
      ▼
MySQL Database
```

---

# 🚀 Key Features

- Automated CI/CD using GitHub Actions
- Dockerized frontend and backend services
- Multi-stage Docker builds
- Docker Compose deployment
- Kubernetes deployment manifests
- Docker Hub image publishing
- AWS EC2 deployment
- GitHub Secrets integration
- Three-tier application architecture
- Infrastructure automation

---

# ⚙️ Key Components

## GitHub Actions

- Automates CI/CD pipelines
- Builds Docker images
- Publishes images to Docker Hub
- Deploys the latest application to AWS EC2

## Docker

- Containerizes frontend and backend services
- Uses Docker Compose for multi-container deployment

## Kubernetes

- Provides deployment manifests
- Includes Deployments, Services, Namespace, and MySQL StatefulSet

## AWS EC2

- Hosts the Dockerized application
- Receives automated deployments through GitHub Actions

---

# 📋 Prerequisites

- Git
- Docker & Docker Compose
- GitHub Account
- Docker Hub Account
- AWS Account
- Ubuntu EC2 Instance
- Kubernetes (Kind / Minikube)

---

# 📸 Screenshots

Screenshots will be added as the project progresses.

| Screenshot | Description |
|------------|-------------|
| GitHub Actions | CI/CD Workflow |
| Docker Images | Build Process |
| Docker Hub | Published Images |
| AWS EC2 | Running Containers |
| Kubernetes | Running Pods |
| Application | Homepage |

---

# 🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

- Building CI/CD pipelines using GitHub Actions
- Containerizing applications with Docker
- Managing multi-container deployments using Docker Compose
- Deploying applications to AWS EC2
- Working with Kubernetes manifests
- Using GitHub Secrets for secure deployments
- Automating software delivery workflows
- Following DevOps best practices

---

# 🚀 Future Enhancements

- Integrate automated unit testing
- Deploy the application on Amazon EKS
- Provision infrastructure using Terraform
- Add Prometheus & Grafana monitoring
- Implement Helm Charts
- Configure Kubernetes Ingress Controller
- Adopt GitOps using Argo CD

---

# 👩‍💻 Author

## Neha Sunil Pawar

**AWS Certified Solutions Architect – Associate**

Passionate about AWS Cloud, DevOps, Linux, Docker, Kubernetes, and CI/CD automation.

**GitHub:** https://github.com/Nehaa3004

---
