\# ⚖️ Lab 02: Set Up Application Load Balancers



\## Overview

Set up a Layer 7 Application Load Balancer on Google Cloud 

using Compute Engine VMs and managed instance groups. Unlike 

the Network Load Balancer, an ALB understands HTTP/HTTPS and 

can route traffic based on URL, headers, and cookies.



\## Objectives

\- ✅ Configure default region and zone

\- ✅ Create 3 web server VMs with Apache

\- ✅ Create an instance template and managed instance group

\- ✅ Configure an Application Load Balancer

\- ✅ Test traffic distribution to instances



\## Key Commands Used

```bash

gcloud compute instance-templates create lb-backend-template

gcloud compute instance-groups managed create lb-backend-group

gcloud compute firewall-rules create fw-allow-health-check

gcloud compute addresses create lb-ipv4-1 --global

gcloud compute health-checks create http http-basic-check

gcloud compute backend-services create web-backend-service

gcloud compute url-maps create web-map-http

gcloud compute target-http-proxies create http-lb-proxy

gcloud compute forwarding-rules create http-content-rule

```



\## What I Learned

\- A Layer 7 ALB understands HTTP content and routes by URL

\- Managed instance groups allow autoscaling and autohealing

\- Instance templates define configuration for all VMs in a group

\- URL maps route different paths to different backend services

\- ALB has more components than NLB but is far more flexible



\## Resources

\- \[GCP ALB Docs](https://cloud.google.com/load-balancing/docs/application-load-balancer)

\- Lab ID: GSP155

