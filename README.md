# 🚀 Production-Grade Kubernetes Cluster with Observability

A complete reference architecture for deploying and managing a production-grade Kubernetes cluster on AWS using GitOps, monitoring, and centralized logging.

## 🛠️ Tech Stack

- **Kubernetes** on EKS
- **Terraform** for Infra provisioning
- **ArgoCD** for GitOps
- **Prometheus + Grafana** for monitoring
- **Loki + Fluent Bit** for logs
- **Sealed Secrets** for secure secret management

## 📊 Architecture

![Architecture](architecture/diagrams.png)

## 📁 Repo Structure

k8s-prod-cluster-observability/
├── README.md
├── architecture/
│   └── diagrams.png
├── terraform/
│   └── eks-cluster.tf
├── helm/
│   ├── prometheus/
│   ├── grafana/
│   ├── loki/
│   └── argocd/
├── manifests/
│   └── demo-app/
├── argocd/
│   └── apps/
├── scripts/
│   └── bootstrap.sh
├── .github/workflows/
│   └── ci.yaml
└── docs/
    └── setup-guide.md


## 🚀 Getting Started

```bash
cd terraform
terraform init
terraform apply
