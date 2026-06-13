# 🏗️ Lab 01: Terraform Fundamentals

## Overview
Used Terraform and Gemini Code Assist to provision a VM instance
on Google Cloud. Learned how Terraform uses declarative
configuration files to safely create and manage infrastructure.

## Objectives
- ✅ Verify Terraform installation in Cloud Shell
- ✅ Use Gemini Code Assist to generate a Terraform configuration
- ✅ Initialize, plan, and apply a Terraform configuration
- ✅ Inspect Terraform state with terraform show

## Key Commands
| Command | Purpose |
|---------|---------|
| terraform init | Initialize working directory and download providers |
| terraform plan | Preview changes without applying |
| terraform apply | Create or update infrastructure |
| terraform show | Inspect current state |
| terraform destroy | Destroy all managed infrastructure |

## What I Learned
- Terraform uses declarative .tf files to describe desired state
- terraform init downloads the provider plugin for the configuration
- terraform plan shows what will change without making changes
- terraform.tfstate tracks the mapping between config and resources
- Gemini Code Assist generates Terraform configs from natural language

## Resources
- Terraform Docs: https://developer.hashicorp.com/terraform/docs
- Lab ID: GSP156
