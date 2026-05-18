## Tools Used

| Tool | Version |
|---|---|
| Terraform | v1.15.3 |
| AWS CLI | v2.34.48 |
| AWS Region | ap-southeast-1 |

## How to Deploy

**Prerequisites:** AWS CLI configured, Terraform installed

```bash
# Clone the repo
git clone https://github.com/nidinshah/aws-vpc-terraform.git
cd aws-vpc-terraform

# Deploy
terraform init
terraform plan
terraform apply
```

**To destroy when done:**
```bash
terraform destroy
```

> ⚠️ The NAT Gateway incurs hourly charges. Always run `terraform destroy` after testing.

## Project Report

Full write-up with architecture breakdown, deployment screenshots, and key learnings:
👉 (https://nidinshah.com)

## Key Learnings

- Terraform IaC workflow — init, plan, apply, destroy
- AWS VPC design — CIDR allocation, subnet segmentation
- Internet Gateway vs NAT Gateway — when and why to use each
- Route table configuration for public and private subnets

## Part of my AWS SAA-C03 study journey
