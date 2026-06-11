# ☸️ Lab 07: Setting up a Private Kubernetes Cluster

## Overview
Created private Kubernetes Engine clusters where nodes have
no public IP addresses. Configured master authorized networks
and deployed both auto and custom subnetwork private clusters.

## Objectives
- ✅ Create a private Kubernetes cluster
- ✅ View subnet and secondary address ranges
- ✅ Enable master authorized networks
- ✅ Create a private cluster with a custom subnetwork

## What I Learned
- Private clusters isolate workloads by removing public IPs
- Master authorized networks restrict kubectl access
- IP aliases allow separate pod and service IP ranges
- privateIPGoogleAccess allows nodes to reach Google APIs

## Resources
- GCP Private Clusters Docs: https://cloud.google.com/kubernetes-engine/docs/how-to/private-clusters
- Lab ID: GSP178
