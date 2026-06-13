# 📦 Lab 03: Interact with Terraform Modules

## Overview
Used a module from the Terraform Registry to provision a VPC
network with three subnets. Then built a custom module to manage
a Cloud Storage bucket configured for static website hosting.

## Objectives
- ✅ Use the terraform-google-modules/network Registry module
- ✅ Configure module input variables with Gemini Code Assist
- ✅ Define module output values
- ✅ Build a custom gcs-static-website-bucket module
- ✅ Upload files to the static website bucket

## Module Structure
- main.tf
- modules/
- modules/gcs-static-website-bucket/website.tf
- modules/gcs-static-website-bucket/variables.tf
- modules/gcs-static-website-bucket/outputs.tf
- modules/gcs-static-website-bucket/README.md
- modules/gcs-static-website-bucket/LICENSE

## What I Learned
- Modules are reusable sets of Terraform configuration files
- The Terraform Registry provides community and official modules
- Module input variables are set as arguments in the module block
- Module outputs are accessed as module.MODULE_NAME.OUTPUT_NAME
- terraform init must be run to install modules before use
- Custom modules follow the same structure as root modules

## Resources
- Terraform Registry: https://registry.terraform.io
- Lab ID: GSP751
