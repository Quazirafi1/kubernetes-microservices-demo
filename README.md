# Microservices Demo with Docker, Kubernetes, and GKE

This project demonstrates the complete deployment workflow of a microservices architecture using Docker and Kubernetes on Google Kubernetes Engine (GKE).  
It features two Spring Boot microservices **Currency Exchange** and **Currency Conversion** with inter-service communication and dynamic service discovery.

The goal of this project is to provide hands-on experience with containerization, orchestration, and cloud-native deployment practices.

---

## ✨ Project Highlights

- **Containerized** the Java Spring Boot applications using Docker.
- **Built and pushed** Docker images to a personal Docker Hub repository.
- **Deployed** microservices to a GKE (Google Kubernetes Engine) cluster using Kubernetes Deployments and Services.
- **Exposed** services using Kubernetes **NodePort** for internal networking.
- **Configured Ingress** for clean URL routing across microservices.
- **Managed configurations** dynamically using Kubernetes **ConfigMaps**.
- **Followed best practices** for resource requests/limits, readiness probes, and liveness probes.

---

## 🔗 Sample API Calls (Local Setup)

- **Currency Exchange Service**  
  `http://localhost:8000/currency-exchange/from/USD/to/INR`

- **Currency Conversion Service**  
  `http://localhost:8100/currency-conversion/from/EUR/to/INR/quantity/10`

---

## 📡 Access via Ingress (GKE Deployment)

Once deployed on GKE and Ingress is active, API calls can be made through the Ingress public IP:

- **Currency Exchange Service**  
  `http://<INGRESS-IP>/currency-exchange/from/USD/to/INR`

- **Currency Conversion Service**  
  `http://<INGRESS-IP>/currency-conversion/from/EUR/to/INR/quantity/10`

> **Note:** Replace `<INGRESS-IP>` with the external IP address assigned to your Ingress.

---

## 📄 Note

The Java springboot applications used in this project are based on publicly available open-source examples.  
The primary contribution of this project lies in:
- Containerizing the applications
- Designing Kubernetes deployments and services
- Setting up service discovery and external access through Ingress
- Deploying and managing microservices on GKE
