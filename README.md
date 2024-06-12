
# Reddit Clone App on Kubernetes with Ingress

This project demonstrates how to deploy a Reddit clone app on Kubernetes with Ingress and expose it to the world using Minikube as the cluster. Below is an overview of the architecture of this Reddit Clone App running on Kubernetes with Ingress.



# Prerequisites

Before you begin, you should have the following tools installed on your local machine:
Docker
Minikube cluster ( Running )
kubectl
Git

# Installation

Follow these steps to install and run the Reddit clone app on your local machine:
Clone this repository to your local machine: git clone https://github.com/VahiniPonnoju/Reddit-Clone-K8s-Ingress.git
Navigate to the project directory: cd reddit-clone-k8s-ingress
Build the Docker image for the Reddit clone app: docker build -t reddit-clone-app .
Deploy the app to Kubernetes: kubectl apply -f deployment.yaml
Deploy the Service for deployment to Kubernetes: kubectl apply -f service.yaml
Enable Ingress by using Command: minikube addons enable ingress
Expose the app as a Kubernetes service: kubectl expose deployment reddit-deployment --type=NodePort --port=3000
Create an Ingress resource: kubectl apply -f ingress.yaml

# Test Ingress DNS for the app:

Test Ingress by typing this command: curl http://domain.com/test

# BLOG DETAILS

You can read this blog for deploying the same https://vahiniponnoju.hashnode.dev/deployment-of-a-reddit-clone-application-with-ingress-enabled
