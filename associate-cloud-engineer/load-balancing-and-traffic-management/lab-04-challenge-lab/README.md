\# 🏆 Lab 04: Challenge Lab - Implement Load Balancing on Compute Engine



\## Overview

Applied all load balancing skills from Labs 01-03 independently

in a timed challenge with no step-by-step instructions.



\## Tasks Completed

\- ✅ Create multiple web server instances with firewall rules

\- ✅ Configure the load balancing service

\- ✅ Create an HTTP load balancer



\## What I Learned

\- Challenge labs test real understanding with no guidance

\- NLB and ALB have different resource requirements and use cases

\- Resource naming matters, wrong names cause tasks to fail

\- Time management is critical, 25 minutes goes fast



\## Challenges \& How I Solved Them

\- Created VMs without the startup script initially. Apache was

&#x20; not installed so curl verification failed. Fixed by deleting

&#x20; all 3 VMs and recreating them with the startup script included.

\- Used internal IP instead of external IP when testing curl.

&#x20; Fixed by using the EXTERNAL\_IP column from

&#x20; gcloud compute instances list.



\## Resources

\- GCP Load Balancing Docs: https://cloud.google.com/load-balancing/docs

\- Lab ID: GSP313

