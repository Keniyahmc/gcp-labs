# 🌐 Lab 02: Multiple VPC Networks

## Overview
Created multiple custom VPC networks with firewall rules and
VM instances, then tested connectivity to understand VPC
isolation. Created a VM with multiple network interfaces.

## Objectives
- ✅ Create custom mode VPC networks with firewall rules
- ✅ Create VM instances in different VPC networks
- ✅ Test connectivity across VPC networks using ping
- ✅ Create a VM with multiple network interfaces

## Key Findings
- External IP pings worked across all VPC networks
- Internal IP pings only worked within the same VPC network
- VMs in different VPCs cannot communicate internally without
  VPC peering or VPN

## What I Learned
- VMs in the same VPC can communicate via internal IP regardless
  of zone or region
- VMs in different VPCs cannot communicate via internal IP
- Auto mode networks create subnets in every region automatically
- A VM can have up to 8 NICs connecting to multiple VPC networks

## Resources
- GCP VPC Docs: https://cloud.google.com/vpc/docs
- Lab ID: GSP211
