**Microservices Demo with Docker, Kubernetes, and GKE**: 
This project demonstrates the deployment of microservices using Docker and Kubernetes on Google Kubernetes Engine (GKE).
It includes two containerized Spring Boot services — Currency Exchange and Currency Conversion — featuring inter-service communication.
The project is designed for hands-on learning of cloud-native application development and orchestration.

Sample API Calls
Currency Exchange Service
http://localhost:8000/currency-exchange/from/USD/to/INR

Currency Conversion Service
http://localhost:8100/currency-conversion/from/EUR/to/INR/quantity/10

Note
The Java microservices used in this project are based on publicly available open-source examples.
The primary contribution of this work is containerizing the services using Docker, orchestrating them with Kubernetes, and deploying them on GKE.
