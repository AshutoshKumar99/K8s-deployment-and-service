# Python Web Application Deployment with Docker and Kubernetes, Create K8s Deployment and Service, deploy this docker application as a deployment on k8s cluster.

This repository contains files necessary to deploy a Python web application using Docker and Kubernetes.
## Instructions

1. **Dockerfile**: This file contains instructions to build a Docker image for the Python web application.
2. **Kubernetes Deployment (deployment.yaml)**: This YAML file describes how to deploy your application on Kubernetes, including the number of replicas and the Docker image to use.
3. **Kubernetes Service (service.yaml)**: This YAML file defines a Kubernetes service to expose your application outside of the cluster.

To deploy your application:

1. Ensure you have Docker installed and Kubernetes configured.
2. Build the Docker image using the provided Dockerfile.
3. Push the Docker image to a registry accessible to your Kubernetes cluster.
4. Apply the deployment and service files using `kubectl apply -f deployment.yaml` and `kubectl apply -f service.yaml`.
5. Access your application via the NodePort defined in the service configuration.
