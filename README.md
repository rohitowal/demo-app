# Java Hello World — DevOps Project

A simple Java Hello World application created to learn and practice DevOps concepts using Git, Docker, Docker Hub, Kubernetes, and Argo CD.

## Project Overview

This project demonstrates the end-to-end workflow of containerizing a Java application, publishing a Docker image, deploying it to Kubernetes, and managing the deployment using Argo CD and GitOps principles.

## Technologies Used

- **Java 21** — Application development
- **Git & GitHub** — Source code management
- **Docker** — Containerization
- **Docker Hub** — Docker image registry
- **Kubernetes** — Container orchestration
- **Argo CD** — GitOps-based continuous delivery
- **AWS** — Future extension for cloud deployment

## Project Structure

```text
java-hello-world/
├── src/
│   └── HelloWorld.java
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
├── Dockerfile
├── .dockerignore
├── .gitignore
└── README.md
```

## Application

The application displays a simple `Hello World!` response using Java's built-in HTTP server.

**Endpoint:** `/`

**Port:** `8080`

## Learning Objectives

### 1. Git and GitHub
- Create a GitHub repository.
- Clone the repository locally.
- Track and commit source code changes.
- Push changes to GitHub.

### 2. Docker
- Understand Docker images and containers.
- Write a Dockerfile using a multi-stage build.
- Build and run a Docker image locally.
- Map container ports to host ports.

### 3. Docker Hub
- Create a Docker Hub repository.
- Tag Docker images.
- Push images to a remote registry.
- Pull images for deployment.

### 4. Kubernetes
- Deploy the application using a Kubernetes Deployment.
- Run multiple replicas of the application.
- Expose the application using a Service.
- Configure readiness and liveness probes.
- Explore scaling, logs, and self-healing.

### 5. Argo CD and GitOps
- Store Kubernetes manifests in GitHub.
- Connect a Git repository to Argo CD.
- Synchronize Kubernetes resources from Git.
- Understand automated synchronization and self-healing.
- Deploy application updates through Git changes.

### 6. AWS (Future Enhancement)
- Store container images in Amazon ECR.
- Deploy workloads to Amazon EKS.
- Explore IAM, VPC networking, load balancing, and CloudWatch.

## Expected Workflow

```text
Java Source Code
       |
       v
   Docker Build
       |
       v
  Docker Image
       |
       v
   Docker Hub
       |
       v
   Kubernetes
       ^
       |
     Argo CD
       ^
       |
    GitHub
  (GitOps Repository)
```

## Project Goal

The goal of this project is to understand how a Java application moves from source code to a containerized application running in Kubernetes, with deployment configuration managed through GitOps using Argo CD.

This project will be extended gradually to include automated image builds, versioned deployments, and AWS integration as part of the DevOps learning journey.
