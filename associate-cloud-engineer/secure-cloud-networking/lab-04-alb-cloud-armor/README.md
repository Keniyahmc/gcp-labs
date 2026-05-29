# 🛡️ Lab 04: Configure ALB with Google Cloud Armor

## Overview
Configured a Global External Application Load Balancer with
backends in two regions. Stress tested it with siege to trigger
cross-region failover then used Cloud Armor to denylist the
stress test VM IP at the edge.

## Objectives
- ✅ Configure HTTP and health check firewall rules
- ✅ Create instance templates and managed instance groups
- ✅ Configure a Global External Application Load Balancer
- ✅ Stress test the load balancer to trigger regional failover
- ✅ Create a Cloud Armor security policy to denylist an IP
- ✅ Verify traffic is blocked via security logs

## What I Learned
- Global ALBs terminate traffic at Google Edge before the VPC
- Cross-region failover triggers when backend exceeds capacity
- Cloud Armor blocks traffic at Layer 7 before reaching backends
- Denylisting at the edge saves backend resources
- Security policy logs show exactly which requests were denied

## Resources
- GCP Cloud Armor Docs: https://cloud.google.com/armor/docs
- Lab ID: GSP215
