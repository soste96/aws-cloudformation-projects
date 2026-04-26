# AWS CloudFormation Projects
**Solomon Sterling** | AWS Cloud Engineer | Atlanta, GA

---

## Project 1 — VPC Web Server Stack

### What I Built
Deployed a production-style AWS networking stack entirely through 
Infrastructure as Code using AWS CloudFormation.

### Architecture
- **VPC** with a /16 CIDR block and DNS support enabled
- **Public Subnet** mapped to an Availability Zone
- **Internet Gateway** attached and routed via a custom Route Table
- **Security Group** allowing inbound HTTP (80) and SSH (22)
- **EC2 t2.micro** instance running Amazon Linux 2
- **Elastic IP** for a consistent public endpoint
- **UserData script** that auto-installs and starts Apache on boot

### Key Skills Demonstrated
- Infrastructure as Code (IaC) with CloudFormation YAML
- VPC networking and routing
- EC2 provisioning and bootstrapping
- Cost-zero deployment using AWS Free Tier

### Result
A live web server accessible via public IP, fully provisioned 
from a single template file with zero manual configuration.
