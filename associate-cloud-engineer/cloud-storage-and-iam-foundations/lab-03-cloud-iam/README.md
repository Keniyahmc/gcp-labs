# 🔐 Lab 03: Cloud IAM Qwik Start

## Overview
Explored Cloud IAM by signing in as two different users with
different roles. Experienced how granting and revoking permissions
affects what each user can see and do in the GCP Console.

## Objectives
- ✅ Explore IAM console and project level roles
- ✅ Create a bucket and upload a file as Owner
- ✅ Verify Viewer access as Username 2
- ✅ Remove project access from Username 2
- ✅ Grant Storage Object Viewer role to Username 2

## What I Learned
- IAM roles control what users can and cannot do across GCP
- Project-level roles like Viewer apply to all services
- Resource-level roles apply to specific resources only
- Revoking a role can take up to 80 seconds to propagate
- Users with no project role can still access specific resources

## Resources
- GCP IAM Docs: https://cloud.google.com/iam/docs
- Lab ID: GSP064
