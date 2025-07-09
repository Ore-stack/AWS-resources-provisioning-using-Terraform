# Terraform AWS Infrastructure Projects

## Overview
This repository contains production-ready Terraform configurations for provisioning various AWS resources across different use cases. Each project simulates real-world infrastructure challenges with complete business context and implementation requirements.

## Project Categories

### 🗄️ Storage Solutions
1. **PixelStream Inc - Secure S3 Storage**
   - Versioned S3 bucket with SSE-S3 encryption
   - Account-restricted bucket policy
   - Region: eu-central-1

### 🌐 Networking
2. **BrightEdge Tech - VPC Setup**
   - VPC with public subnets across 2 AZs
   - Internet gateway and route tables
   - Resource naming: `brightedge-dev-*`

3. **Innovative Coders - Route 53 DNS**
   - Hosted zone for `innovativecoders.io`
   - A records for root/staging domains
   - CNAME for www subdomain

### 🖥️ Compute & Scaling
4. **EcoDelivery - Auto Scaling Group**
   - Launch Template (Amazon Linux 2)
   - ASG (2-4 instances) with ALB
   - Multi-AZ deployment

### 📊 Monitoring
5. **ArcticView - CloudWatch Alarms**
   - CPU/Disk monitoring for EC2
   - SNS alerts (`arcticview-alerts`)
   - Resource prefix: `arcticview-data-*`

### 🔐 Security & IAM
6. **FincomPay - CI/CD IAM Roles**
   - ECS deployment permissions
   - CloudWatch and S3 access
   - Tags: `environment = "cicd"`

7. **SecureVault - KMS & Parameter Store**
   - Encrypted secrets management
   - Automatic key rotation
   - IAM-restricted access

### 🗃️ Databases
8. **GreenFleet AI - RDS PostgreSQL**
   - Multi-AZ with 7-day backups
   - Secrets Manager integration
   - High availability setup

### ☸️ Kubernetes
9. **FinTech Solutions - EKS Cluster**
   - Managed node groups
   - IRSA with OIDC provider
   - ALB Controller via Helm

### 🚀 CI/CD Pipelines
10. **LogisticsX - ECS Fargate CI/CD**
    - ECR → ECS deployment pipeline
    - GitHub webhook integration
    - Automated initial deployment

## Getting Started

### Prerequisites
- Terraform v1.0+
- AWS CLI configured
- Appropriate AWS permissions

### Usage
## 1. Clone the Repository
   ```bash
   git clone https://github.com/Ore-stack/AWS-resources-provisioning-using-Terraform
   ```
## 2. Navigate to desired project directory:
   ```bash
   cd </path/to/project-folder>
   ```
