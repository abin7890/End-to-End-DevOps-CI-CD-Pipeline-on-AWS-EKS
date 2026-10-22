
# 🚀 End-to-End DevSecOps CI/CD Pipeline on AWS

![DevOps](https://img.shields.io/badge/DevOps-CI%2FCD-blue)
![Jenkins](https://img.shields.io/badge/Jenkins-Automation-red)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5)
![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![Terraform](https://img.shields.io/badge/Terraform-IaC-purple)

## 📌 Project Overview

This project demonstrates an **End-to-End DevSecOps CI/CD Pipeline** that automates the process of building, testing, analyzing, securing, containerizing, and deploying a Java-based application using modern DevOps tools and AWS cloud infrastructure.

The project integrates **Jenkins, GitHub, Maven, SonarQube, Trivy, Docker, Terraform, Kubernetes, AWS Elastic Load Balancer, Prometheus, and Grafana** to demonstrate a complete application delivery workflow.

The main objective is to implement DevSecOps practices by integrating continuous integration, continuous delivery, security scanning, infrastructure automation, container orchestration, and monitoring into a unified workflow.

---

## 🏗️ Project Architecture

The architecture follows a DevSecOps workflow:

```text
                   Developer
                       |
                       v
                    GitHub
                       |
                       v
                    Jenkins
                       |
                       v
               Source Code Checkout
                       |
                       v
              SonarQube Analysis
                       |
                       v
                Maven Build
                       |
                       v
                Docker Build
                       |
                       v
               Trivy Image Scan
                       |
                       v
              Docker Container Image
                       |
                       v
               Kubernetes Deployment
                       |
                       v
              AWS Elastic Load Balancer
                       |
                       v
                Application UI

Infrastructure Provisioning:
GitHub --> Terraform --> AWS Infrastructure
                              |
                              v
                       Kubernetes Cluster

Monitoring:
Kubernetes --> Prometheus --> Grafana
```

The architecture combines automated application delivery, infrastructure provisioning, and monitoring.

---

## 🛠️ Technology Stack

| Category | Tools & Technologies |
|----------|----------------------|
| Cloud Platform | Amazon Web Services (AWS) |
| Version Control | Git, GitHub |
| CI/CD Automation | Jenkins |
| Infrastructure as Code | Terraform |
| Code Quality Analysis | SonarQube |
| Security Scanning | Trivy |
| Build Automation | Apache Maven |
| Containerization | Docker |
| Container Orchestration | Kubernetes |
| Load Balancing | AWS Elastic Load Balancer |
| Monitoring | Prometheus |
| Visualization | Grafana |
| Application | Java-based Application |

---

## ⚙️ CI/CD Pipeline Workflow

### 1️⃣ Source Code Management – GitHub

- Application source code is maintained in a GitHub repository.
- Jenkins retrieves the source code from GitHub.
- Git provides version control and supports collaborative development.

### 2️⃣ Continuous Integration – Jenkins

Jenkins acts as the central automation server responsible for orchestrating the CI/CD workflow.

**Responsibilities:**

- Retrieve application source code.
- Execute pipeline stages.
- Integrate code quality and security checks.
- Build application artifacts.
- Automate Docker image creation.
- Coordinate application deployment.

### 3️⃣ Code Quality Analysis – SonarQube

SonarQube performs static code analysis to identify potential code quality issues.

**Key capabilities:**

- Detect code smells.
- Identify potential bugs.
- Highlight security-related issues.
- Analyze maintainability.
- Provide code quality reports.

This helps identify potential issues before deployment.

### 4️⃣ Security Scanning – Trivy

Trivy is integrated into the workflow to identify known security vulnerabilities.

**Security checks include:**

- Filesystem vulnerability scanning.
- Container image vulnerability scanning.
- Detection of vulnerable software dependencies.

Integrating Trivy helps introduce security checks earlier in the software delivery lifecycle.

### 5️⃣ Application Build – Maven

Apache Maven manages the build process for the Java application.

**Responsibilities:**

- Resolve project dependencies.
- Compile Java source code.
- Execute configured tests.
- Package application artifacts.

Example Maven command:

```bash
mvn clean package
```

### 6️⃣ Containerization – Docker

Docker packages the application and its required runtime dependencies into a container image.

**Benefits:**

- Consistent application runtime.
- Portability across environments.
- Simplified deployment.
- Efficient container management.

Example commands:

```bash
docker build -t devsecops-app:latest .
```

```bash
docker images
```

### 7️⃣ Infrastructure Provisioning – Terraform

Terraform is used to define and provision AWS infrastructure using Infrastructure as Code (IaC).

**Benefits:**

- Declarative infrastructure configuration.
- Repeatable infrastructure provisioning.
- Version-controlled infrastructure definitions.
- Reduced manual configuration.

Common Terraform commands:

```bash
terraform init
```

```bash
terraform plan
```

```bash
terraform apply
```

### 8️⃣ Container Orchestration – Kubernetes

Kubernetes manages the deployment and execution of containerized applications.

**Capabilities:**

- Container orchestration.
- Pod scheduling.
- Service discovery.
- Application scaling.
- Self-healing of workloads.
- Rolling updates.

Useful Kubernetes commands:

```bash
kubectl get nodes
```

```bash
kubectl get pods
```

```bash
kubectl get deployments
```

```bash
kubectl get services
```

### 9️⃣ Application Exposure – AWS Elastic Load Balancer

AWS Elastic Load Balancer provides an endpoint for accessing the deployed application.

**Benefits:**

- Distributes incoming application traffic.
- Provides a stable application endpoint.
- Supports application availability.

Users access the deployed application through the configured Load Balancer endpoint.

### 🔟 Monitoring – Prometheus & Grafana

Prometheus and Grafana provide monitoring and visualization capabilities for the deployed environment.

**Prometheus:**

- Collects metrics from configured monitoring targets.
- Stores time-series monitoring data.
- Supports querying system and application metrics.

**Grafana:**

- Visualizes monitoring metrics.
- Provides customizable dashboards.
- Helps observe infrastructure and application performance.

Together, these tools improve visibility into the Kubernetes environment.

---

## 🔐 DevSecOps Practices

This project incorporates DevSecOps principles by introducing security and quality checks into the CI/CD workflow.

| Practice | Implementation |
|----------|----------------|
| Source Code Management | GitHub |
| Pipeline Automation | Jenkins |
| Static Code Analysis | SonarQube |
| Vulnerability Scanning | Trivy |
| Build Automation | Maven |
| Containerization | Docker |
| Infrastructure Automation | Terraform |
| Deployment Management | Kubernetes |
| Monitoring | Prometheus & Grafana |

The objective is to identify code quality and security issues before application deployment.

---

## ✨ Key Features

- Automated CI/CD workflow using Jenkins.
- GitHub integration for source code management.
- Static code analysis using SonarQube.
- Vulnerability scanning using Trivy.
- Automated Java application builds using Maven.
- Docker-based application containerization.
- AWS infrastructure provisioning using Terraform.
- Container orchestration using Kubernetes.
- Application exposure through AWS Elastic Load Balancer.
- Infrastructure and workload monitoring using Prometheus and Grafana.
- Integration of development, security, deployment, and monitoring practices.

---

## 📚 Key Learnings

Through this project, I gained hands-on experience with:

- Designing an end-to-end DevSecOps workflow.
- Building and managing Jenkins CI/CD pipelines.
- Integrating SonarQube and Trivy into application delivery.
- Building Java applications using Maven.
- Creating and managing Docker images.
- Provisioning AWS infrastructure with Terraform.
- Deploying containerized applications on Kubernetes.
- Configuring cloud load balancing.
- Monitoring Kubernetes environments using Prometheus and Grafana.
- Troubleshooting CI/CD and deployment-related issues.

---

## 🎯 Project Objective

The objective of this project is to demonstrate how DevOps and DevSecOps technologies can be integrated to streamline application delivery.

By combining CI/CD automation, security scanning, Infrastructure as Code, container orchestration, and monitoring, the project demonstrates practical concepts used in modern cloud-native application deployment workflows.

---

## 👨‍💻 Author

**Abin VA**

Aspiring DevOps Engineer | AWS | Docker | Kubernetes | Terraform | Jenkins | CI/CD

- **GitHub:** [github.com/abin7890](https://github.com/abin7890)
- **LinkedIn:** [Abin VA](https://www.linkedin.com/in/abin-va-37b502354)

---

⭐ If you found this project useful, consider giving the repository a star!
