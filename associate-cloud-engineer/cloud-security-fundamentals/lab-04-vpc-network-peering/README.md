# 🔗 Lab 04: VPC Network Peering

## Overview
Set up VPC Network Peering between two projects to enable
private connectivity across VPC networks without using
external IPs or VPNs.

## Objectives
- ✅ Create custom VPC networks in two projects
- ✅ Configure VPC peering from both sides
- ✅ Test internal IP connectivity between projects

## What I Learned
- Both sides must configure peering before it becomes ACTIVE
- Peered networks share routes automatically once active
- Peering provides lower latency and cost than VPNs
- CIDR ranges of peered networks must not overlap

## Resources
- GCP VPC Peering Docs: https://cloud.google.com/vpc/docs/vpc-peering
- Lab ID: GSP193
