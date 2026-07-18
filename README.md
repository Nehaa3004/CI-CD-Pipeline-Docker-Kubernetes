# 🚀 Automated CI/CD Pipeline for a Dockerized 3-Tier Application

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5?logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Cloud-FF9900?logo=amazonaws&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Linux-Ubuntu-E95420?logo=ubuntu&logoColor=white)

> 🚧 **Project Status:** Ongoing

---
## 📌 Project Overview

This project demonstrates an automated CI/CD pipeline for a Dockerized three-tier web application using GitHub Actions, Docker, Kubernetes, and AWS. The primary objective is to automate the software delivery process from source code to deployment while following modern DevOps practices.

The application consists of a frontend, backend, and MySQL database. Every code change pushed to the GitHub repository automatically triggers a Continuous Integration (CI) workflow that builds Docker images and prepares them for deployment. After a successful build, the Continuous Deployment (CD) workflow deploys the latest application version to the target environment.

This repository is maintained as an ongoing DevOps learning project, with continuous improvements in automation, deployment strategies, and infrastructure management.


## ✨ Project Highlights

- Automated CI/CD pipeline using GitHub Actions
- Dockerized three-tier application architecture
- Multi-stage Docker image builds
- Continuous Integration for automated builds
- Continuous Deployment to target infrastructure
- Kubernetes manifests for container orchestration
- Docker Compose for local development
- MySQL database integration
- AWS EC2 deployment
- Infrastructure automation following DevOps best practices

## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| CI/CD | GitHub Actions |
| Containers | Docker, Docker Compose |
| Orchestration | Kubernetes (Kind) |
| Cloud | AWS EC2 |
| Backend | Go (Gin Framework) |
| Frontend | HTML, CSS, JavaScript, Nginx |
| Database | MySQL |
| Version Control | Git & GitHub |
| Operating System | Ubuntu Linux |

## 🏗️ Solution Architecture

<p align="center">
  <img src="architecture/architecture.png" alt="CI/CD Pipeline Architecture" width="100%">
</p>

The following diagram illustrates the end-to-end CI/CD workflow for the Dockerized three-tier application. Every code push triggers an automated GitHub Actions pipeline that builds Docker images, publishes them to Docker Hub, and deploys the latest version to AWS EC2. The project also includes Kubernetes manifests for deploying the application on a local Kind cluster.

## 🔄 CI/CD Workflow

The project follows an automated Continuous Integration and Continuous Deployment (CI/CD) workflow.

```text
Developer
    │
    │ Git Push
    ▼
GitHub Repository
    │
    ▼
GitHub Actions (CI)
    │
    ├── Checkout Source Code
    ├── Build Docker Images
    ├── Tag Images
    └── Push Images to Docker Hub
                │
                ▼
GitHub Actions (CD)
                │
                ├── Connect to AWS EC2 (SSH)
                ├── Pull Latest Docker Images
                └── Restart Application Containers
                │
                ▼
      Running Dockerized Application
```

### Continuous Integration (CI)

The CI workflow automatically executes whenever changes are pushed to the main branch.

- Checks out the latest source code
- Builds backend and frontend Docker images
- Tags images using the latest and commit SHA
- Pushes Docker images to Docker Hub

### Continuous Deployment (CD)

After a successful CI pipeline, the deployment workflow automatically:

- Connects to the deployment server
- Pulls the latest Docker images
- Updates running containers using Docker Compose
- Deploys the latest application version with minimal downtime

## 🚀 Key Features

- Automated CI/CD using GitHub Actions
- Dockerized frontend and backend services
- Multi-stage Docker builds
- Docker Compose for local development
- Kubernetes deployment manifests
- AWS EC2 deployment
- Automated Docker image publishing
- Secure credential management using GitHub Secrets
- Version-controlled infrastructure configuration
- Scalable three-tier application architecture

## ⚙️ Key Components

### GitHub Actions
- Automates Continuous Integration and Continuous Deployment.
- Builds and tags Docker images.
- Pushes images to Docker Hub.
- Deploys updated application to AWS EC2.

### Docker
- Containerizes frontend and backend services.
- Uses Docker Compose for multi-container deployment.

### Kubernetes
- Provides deployment manifests for running the application on a Kubernetes cluster.
- Includes Deployments, Services, Namespace, and MySQL configuration.

### AWS EC2
- Hosts the Dockerized application.
- Receives automated deployments through GitHub Actions.

## ✨ Features

- Automated CI/CD using GitHub Actions
- Dockerized multi-container application
- Docker Compose deployment
- Kubernetes-ready manifests
- AWS EC2 deployment
- Docker Hub image registry
- Secure GitHub Secrets integration
- Three-tier application architecture
- Continuous deployment automation

## 📋 Prerequisites

- Git
- Docker & Docker Compose
- GitHub Account
- Docker Hub Account
- AWS Account
- Ubuntu EC2 Instance
- Kubernetes (Kind or Minikube)

## 📸 Screenshots

Screenshots will be added as the project progresses.

| Screenshot | Description |
|------------|-------------|
| GitHub Actions | CI/CD workflow execution |
| Docker Images | Successfully built images |
| Docker Hub | Published container images |
| AWS EC2 | Running application |
| Kubernetes | Deployed workloads |

## 🎯 Learning Outcomes

Through this project, I gained practical experience in:

- Designing CI/CD pipelines using GitHub Actions
- Containerizing applications with Docker
- Managing multi-container deployments using Docker Compose
- Deploying applications on AWS EC2
- Working with Kubernetes manifests
- Automating software delivery workflows
- Managing secrets securely in GitHub Actions


## 🚀 Future Enhancements

- Implement automated testing in CI pipeline
- Deploy to Amazon EKS
- Integrate Terraform for infrastructure provisioning
- Add monitoring with Prometheus & Grafana
- Implement Helm Charts
- Configure Ingress Controller

## 👩‍💻 Author

**Neha Sunil Pawar**

AWS Certified Solutions Architect – Associate

Passionate about Cloud Computing, DevOps, AWS, Docker, Kubernetes, and CI/CD Automation.