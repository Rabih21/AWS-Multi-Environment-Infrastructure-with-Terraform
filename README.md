# AWS Multi-Environment Infrastructure with Terraform

## Project Overview

This project demonstrates the deployment of reusable AWS infrastructure using Terraform, implementing separate Development and Production environments.

The infrastructure includes VPC networking, public and private subnets, Internet Gateway, NAT Gateways, route tables, Security Groups, EC2 instances, and Nginx web servers.

Terraform remote state is managed through Amazon S3 with state locking.

## Objectives

- Implement Infrastructure as Code using Terraform.
- Configure an S3 remote backend for Terraform state.
- Understand state locking and state isolation.
- Build reusable Terraform modules.
- Deploy separate Development and Production environments.
- Implement secure AWS networking.
- Deploy EC2 instances running Nginx.
- Document infrastructure deployment and cleanup.

## Technologies

- Amazon Web Services (AWS)
- Terraform
- Amazon VPC
- Amazon EC2
- Amazon S3
- AWS IAM
- Nginx
- Git and GitHub
- Visual Studio Code
- AWS CLI

## Environments

| Environment | Purpose |
|---|---|
| Development | Testing and infrastructure experimentation |
| Production | Production-style infrastructure deployment |

## Project Status

In Progress

## Architecture

Architecture diagram and deployment documentation will be added as the project develops.

## Security Considerations

- S3 public access blocked.
- Terraform state encryption enabled.
- Separate state keys for each environment.
- Least-privilege security group rules.
- Secure EC2 administration using AWS Systems Manager where supported.
- No AWS credentials or Terraform state files committed to GitHub.

## Cleanup

All billable AWS resources will be destroyed after project validation and documentation. The remote state bucket will be retained until the project is fully decommissioned.