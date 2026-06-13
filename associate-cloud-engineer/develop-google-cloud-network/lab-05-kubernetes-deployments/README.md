# ☸️ Lab 05: Managing Deployments Using Kubernetes Engine

## Overview
Learned how to manage and scale Kubernetes deployments using
multiple deployment strategies including rolling updates, canary
deployments, and blue-green deployments.

## Objectives
- ✅ Create and scale a Kubernetes deployment
- ✅ Perform rolling updates, pause, resume, and roll back
- ✅ Implement a canary deployment
- ✅ Implement a blue-green deployment

## Deployment Strategies
| Strategy | How It Works |
|----------|-------------|
| Rolling Update | Gradually replaces old pods with new version |
| Canary | Serves new version to a small subset of traffic |
| Blue-Green | Switches all traffic instantly via service selector |

## What I Learned
- Rolling updates gradually replace pods without downtime
- Canary deployments test new versions with a subset of real traffic
- Blue-green deployments switch all traffic instantly
- kubectl rollout undo rolls back to the previous version
- kubectl scale changes the number of pod replicas immediately

## Resources
- GCP GKE Docs: https://cloud.google.com/kubernetes-engine/docs
- Lab ID: GSP053
