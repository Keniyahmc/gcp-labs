# 🏆 Lab 06: Build a Secure Google Cloud Network - Challenge Lab

## Overview
Applied all skills from Labs 01-05 independently to secure
a real-world website (juice-shop) for a small business owner.
Removed overly permissive firewall rules and implemented a
secure bastion host architecture using IAP.

## Tasks Completed
- ✅ Remove overly permissive firewall rules
- ✅ Start the bastion host instance
- ✅ Create firewall rule for SSH via IAP to bastion
- ✅ Create firewall rule for HTTP to juice-shop
- ✅ Create firewall rule for SSH from bastion to juice-shop
- ✅ SSH to bastion via IAP and connect to juice-shop

## What I Learned
- Overly permissive firewall rules are a major security risk
- Bastion hosts act as a secure jump box for private VMs
- IAP tunnels eliminate the need for a public IP on bastion
- Network tags allow precise targeting of firewall rules
- Zero trust means verifying identity before any network access

## Challenges & How I Solved Them
- [Add your challenges here]

## Resources
- GCP IAP Docs: https://cloud.google.com/iap/docs
- Lab ID: GSP322
