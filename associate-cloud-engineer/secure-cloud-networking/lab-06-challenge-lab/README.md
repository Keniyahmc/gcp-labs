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
- Overly permissive firewall rules: The default open-access rule
  was allowing unrestricted traffic. Removed it and replaced with
  specific rules scoped to correct source ranges and target tags.

- IAP SSH connection failing with Error 4003: The browser SSH
  button was trying to connect directly instead of through IAP.
  Fixed by using the Open in browser window with IAP tunnel
  option from the SSH dropdown menu on the bastion VM.

- Network tags not applied: Firewall rules were correctly
  configured but not taking effect because the network tags
  were not saved on the VMs. Fixed by editing each VM and
  ensuring the tags were properly committed.

- SSHing from bastion to juice-shop: A plain ssh internal-ip
  command was not reliable from inside the bastion. Fixed by
  using gcloud compute ssh juice-shop --zone=us-west1-c
  --internal-ip to force the connection through the internal
  network correctly.

## Resources
- GCP IAP Docs: https://cloud.google.com/iap/docs
- Lab ID: GSP322
