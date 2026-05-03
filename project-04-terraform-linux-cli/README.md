# Project 04 — Terraform + Linux CLI

## What I Built
Provisioned AWS infrastructure using Terraform IaC from 
a local Mac terminal — deployed in under 60 seconds with 
a single command.

## Resources Provisioned
- **EC2 t2.micro** running Apache web server
- **Security Group** allowing HTTP (80) and SSH (22)
- **S3 Bucket** for object storage

## Terraform Workflow Used
1. `terraform init` — downloaded AWS provider
2. `terraform plan` — previewed infrastructure changes
3. `terraform apply` — deployed all resources in 22 seconds
4. `terraform destroy` — tore down everything cleanly

## CLI Commands Used
- `aws ec2 describe-instances` — listed running instances
- `aws s3 ls` — listed S3 buckets
- `aws s3 cp` — uploaded file to S3 from terminal

## Key Concepts Demonstrated
- Infrastructure as Code with Terraform HCL
- AWS provider configuration
- Resource dependency management
- Output variables
- Full infrastructure lifecycle management

## Result
Live web server provisioned entirely via code — 
no manual AWS Console clicks required.
