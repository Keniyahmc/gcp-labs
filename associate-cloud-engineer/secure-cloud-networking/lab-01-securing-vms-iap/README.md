# 🔐 Lab 01: Securing VMs using Chrome Enterprise Premium

## Overview
Used Identity-Aware Proxy (IAP) TCP forwarding to enable
secure administrative access to VM instances with no external
IP addresses using Chrome Enterprise Premium (BeyondCorp).

## Objectives
- ✅ Enable IAP TCP forwarding
- ✅ Create Linux and Windows VMs with no external IPs
- ✅ Configure firewall rules for IAP access
- ✅ Grant IAP tunnel permissions via IAM
- ✅ Use IAP Desktop to connect to instances
- ✅ Demonstrate SSH and RDP tunneling via IAP

## What I Learned
- VMs without external IPs cannot be accessed directly
- IAP tunnels allow SSH and RDP without exposing VMs publicly
- IAP source IP range 35.235.240.0/20 must be allowed in firewall
- BeyondCorp zero trust model verifies identity before access

## Resources
- GCP IAP Docs: https://cloud.google.com/iap/docs
- Lab ID: GSP1036
