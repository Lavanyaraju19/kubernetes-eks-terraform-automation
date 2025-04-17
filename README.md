# kubernetes-eks-terraform-automation

Deploy a fully functional AWS EKS cluster with Terraform and manage applications using Kubernetes and Helm.

## 🚀 Features

- Provision EKS cluster on AWS using Terraform
- Create and configure VPC, subnets, IAM roles
- Deploy applications with `kubectl` and Helm
- Scalable and modular infrastructure setup

## 🧰 Tools Used

- Terraform
- AWS EKS
- Kubernetes
- Helm
- AWS CLI

## 📁 Folder Structure

├── terraform/ │ ├── main.tf │ ├── variables.tf │ └── outputs.tf ├── helm/ │ └── chart/ └── k8s/ └── deployment.yaml


## ⚙️ Setup Instructions

1. **Initialize Terraform**

```bash
cd terraform
terraform init
terraform apply

aws eks --region <region> update-kubeconfig --name <cluster_name>

helm install my-app ./helm/chart
kubectl apply -f k8s/deployment.yaml

