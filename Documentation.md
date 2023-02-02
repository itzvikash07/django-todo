# Documentation of the Django Web Application 


## Introduction

This project aims to build a robust CI/CD pipeline for a Django application using Jenkins and to set up and manage
a Kubernetes cluster on AWS with Minikube. The project will cover the following areas:

- Building the CI/CD pipeline for the Django application using Jenkins
- Setting up and managing a Kubernetes cluster on AWS from scratch with Minikube Containerizing the Django application and deploying it in the Kubernetes cluster as pods
- Managing deployments, replications, auto-healing, and auto-scaling for the Kubernetes cluster
- Managing network and services with host IP allocation for the Kubernetes cluster


## Project Goals

The main goals of this DevOps project are to:

- Automate the deployment and scaling of Django applications
- Improve the reliability and stability of the delivery pipeline
- Streamline the development and release process
Enhance collaboration between development and operations teams Architecture
- Provide the Ability of Auto healing
- Reduce downtime by 70% using k8s.

### The project architecture consists of the following components:

 Github --> EC2 server --> Docker image --> Kuberenetes pod (Jenkins Pipeline)

 ## Implementation Details
The project will be implemented in several stages, including:

Stage 1: Developer push the code to Github repo.

Stage 2: A CI/CD pipeline which is configure on    Jenkins will pull the code of Github

Stage 3: In pipeline: This code will copy in server which is a AWS EC2 instance

Stage 4: In pipeline: Now docker comes in picture a Dockerfile configured for run this application and create a image of it.

Stage 5: In pipeline: Now the container of this image run in Kubernetes pods.

Stage 6: Manually allocate a host IP

## Project Outcome
At the end of this project, the following outcomes are Achieved:

- The Django application will be automatically deployed every time there is a change in the code

- The Kubernetes cluster will be set up and managed on AWS with Minikube, providing a scalable and reliable platform for the Django application

- The Django application will be deployed in the Kubernetes cluster as pods, providing a secure and isolated environment for each instance of the application

- The Kubernetes cluster will be configured for deployment, replication, auto-healing, and auto-scaling, ensuring high availability and reliability of the application

- The network and services for the Kubernetes cluster will be managed with host IP allocation,  providing a stable and secure communication between the different components of the cluster.