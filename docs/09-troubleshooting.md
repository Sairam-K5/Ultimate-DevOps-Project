# Troubleshooting

## Terraform Issues
- S3 backend errors → ensure bucket exists.
- IAM failures → verify correct permissions.

## Kubernetes Issues
- Pods stuck in CrashLoopBackOff → check logs and env variables.
- ALB not created → verify Ingress annotations and controller.

## CI/CD Issues
- GitHub Actions failing → check Docker/login or AWS credentials.
- Argo CD out of sync → ensure manifests updated with correct image tag.

## DNS Issues
- Domain not resolving → propagation may take up to 24 hrs or nameservers not mapped correctly.

