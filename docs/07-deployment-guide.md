## 1. Provision AWS Infra (Terraform)
```bash
cd terraform
terraform init
terraform apply
```

## 2. Deploy Application on Kubernetes
```bash
kubectl apply -f kubernetes/complete-deploy.yml
```

## 3. CI/CD & GitOps
```bash
- GitHub Actions builds and pushes images on every commit.
- Argo CD auto-syncs deployments in EKS.
```

## 4. Access the Application
```bash
- Frontend is exposed via AWS ALB.
- DNS (Route53) points your domain → ALB DNS.
```
You now have a fully automated cloud-native DevOps environment.
