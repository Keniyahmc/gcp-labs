# 🔒 Lab 03: VPC Networks - Controlling Access

## Overview
Created two nginx web servers and controlled external HTTP
access using tagged firewall rules. Explored IAM Network Admin
and Security Admin roles using a service account.

## Objectives
- ✅ Create nginx web servers with and without network tags
- ✅ Create a tagged firewall rule to control HTTP access
- ✅ Create a service account with Network Admin role
- ✅ Compare Network Admin vs Security Admin permissions

## Key Findings
- Blue server (web-server tag): accessible via external IP
- Green server (no tag): external IP blocked, internal only
- Network Admin: can list but not delete firewall rules
- Security Admin: can list and delete firewall rules

## What I Learned
- Network tags allow firewall rules to target specific VMs
- Tagged rules are more secure than rules applying to all VMs
- Network Admin cannot modify firewall rules
- Security Admin can create, modify, and delete firewall rules
- Principle of least privilege means only granting what is needed

## Resources
- GCP VPC Firewall Docs: https://cloud.google.com/vpc/docs/firewalls
- Lab ID: GSP213
