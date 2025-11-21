# aws-three-tier-web-app
A production-ready, highly available three-tier web application built on AWS.

# AWS Three-Tier Web Application

## 📖 The Project Story

This repository documents my journey of building a production-ready, highly available three-tier web application on AWS. This is **Project #2** from the guide ["5 AWS Projects To Get You Hired"](https://learn.thecloudengineers.com/5-aws-projects-to-get-you-hired) by Lefteris Karageorgiou.

The goal is to demonstrate hands-on skills with core AWS services, networking, and architectural best practices that are essential for a cloud role.

---

## 🏗️ Architecture

*(We will add the architecture diagram here later. You can create one using tools like draw.io or Lucidchart and upload it to the repo.)*

The application consists of three distinct layers:
- **Presentation Tier:** Public-facing Application Load Balancer (ALB) and web servers.
- **Application Tier:** EC2 instances in private subnets, managed by an Auto Scaling Group (ASG).
- **Data Tier:** Amazon RDS (PostgreSQL/MySQL) instance in a private subnet for data persistence.

The entire infrastructure is deployed within a custom VPC across multiple Availability Zones for high availability.

---

## 🚀 Implementation Progress

This is my live progress tracker. I am building this step-by-step.

| Phase | Status | Date Completed | Notes & Learnings |
| :--- | :---: | :---: | :--- |
| **Phase 0: Project Setup** | ✅ | `{{21/11/2025}}` | Set up GitHub repository and project documentation. Ready to start building in AWS! |
| **Phase 1: Network Foundation** | ✅ | `{{21/11/2025}}` | Successfully created VPC with CIDR 10.0.0.0/16, spanning 2 AZs with 2 public and 4 private subnets. All route tables, Internet Gateway, and NAT Gateway configured automatically. |
| **Phase 2: Security Configuration** | ❌ | | |
| **Phase 3: Data Tier Setup** | ❌ | | |
| **Phase 4: Application Tier Setup** | ❌ | | |
| **Phase 5: Presentation Tier Setup** | ❌ | | |
| **Phase 6: Automation & Scaling** | ❌ | | |
| **Phase 7: Final Validation & Cleanup** | ❌ | | |

---

## 🛠️ Technologies & AWS Services Used

- **Compute:** Amazon EC2, Auto Scaling
- **Networking:** Amazon VPC, Elastic Load Balancing (ALB), Internet Gateway, NAT Gateway
- **Database:** Amazon RDS (PostgreSQL/MySQL)
- **Security:** Security Groups, IAM Roles
- **Other:** AWS CloudWatch (for monitoring)

---

## 📂 Repository Structure
├── README.md # You are here! The project story and guide.
├── diagrams/ # Architecture diagrams
├── infrastructure/ # (Future) IaC code (Terraform/CDK/CloudFormation)
└── application-code/ # (Future) Sample application code for the EC2 instances


---

## 🎯 Next Steps

My immediate next task is to build the **Network Foundation (Phase 1)** in the AWS Console.

1.  Create a VPC with a defined CIDR block.
2.  Create public and private subnets across two Availability Zones.
3.  Set up an Internet Gateway and Route Tables.

Let's build!
