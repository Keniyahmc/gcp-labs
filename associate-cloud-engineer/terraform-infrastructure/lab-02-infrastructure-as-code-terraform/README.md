# 🔧 Lab 02: Infrastructure as Code with Terraform

## Overview
Built, changed, and destroyed infrastructure with Terraform.
Created resource dependencies using implicit and explicit methods
and provisioned infrastructure using local-exec provisioners.

## Objectives
- ✅ Build a VPC network and VM instance with Terraform
- ✅ Make in-place and destructive changes to infrastructure
- ✅ Create implicit and explicit resource dependencies
- ✅ Assign a static IP and connect it to a VM
- ✅ Use local-exec provisioner to write instance data to a file

## Key Concepts
- ~ prefix means in-place update
- -/+ prefix means destroy and recreate
- Implicit dependencies via interpolation expressions
- Explicit dependencies via depends_on argument
- Provisioners run commands after resource creation

## What I Learned
- Terraform tracks changes and only modifies what needs to change
- Changing a boot disk image requires destroying and recreating the VM
- Implicit dependencies are created when one resource references another
- depends_on is used when the dependency is not visible to Terraform
- terraform taint forces a resource to be recreated on next apply

## Resources
- Terraform Docs: https://developer.hashicorp.com/terraform/docs
- Lab ID: GSP750
