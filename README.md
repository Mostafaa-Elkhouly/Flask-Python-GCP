# Project Title

## Flask Web App on Google Kubernetes Engine (GKE)

This project demonstrates the deployment of a simple Python Flask web application on Google Kubernetes Engine (GKE). The project consists of the following key steps:

1. **Create a Simple Python Flask Web App**:
   - Develop a basic Python Flask web application that prints "Hello from GKE."

2. **Create an Artifact Repository**:
   - Set up an Artifact Repository named "my-images" to store Docker images used for the application.

3. **Dockerize the Application**:
   - Containerize the Flask application using Docker.

4. **Push Docker Image to "my-images"**:
   - Push the Docker image of the Flask application to the "my-images" Artifact Repository.

5. **Enable Vulnerability Scanner**:
   - Enable a vulnerability scanner to identify and fix any security vulnerabilities in the Docker image.
   
6. **Create a "Private" GKE Deployment**:
   - Deploy the Flask application to a "private" standard GKE cluster.
   - Configure the deployment with 2 replicas using the previously built Docker image.
   - Expose the deployment using a LoadBalancer service type.

7. **Restrict GKE Cluster Control Plane Communication**:
   - Secure the GKE cluster by limiting control plane communication to your localhost only.
   - Utilize authorized networks to achieve this security configuration.

8. **Create an Autopilot Mode Cluster**:
   - Set up an Autopilot mode GKE cluster, a fully managed Kubernetes environment.
   - Deploy a simple NGINX application within the Autopilot mode cluster.
   - Expose the NGINX deployment using a LoadBalancer service type.

## Prerequisites

Before you begin, ensure that you have the following prerequisites in place:

- Google Cloud Platform (GCP) account.
- GKE cluster provisioning and management access.
- Docker installed on your local machine.
