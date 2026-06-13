# 💾 Lab 04: Manage Terraform State

## Overview
Configured local and Cloud Storage backends for Terraform state
management. Refreshed state to detect infrastructure drift.
Imported an existing Docker container into Terraform and managed
it going forward.

## Objectives
- ✅ Create a local backend
- ✅ Migrate to a Cloud Storage backend
- ✅ Refresh state to detect infrastructure drift
- ✅ Import an existing Docker container into Terraform
- ✅ Manage the imported container with Terraform

## What I Learned
- Terraform state maps real-world resources to configuration blocks
- Remote backends like GCS enable team collaboration with locking
- terraform refresh detects drift between state and real infrastructure
- terraform import brings existing resources under Terraform management
- After import you must manually write the configuration to match
- terraform show -no-color generates a starting config from state

## Resources
- Terraform State Docs: https://developer.hashicorp.com/terraform/language/state
- Lab ID: GSP752
