# 🏆 Lab 10: Set Up an App Dev Environment - Challenge Lab

## Overview
Applied all skills from Labs 01-09 independently to set up
an app dev environment for the fictional Memories team. Created
a storage bucket, Pub/Sub topic, Cloud Run Function for image
thumbnails, and removed a previous engineer's access.

## Tasks Completed
- ✅ Create a bucket for storing photographs
- ✅ Create a Pub/Sub topic
- ✅ Create a thumbnail Cloud Run Function
- ✅ Remove the previous cloud engineer's access

## What I Learned
- Cloud Run Functions triggered by Cloud Storage require the
  Cloud Storage service agent to have Pub/Sub publisher role
- gsutil kms serviceaccount gets the correct service account
  email for granting IAM permissions
- Always grant IAM permissions before deploying functions
  that use Cloud Storage triggers
- CLI deployment gives more control than the console for
  complex function configurations

## Challenges & How I Solved Them
- Eventarc service agent did not exist causing trigger creation
  to fail. Fixed by granting Pub/Sub publisher role to the
  Cloud Storage service agent using gsutil kms serviceaccount.
- Cloud Run API was not enabled on first deploy. Fixed by
  typing y when prompted during deployment.
- Wrong trigger type selected in console. Switched to CLI
  deployment for more control over configuration.
- Function showed 0 items after first deploy. Fixed by
  granting correct IAM roles and redeploying.
- Key lesson: Always grant necessary IAM permissions before
  deploying Cloud Run Functions with Cloud Storage triggers.

## Resources
- GCP Cloud Run Functions Docs: https://cloud.google.com/functions/docs
- GCP Cloud Storage Docs: https://cloud.google.com/storage/docs
- GCP Pub/Sub Docs: https://cloud.google.com/pubsub/docs
- Lab ID: GSP315
