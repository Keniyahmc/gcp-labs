# Lab: Network Load Balancer (NLB)

## Overview
Set up a passthrough Network Load Balancer on GCP using 3 Compute Engine VMs running Apache.

## Objectives
- Set default region and zone
- Create 3 web server VMs with Apache
- Configure a load balancing service
- Create a target pool and forwarding rule
- Send traffic and verify distribution

## Key Commands Used
- gcloud compute instances create
- gcloud compute firewall-rules create
- gcloud compute addresses create
- gcloud compute target-pools create
- gcloud compute forwarding-rules create

## What I Learned
- How a Layer 4 NLB routes traffic based on IP/port (not content)
- How target pools group backend instances
- How forwarding rules direct traffic to a target pool
- How health checks keep the load balancer reliable

## Resources
- GCP NLB Docs: https://cloud.google.com/load-balancing/docs/network