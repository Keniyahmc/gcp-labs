# ⚡ Lab 06: Cloud Run Functions Qwik Start - CLI

## Overview
Created, deployed, and tested a Cloud Run function using the
command line. The function is triggered by a Pub/Sub topic
and logs a Hello message when a message is published.

## Objectives
- ✅ Create a Cloud Run function using the CLI
- ✅ Deploy the function triggered by a Pub/Sub topic
- ✅ Test by publishing a message to the topic
- ✅ View function logs via CLI

## Key Commands Used

### Setup
gcloud config set run/region [REGION]
mkdir gcf_hello_world && cd $_

### Deploy
gcloud functions deploy nodejs-pubsub-function --gen2
gcloud functions describe nodejs-pubsub-function

### Test
gcloud pubsub topics publish cf-demo --message="Cloud Function Gen2"

### View Logs
gcloud functions logs read nodejs-pubsub-function --region=[REGION]

## What I Learned
- Cloud Run functions can be triggered by Pub/Sub topics not just HTTP
- Functions are written as separate files and deployed via gcloud
- The --gen2 flag uses the second generation execution environment
- Publishing a message to the trigger topic automatically runs the function
- Logs may take up to 10 minutes to appear after function execution

## Challenges & How I Solved Them
- Found vulnerabilities after running npm install to install
  the package.json dependencies. Fixed by running
  npm audit fix --force which automatically updated the
  vulnerable packages to safer versions before deploying.

## Resources
- GCP Cloud Run Functions Docs: https://cloud.google.com/functions/docs
- Lab ID: GSP080
