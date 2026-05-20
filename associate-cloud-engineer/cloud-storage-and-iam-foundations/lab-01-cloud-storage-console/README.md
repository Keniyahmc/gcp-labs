# 🪣 Lab 01: Cloud Storage Qwik Start - Console

## Overview
Used the Google Cloud Console to create a Cloud Storage bucket,
upload objects, organize files with folders, and make objects
publicly accessible.

## Objectives
- ✅ Create a Cloud Storage bucket
- ✅ Upload an object to the bucket
- ✅ Share a bucket object publicly
- ✅ Create folders and subfolders
- ✅ Delete a folder

## What I Learned
- Bucket names must be globally unique across all of Cloud Storage
- Object names only need to be unique within their own bucket
- Granting allUsers the Storage Object Viewer role makes objects public
- Uniform access control manages permissions at bucket level via IAM
- Public objects get a shareable URL at storage.googleapis.com

## Challenges & How I Solved Them
- Missed unchecking Enforce public access prevention during bucket
  creation. This blocked making objects public in Task 3. Fixed by
  going back into Permissions and turning it off before granting
  access to allUsers.
- Had trouble setting permissions to allUsers because public access
  prevention was still enabled. Once turned off the allUsers principal
  was added successfully with the Storage Object Viewer role.

## Resources
- GCP Cloud Storage Docs: https://cloud.google.com/storage/docs
- Lab ID: GSP073
