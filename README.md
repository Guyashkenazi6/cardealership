# 🚗 Car Dealership App

Welcome to the Car Dealership App, a modern solution integrating a range of tools and platforms to deliver a top-tier car dealership experience.

## 🌟 Features

- **FastAPI Backend**: Built using the FastAPI framework, allowing dynamic API interactions.
- **Data Management**: Utilizing MongoDB, manage car stocks with CRUD operations.
- **Order & Payment**: Intuitive order system with VISA transaction integration.
- **Dual Services**: Comprising the primary Car Dealership and the VISA transaction service.

## 🛠️ Tech Stack

- Kubernetes
- Docker
- Google Cloud
- Azure DevOps
- ArgoCD
- MongoDB
- Python
- FastAPI

## 🔧 Deployment Details

1. **CI Pipeline**: Managed by Azure DevOps, which builds a Docker image and subsequently pushes it to DockerHub.
2. **CD & Deployment**: Leveraging ArgoCD for Continuous Deployment to a Kubernetes cluster within Google Cloud.
3. **Access**: Utilize the external IP courtesy of the Google Cloud load balancer.
4. **Ingress Services**: Separate ingress for the main app and VISA transaction interactions.

## 🚀 Getting Started

### Prerequisites
Ensure the installation of `kubectl`, `docker`, and `argocd` CLI tools.

```bash
git clone [repository-url]
cd [repository-name]
```

- Activate Azure DevOps pipeline for image creation and pushing to DockerHub.
- Use ArgoCD for deploying the app.

Access the deployed application via the Google Cloud LoadBalancer's external IP.

## 📘 API Endpoints

- **Car Dealership Site**: 
  - Supports GET, POST, PUT, DELETE for stock management.
  - POST order using `car_id` and `cardnumber` for processing transactions.
- **VISA Service**
  
## 🔗 Inter-service Connection

Upon a successful transaction, the VISA service relays a transaction ID and price, exemplifying the connectivity between services and MongoDB.

## 🙌 Acknowledgments

Gratitude to the open-source community and all technologies that have empowered this project.

