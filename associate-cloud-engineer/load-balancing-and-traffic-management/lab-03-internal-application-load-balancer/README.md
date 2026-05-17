\# 🔒 Lab 03: Use an Internal Application Load Balancer



\## Overview

Built a two-tier architecture using an Internal ALB. Backend VMs

run a private prime number calculator with no public IP. A public

frontend queries the internal service through the load balancer.



\## Objectives

\- Create a Python backend prime number calculator

\- Deploy backend VMs using a managed instance group

\- Set up an internal Application Load Balancer

\- Test the internal load balancer from inside the VPC

\- Create a public-facing frontend using the internal service



\## Key Commands Used

gcloud compute instance-templates create primecalc --no-address

gcloud compute instance-groups managed create backend --size 3

gcloud compute health-checks create http ilb-health

gcloud compute backend-services create prime-service

gcloud compute forwarding-rules create prime-lb

gcloud compute instances create frontend



\## What I Learned

\- Internal ALBs have no public IP — only reachable inside the VPC

\- Backend VMs with --no-address are more secure

\- Managed instance groups automatically replace failed VMs

\- Two-tier architecture separates public and private services



\## Challenges \& How I Solved Them

\- Forgot to SSH into the test instance before running curl commands.

&#x20; Ran curl from Cloud Shell instead of inside the test VM which

&#x20; caused it to immediately exit since the internal ALB is not

&#x20; reachable from outside the VPC. Fixed by running SSH first then

&#x20; running curl from inside the instance.



\## Resources

\- GCP Internal ALB Docs: https://cloud.google.com/load-balancing/docs/internal

\- Lab ID: GSP041

