# AWS Resources Sample

Terraform-based AWS infrastructure for demonstrating **Cloudability integration for HCP Terraform to test cost estimation, cost-allocation tag compliance, and view recommendations**.

## Overview

This project provisions sample AWS resources to test cloud cost management workflows, including:

- **AWS Infrastructure:** VPC, subnet, internet gateway, EC2 instance, and S3 bucket.
- **Tag Compliance:** Demonstrates compliant and noncompliant resource tagging.
- **Cost Estimation:** Includes sample S3 usage data in `usage.json`.

## Prerequisites

- AWS account and configured credentials
- HCP Terraform standard tier and above
- Cloudability standard tier and above

## Quick Start

```bash
git clone https://github.com/vravind1/aws-resources-sample.git
cd aws-resources-sample
terraform init
terraform validate
terraform plan
terraform apply

## Clean up
Remove the resources when testing is complete:

```bash
terraform destroy


## Repository Structure
- main.tf — AWS resource definitions
- variables.tf — Configurable deployment variables
- usage.json — Sample S3 usage data for cost estimation

### Note
This project is intended for testing and demonstration. Review security settings and potential AWS charges before deployment.

### License
Apache License 2.0 — see LICENSE.
