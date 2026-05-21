# 🪣 Lab 02: Cloud Storage Qwik Start - CLI/SDK

## Overview
Performed Cloud Storage tasks entirely through the command line
using gcloud storage commands in Cloud Shell instead of the console.

## Objectives
- ✅ Create a bucket via CLI
- ✅ Upload an object to the bucket
- ✅ Download an object from the bucket
- ✅ Copy an object to a folder
- ✅ List bucket contents and object details
- ✅ Make an object publicly accessible
- ✅ Remove public access from an object

## Key Commands Used
gcloud storage buckets create gs://[BUCKET-NAME]
gcloud storage cp ada.jpg gs://[BUCKET-NAME]
gcloud storage cp -r gs://[BUCKET-NAME]/ada.jpg .
gcloud storage ls gs://[BUCKET-NAME]
gcloud storage ls -l gs://[BUCKET-NAME]/ada.jpg
gcloud storage objects update --add-acl-grant=entity=allUsers,role=READER
gcloud storage objects update --remove-acl-grant=allUsers
gcloud storage rm gs://[BUCKET-NAME]/ada.jpg

## What I Learned
- CLI can do everything the Console can do and more
- gcloud storage cp uploads and downloads objects
- Public access granted via --add-acl-grant=entity=allUsers,role=READER
- Folders in Cloud Storage are virtual paths in object names

## Challenges & How I Solved Them
- Named the bucket with a period in the name which caused the
  creation command to fail. Fixed by renaming using only lowercase
  letters, numbers, and dashes with no periods.
- Key lesson: Stick to lowercase letters, numbers, and dashes
  when naming buckets to avoid naming rule violations.

## Resources
- GCP Cloud Storage CLI Docs: https://cloud.google.com/storage/docs
- Lab ID: GSP074
