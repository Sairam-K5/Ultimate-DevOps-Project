## About This Project
This project is based on the **OpenTelemetry Demo** repository.

Original repository:
https://github.com/open-telemetry/opentelemetry-demo
License: **Apache License 2.0**

This version has been modified and used for learning and experimentation purposes.

---


# Ultimate DevOps Project – Microservices + Observability + CI/CD

A complete, production-style DevOps showcase built using the OpenTelemetry Astronomy Shop microservices application, 
extended with containerization, Kubernetes, CI/CD automation, GitOps readiness, and Infrastructure as Code (Terraform).



## What This Project Demonstrates

- Microservices architecture (multi-language: Python, Go, Java, Node, Rust)
- Docker containerization for every service
- Kubernetes deployment with production-style manifests
- GitHub Actions CI pipeline
- Docker Compose for local + integration testing
- GitOps-ready structure (ArgoCD compatible)
- Infrastructure-as-Code using Terraform (folder included)
- Deployment-ready for EKS / cloud clusters

## Tech Stack

**Languages:** Python, Java, Go, Node, Rust
**DevOps Tools:** Docker, Kubernetes, Terraform, GitHub Actions, ArgoCD
**Cloud-Ready:** EKS-compatible manifests, IaC-ready Terraform
**Local Runtime:** Docker Compose (minimal + full stacks)
**CI/CD:** Automated build → test → image push → deployment-ready artifacts


# Quick Start

## Run locally using Docker Compose

```bash
docker-compose up --build
```

## Kubernetes & Cloud Deployment

Features:
- Deployment, Service, ConfigMap, Ingress manifests
- Ready for any CNCF-compliant cluster (EKS, GKE, AKS, Minikube, Kind)
- Auto-scalable microservice patterns

## EKS-ready
Add the values to Terraform and deploy EKS directly.

## Networking

- Kubernetes Services (ClusterIP)
- Ingress controller support (Nginx/ALB)
- DNS-ready architecture (Route53 recommended)

## Deploy to Kubernetes

```bash
kubectl apply -f kubernetes/complete-deploy.yaml #(complete yaml deployment file for all micro-services)
```
```bash
kubectl get pods
```

## CI/CD Overview

This project uses GitHub Actions to:

1. Checkout repo
2. Build microservices
3. Run unit/integration tests
4. Build Docker images
5. Push images to registry
6. Prepare K8s deployment artifacts
7. Trigger ArgoCD for GitOps deployment

Workflows file in: `.github/workflows/`

## Infrastructure as Code (Terraform)

A complete Terraform scaffold is included under terraform/:

- provider.tf – AWS provider setup
- backend.tf – S3 + DynamoDB state backend
- variables.tf – configurable project variables
- main.tf – root infrastructure logic
- outputs.tf – export cluster/domain outputs
- modules/ – extendable VPC/EKS modules

##Terraform Commands

```bash
cd terraform
terraform init
terraform plan
terraform apply
```


## Repository Structure

<pre>
.
├── src/                      # Microservices
├── kubernetes/               # K8s manifests
├── docs/                     # Documentation & diagrams
├── docker-compose.yml
├── docker-compose.minimal.yml
├── .github/workflows/        # CI/CD pipelines
├── terraform/                # Infrastructure as Code (Terraform)
│   ├── README.md
│   ├── backend.tf            # Optional : reusable modules (s3,Dynamo DB)
│   ├── variables.tf
│   ├── main.tf
│   ├── outputs.tf
│   └── modules/              # Optional: reusable modules (vpc, eks)
└── test/                     # Integration tests

</pre>

---

# Documentation Index

This project contains detailed technical documentation for every DevOps component implemented.  
For complete walkthroughs, screenshots, architecture diagrams, and explanations, please refer to the **[`docs/`](./docs/)** folder.

The documentation covers:

- **Architecture Overview**
- **Infrastructure Details (Terraform + AWS)**
- **CI/CD Pipeline (GitHub Actions)**
- **GitOps with ArgoCD**
- **Microservices Overview**
- **Kubernetes (EKS) Notes**
- **Networking & DNS (VPC, ALB, Route53)**
- **Deployment Guide**
- **Docker Containerization Overview**
- **Troubleshooting**
- **Application UI Screenshots**

Each document includes real execution screenshots to prove the implementation and workflow.



# What This Project Demonstrates About Me

This project highlights my hands-on DevOps skills and end-to-end understanding of modern cloud-native systems:

- Designing and deploying **multi-language microservices** architectures
- Strong expertise with **Docker** and **Kubernetes** (EKS)
- Building **CI/CD pipelines** using GitHub Actions
- Implementing **GitOps** using ArgoCD for fully automated deployments
- Writing production-grade **Kubernetes manifests**
- Creating scalable cloud infrastructure using **Terraform**
- Applying **AWS networking concepts** like VPC, Subnets, Route53 & ALB
- Clear professional documentation and architectural thinking
- Experience with **observability**, distributed tracing, and reliability engineering
- Ability to work with real DevOps workflows used in modern engineering teams


---

## License & Attribution

This project is derived from the OpenTelemetry Demo:
https://github.com/open-telemetry/opentelemetry-demo

Licensed under the **Apache License, Version 2.0**.

All original copyrights and license terms are preserved.

---
