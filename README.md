<div align="center">

# 🚀 Azure Container Platform

### End-to-End Azure DevOps Implementation using Terraform, Docker and GitHub Actions

<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=24&pause=1200&color=0078D4&center=true&vCenter=true&width=850&lines=Infrastructure+as+Code+with+Terraform;Containerized+Applications+using+Docker;CI%2FCD+using+GitHub+Actions;Azure+Container+Apps+Deployment;Monitoring+with+Application+Insights" />
</p>

<p align="center">

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=for-the-badge&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask)

</p>

<p align="center">

![Deployment](https://github.com/darshanthenge03-cloud/azure-container-platform/actions/workflows/deploy.yml/badge.svg)

</p>

</div>

---

# 📖 Project Overview

This project demonstrates a complete Azure DevOps implementation using modern cloud-native technologies.

The solution provisions Azure infrastructure using Terraform, containerizes a Flask-based web application using Docker, stores images within Azure Container Registry, and deploys applications automatically to Azure Container Apps using GitHub Actions.

The application itself is designed as an Azure DevOps Dashboard that visually represents the deployment platform, cloud architecture, and CI/CD workflow used throughout the project.

---

# 🌐 Application Dashboard

The dashboard provides a visual representation of the cloud platform and deployment architecture.

Features include:

- Responsive Bootstrap UI
- Azure-themed design
- Technology stack overview
- Deployment information
- Environment status
- Monitoring integration details
- Health endpoint
- Containerized deployment

---

# 🏗 Architecture

```mermaid
flowchart TD

A[Developer] --> B[GitHub Repository]

B --> C[GitHub Actions]

C --> D[Docker Build]

D --> E[Azure Container Registry]

E --> F[Azure Container Apps]

F --> G[Application Insights]

F --> H[Log Analytics Workspace]

F --> I[Public HTTPS Endpoint]
```

---

# 🔄 CI/CD Workflow

```mermaid
flowchart LR

A[Code Change] --> B[Git Commit]

B --> C[Git Push]

C --> D[Manual Workflow Trigger]

D --> E[GitHub Actions]

E --> F[Build Docker Image]

F --> G[Push Image to ACR]

G --> H[Deploy Container App]

H --> I[Application Updated]
```

---

# ☁ Azure Resources

| Resource | Purpose |
|---------|----------|
| Resource Group | Resource Organization |
| Azure Container Registry | Docker Image Storage |
| Log Analytics Workspace | Centralized Logging |
| Application Insights | Application Monitoring |
| Container Apps Environment | Managed Runtime |
| Azure Container App | Application Hosting |

---

# 🛠 Technology Stack

| Category | Technologies |
|---------|-------------|
| Programming | Python, Flask |
| Frontend | HTML, Bootstrap |
| Containerization | Docker |
| Infrastructure | Terraform |
| Cloud Platform | Microsoft Azure |
| CI/CD | GitHub Actions |
| Monitoring | Application Insights |
| Logging | Log Analytics |
| Version Control | Git, GitHub |

---

# 📂 Repository Structure

```text
azure-container-platform
│
├── app
│   ├── app.py
│   ├── Dockerfile
│   ├── requirements.txt
│   └── templates
│       └── index.html
│
├── terraform
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── provider.tf
│
├── architecture
│
├── .github
│   └── workflows
│       └── deploy.yml
│
├── README.md
└── .gitignore
```

---

# ⚙ Infrastructure Deployment

Infrastructure provisioning is managed using Terraform.

```bash
terraform init

terraform plan

terraform apply
```

Resources are automatically provisioned within Azure.

---

# 🐳 Application Containerization

The Flask dashboard is containerized using Docker and stored within Azure Container Registry.

```bash
docker build -t devops-platform:v1 .

docker tag devops-platform:v1 darshanacr001.azurecr.io/devops-platform:v1

docker push darshanacr001.azurecr.io/devops-platform:v1
```

---

# 🚀 Deployment Process

The deployment workflow performs the following operations:

- Checkout source code
- Authenticate with Azure
- Build Docker image
- Push image to Azure Container Registry
- Deploy latest container image
- Update Azure Container App

The workflow is currently executed manually through GitHub Actions.

---

# 📈 Monitoring and Observability

### Application Insights

- Request Monitoring
- Performance Analysis
- Exception Tracking
- Application Telemetry

### Log Analytics

- Container Logs
- Deployment Logs
- Application Logs
- Troubleshooting Information

---

# 📸 Screenshots

## Azure DevOps Dashboard

![Dashboard](architecture/app-url1.png)

---

## Architecture Diagram

![Architecture](architecture/architecture.PNG)

---

## GitHub Actions Pipeline

![Pipeline](architecture/github-actions.png)

---

## Azure Resources

![Azure Resources](architecture/azure-resources.png)

---

# 🎯 Project Objectives

This project was created to gain practical experience with:

- Infrastructure as Code
- Containerized applications
- CI/CD implementation
- Azure cloud services
- Application monitoring
- Deployment automation
- DevOps workflows

---

# 🚀 Future Enhancements

Planned improvements include:

- Multi-environment deployments
- Remote Terraform backend
- AKS deployment
- Blue-Green deployment strategy
- Autoscaling rules
- Custom domains
- SSL certificates
- Environment approvals

---

# 💼 Project Outcome

This project demonstrates the implementation of an end-to-end Azure DevOps workflow using modern cloud-native services.

The solution combines Infrastructure as Code, containerization, CI/CD automation, application monitoring, and managed container hosting on Microsoft Azure.

The project was built to gain practical experience with real-world DevOps workflows and Azure platform services.

---

# 👨‍💻 Author

### Darshan Thenge

Cloud Engineer | Azure | Terraform | DevOps

GitHub:

https://github.com/darshanthenge03-cloud

LinkedIn:

https://www.linkedin.com/in/darshan-thenge-933394121/

---

<div align="center">
### ⭐ If you found this project interesting, please consider giving it a star.
</div>
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0078D4,100:623CE4&height=120&section=footer"/>
