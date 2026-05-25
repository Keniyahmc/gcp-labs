# 📊 Lab 04: Cloud Monitoring Qwik Start

## Overview
Set up Cloud Monitoring for a Compute Engine VM running Apache.
Installed monitoring and logging agents, created uptime checks,
configured alerting policies, and built a custom dashboard.

## Objectives
- ✅ Create a Compute Engine VM with Apache installed
- ✅ Install Cloud Monitoring and Logging agents
- ✅ Create an uptime check for the VM
- ✅ Create an alerting policy for network traffic
- ✅ Build a custom dashboard with charts
- ✅ View logs in Cloud Logging

## What I Learned
- Cloud Ops Agent must be installed on VMs to send monitoring data
- Uptime checks verify a resource is accessible from multiple regions
- Alerting policies can notify via email, Slack, PagerDuty and more
- Cloud Logging and Cloud Monitoring are tightly integrated
- Stopping and starting a VM generates log entries in real time

## Challenges & How I Solved Them
- Forgot to open SSH terminal for lamp-1-vm and tried to install
  Apache from Cloud Shell instead. Cloud Shell is not connected
  to the VM so the install had no effect. Fixed by clicking the
  SSH button next to lamp-1-vm in Compute Engine console and
  running the install commands from inside that session.
- Key lesson: Cloud Shell and SSH are different. Always use SSH
  when running commands on a Compute Engine instance.

## Resources
- GCP Cloud Monitoring Docs: https://cloud.google.com/monitoring/docs
- Lab ID: GSP089
