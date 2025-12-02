# Microservices Overview

The project consists of a multi-service architecture typical of modern E-commerce applications.

## Key Work Done
- Each service was containerized using Docker with production-ready Dockerfiles.
- Services were deployed as individual Kubernetes Deployments.
- ConfigMaps and Secrets were used for environment configuration.
- Services communicate via internal DNS within the EKS cluster.
- Horizontal scaling capabilities were enabled through Kubernetes.

This modularity simplifies CI/CD, scaling, debugging, and observability.
