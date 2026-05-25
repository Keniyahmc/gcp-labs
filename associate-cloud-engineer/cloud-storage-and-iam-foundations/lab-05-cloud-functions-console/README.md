# ⚡ Lab 05: Cloud Run Functions Qwik Start - Console

## Overview
Created, deployed, and tested a Cloud Run function using the
Google Cloud Console. Cloud Run functions are serverless and
event-driven — they only run when triggered making them
cost-efficient for tasks that don't need to run continuously.

## Objectives
- ✅ Create a Cloud Run function via the console
- ✅ Deploy the function
- ✅ Test the function with a Hello World triggering event
- ✅ View function logs

## What I Learned
- Cloud Run functions are serverless and event-driven
- Functions only run when triggered — no cost when idle
- HTTPS is one trigger type — others include Pub/Sub and Storage
- The inline editor lets you write and deploy code in the console
- Logs are available in the Observability tab of the service page
- Second generation execution environment offers better performance

## Challenges & How I Solved Them
- Accidentally selected Deploy a container instead of Write a
  function on the Create function page. This opened a different
  setup flow that did not match the lab instructions. Had to
  restart the entire lab to get a fresh environment and start over.
- Key lesson: Always read the options carefully before clicking.
  Write a function and Deploy a container are two different paths
  and choosing the wrong one requires restarting the lab.

## Resources
- GCP Cloud Run Functions Docs: https://cloud.google.com/functions/docs
- Lab ID: GSP081
