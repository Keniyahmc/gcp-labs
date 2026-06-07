# ⚖️ Lab 05: Enhance Application Reliability with Internal Load Balancing

## Overview
Set up an Internal Load Balancer using two managed instance
groups in the same region but different zones. The ILB
distributes traffic across private backends without exposing
them to the public internet.

## Objectives
- ✅ Configure HTTP and health check firewall rules
- ✅ Create instance templates for consistent VM deployments
- ✅ Deploy managed instance groups in two zones
- ✅ Configure an Internal Load Balancer with a static private IP
- ✅ Test traffic distribution using curl from a utility VM

## What I Learned
- Internal Load Balancers use private IPs only
- Deploying instance groups in different zones provides redundancy
- Health checks ensure traffic only goes to healthy instances
- A utility VM inside the same network is needed to test ILB
- ILB is regional, not global like external ALBs

## Resources
- GCP Internal LB Docs: https://cloud.google.com/load-balancing/docs/internal
- Lab ID: GSP216
