# Kurbenetes_lab
Widgetario Kubernetes Project - README

 Overview
This project demonstrates the deployment and management of a microservices-based application using Kubernetes. It covers essential components such as deployments, services, secrets, config maps, ingress, and monitoring using Prometheus and Grafana.
Each part of the project corresponds to a step-by-step build-up of the system architecture.
Repository Structure
widgetario-k8s/
├── Part1/               # Basic deployment of product service
├── Part2/               # Configuration using ConfigMaps and Secrets
├── Part3/               # MongoDB StatefulSet and database service
├── Part4/               # Ingress resources and reverse proxy setup
├── Part5/               # Troubleshooting and scaling setup
├── Part6/               # Monitoring using Prometheus and Grafana
└── README.md            # Project overview and usage instructions

 Technologies & Tools Used
- Kubernetes 
- kubectl
- Docker
- MongoDB (StatefulSet)
- Ingress-NGINX Controller
- Prometheus & Grafana
- Node.js (API layer)
- YAML for Kubernetes manifests
Installation Instructions
1. Clone the Repository

git clone   https://github.com/JoyAndati/Kurbenetes.git
cd widgetario-k8s

2. Apply Each Part (1 to 6)

kubectl apply -f Part1/
kubectl apply -f Part2/
kubectl apply -f Part3/
kubectl apply -f Part4/
kubectl apply -f Part5/
kubectl apply -f Part6/

 Usage
Once deployed, you can:
- Access the application using the Ingress hostname.
- Monitor metrics through Prometheus and Grafana dashboards (Part6).
- Use kubectl get pods  for troubleshooting.
 Testing
Although automated test cases are not included in this version, you can test manually by:
- Checking service availability via browser or curl.
- Ensuring all pods are in Running state:

kubectl get pods

- Confirming Ingress routing by accessing the domain in a browser 
Deployment Instructions
- Ensure your cluster is up and running.
- Apply manifests in order as described in the installation section.
- Use `kubectl port-forward`, or ingress URLs to access services.
 Media & Visuals
You may include screenshots or video walkthroughs of:
- The deployed UI
- Prometheus and Grafana dashboards
- Terminal showing pods running successfully

Secrets & Security
Sensitive data such as database credentials are managed using Kubernetes Secrets in Part2/.
