# 🌐 Lab: Network Load Balancer (NLB)

## Overview
Set up a passthrough **Network Load Balancer (NLB)** on Google Cloud Platform using 3 Compute Engine VMs running Apache. A Layer 4 NLB routes traffic based on IP addresses and port numbers.

## Objectives
- ✅ Configure the default region and zone
- ✅ Create 3 web server VMs with Apache installed
- ✅ Configure a load balancing service
- ✅ Create a target pool and forwarding rule
- ✅ Send traffic and verify distribution across instances

## Key Commands Used
```bash
gcloud compute instances create
gcloud compute firewall-rules create
gcloud compute addresses create
gcloud compute http-health-checks create
gcloud compute target-pools create
gcloud compute forwarding-rules create
```

## What I Learned
- A Layer 4 NLB routes traffic based on IP/port — it does not inspect content
- Target pools group backend instances that receive incoming traffic
- Forwarding rules direct traffic from a static IP to a target pool
- Health checks ensure only healthy instances receive traffic

## Resources
- [GCP Network Load Balancer Docs](https://cloud.google.com/load-balancing/docs/network)
