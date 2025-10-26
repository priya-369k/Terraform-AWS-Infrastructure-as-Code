# Terraform-AWS-Infrastructure-as-Code
[![Terraform](https://img.shields.io/badge/Terraform-1.6+-623CE4?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![AWS](https://img.shields.io/badge/AWS-Cloud-FF9900?logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
## 📋 Overview  
Professional Terraform project demonstrating Infrastructure as Code (IaC) best practices for AWS cloud automation. This repository showcases multi-cloud infrastructure provisioning, state management, and enterprise-grade DevOps practices.

### Key Features

- ✅ **Multi-Environment Support**: Dev, Staging, Production configurations
- ✅ **Modular Architecture**: Reusable, composable infrastructure modules
- ✅ **State Management**: Remote state with S3 backend and DynamoDB locking
- ✅ **Security First**: Encrypted state files, security groups, IAM policies
- ✅ **Auto-Scaling**: Dynamic resource provisioning
- ✅ **CI/CD Ready**: GitHub Actions integration for automated deployments
- ✅ **Cost Optimized**: Resource tagging and cost tracking

## 🏗️ Architecture

This project provisions:

- **VPC**: Custom Virtual Private Cloud with public/private subnets
- **EC2 Instances**: Auto-scaled compute resources with monitoring
- **Security Groups**: Properly configured ingress/egress rules
- **Internet Gateway**: Public internet connectivity
- **Monitoring**: CloudWatch integration for observability

## 📂 Project Structure

## 🚀 Getting Started

### Prerequisites

- **Terraform**: Version 1.6.0 or higher
- **AWS CLI**: Configured with appropriate credentials
- **AWS Account**: With sufficient permissions (AdministratorAccess for testing)
- **Git**: For version control

## 📊 Outputs

After successful deployment, Terraform provides:

| Output | Description |
|--------|-------------|
| `instance_ids` | EC2 instance IDs |
| `instance_public_ips` | Public IP addresses for SSH/HTTP access |
| `instance_private_ips` | Private IPs for internal communication |
| `vpc_id` | VPC identifier |
| `subnet_ids` | Subnet identifiers |

## 🔒 Security Best Practices

- ✅ Never commit `.tfvars` files with sensitive data to Git
- ✅ Use IAM roles instead of access keys for production
- ✅ Enable MFA for IAM users with administrative access
- ✅ Encrypt Terraform state files (enabled by default with S3 backend)
- ✅ Use least-privilege IAM policies
- ✅ Regularly rotate AWS access keys
- ✅ Review security group rules for overly permissive access
- ✅ Enable CloudTrail logging for audit trails

## 📈 Cost Optimization

- Use `t2.micro` instances for dev/testing (AWS Free Tier eligible)
- Enable detailed billing and cost allocation tags
- Set up AWS Budget alerts
- Use spot instances for non-critical workloads
- Regularly review and terminate unused resources



