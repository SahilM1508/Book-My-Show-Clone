# 🎬 BookMyShow Clone – End-to-End DevSecOps CI/CD Pipeline on AWS EKS

## 🚀 Project Overview

This project demonstrates a complete **DevSecOps CI/CD implementation** using a BookMyShow Clone application.

The application is integrated with modern DevOps and Cloud-Native tools to automate:

* Source Code Management
* Continuous Integration
* Code Quality Analysis
* Security Scanning
* Containerization
* Continuous Deployment
* Kubernetes Orchestration
* Infrastructure Monitoring

The application is deployed on **Amazon EKS (Elastic Kubernetes Service)** and monitored using **Prometheus + Grafana**.

---

## 🏗️ Architecture

```text
GitHub
   │
   ▼
Jenkins Pipeline
   │
   ├── SonarQube Analysis
   ├── Quality Gate
   ├── Trivy Security Scan
   ├── Docker Build
   └── Docker Push
          │
          ▼
     Amazon EKS
          │
          ▼
 Kubernetes Deployment
          │
          ▼
 LoadBalancer Service
          │
          ▼
   BookMyShow Application

Monitoring Stack
----------------
Node Exporter
      │
      ▼
 Prometheus
      │
      ▼
  Grafana
```

---

## 🛠️ Tech Stack

### Cloud

* AWS EC2
* AWS EKS
* AWS Elastic Load Balancer

### DevOps Tools

* Jenkins
* Docker
* Kubernetes
* SonarQube
* Trivy
* Prometheus
* Grafana
* Node Exporter
* cAdvisor

### SCM

* Git
* GitHub

### Frontend

* ReactJS
* JavaScript
* HTML
* CSS

---

## ⚙️ CI/CD Pipeline Workflow

### Jenkins Stages

```text
✔ Clean Workspace
✔ Checkout Code
✔ SonarQube Analysis
✔ Quality Gate Validation
✔ Install Dependencies
✔ Trivy File System Scan
✔ Docker Build
✔ Docker Push
✔ Deploy to Kubernetes
✔ Post Actions
```

---

## 🔍 Code Quality Analysis

### SonarQube

SonarQube performs:

* Bug Detection
* Code Smell Analysis
* Vulnerability Detection
* Maintainability Checks
* Quality Gate Validation

---

## 🔐 Security Scanning

### Trivy

Trivy is used to scan:

* Source Code
* Dependencies
* Docker Images

Example:

```bash
trivy image <image-name>
```

---

## 🐳 Docker Containerization

Build Image

```bash
docker build -t bookmyshow .
```

Push Image

```bash
docker push <dockerhub-username>/bookmyshow
```

---

## ☸️ Kubernetes Deployment

Deploy Application

```bash
kubectl apply -f deployment.yaml
```

Deploy Service

```bash
kubectl apply -f service.yaml
```

Verify Resources

```bash
kubectl get pods
kubectl get svc
kubectl get nodes
```

---

## 📊 Monitoring Setup

### Prometheus

Prometheus collects metrics from:

* Node Exporter
* cAdvisor
* Kubernetes Components

Access:

```text
http://<SERVER-IP>:9090
```

---

### Grafana

Grafana visualizes metrics through dashboards.

Access:

```text
http://<SERVER-IP>:3001
```

Default Credentials:

```text
Username: admin
Password: admin
```

---

### Node Exporter

Monitored Metrics:

* CPU Usage
* Memory Usage
* Disk Utilization
* Network Traffic
* System Uptime

Port:

```text
9100
```

---

### cAdvisor

Container Metrics:

* CPU Usage
* Memory Usage
* Network Usage
* Filesystem Usage

Port:

```text
8081
```

---

## 📈 Monitoring Dashboard

The Grafana dashboard displays:

### System Monitoring

* CPU Usage
* Memory Usage
* Disk Usage
* Network Traffic
* Uptime

### Container Monitoring

* Container CPU
* Container Memory
* Container Network
* Container Health

### Kubernetes Monitoring

* Nodes
* Pods
* Services
* Cluster Health

---

## 📷 Project Screenshots

### Application Dashboard

![Application](screenshots/application.png)

### Jenkins Pipeline

![Jenkins](screenshots/jenkins.png)

### SonarQube Analysis

![SonarQube](screenshots/sonarqube.png)

### Grafana Monitoring

![Grafana](screenshots/grafana.png)

### Kubernetes Cluster

![Kubernetes](screenshots/kubernetes.png)

---

## 🎯 Learning Outcomes

This project helped in understanding:

* CI/CD Automation
* Docker Containerization
* Kubernetes Deployments
* AWS EKS Management
* SonarQube Quality Gates
* Trivy Security Scanning
* Prometheus Monitoring
* Grafana Visualization
* DevSecOps Best Practices

---

## 🔮 Future Enhancements

* ArgoCD GitOps Deployment
* Helm Charts
* Terraform Infrastructure Automation
* Slack Notifications
* Alertmanager Integration
* CloudWatch Monitoring

---

## 👨‍💻 Author

**Sahil Mahadik**

M.Sc Computer Science | DevOps Enthusiast

GitHub: https://github.com/SahilM1508

LinkedIn: https://www.linkedin.com/in/sahil-mahadik-27b2812a1/

---

## 🙏 Acknowledgement

Special thanks to **Kastrov Kiran** for the DevOps learning resources, project guidance, and practical implementation knowledge that helped in building this end-to-end DevSecOps project.

---

⭐ If you found this project useful, please Star the repository.
