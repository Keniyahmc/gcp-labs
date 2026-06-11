# 🔑 Lab 06: Getting Started with Cloud KMS

## Overview
Set up a secure Cloud Storage bucket, created a KeyRing and
CryptoKey in Cloud KMS, encrypted financial data using the
KMS API, and configured IAM permissions for key management.

## Objectives
- ✅ Create a Cloud Storage bucket
- ✅ Enable Cloud KMS and create a KeyRing and CryptoKey
- ✅ Encrypt data using the KMS encrypt API endpoint
- ✅ Upload encrypted files to Cloud Storage
- ✅ View Cloud Audit logs for KMS activity

## What I Learned
- Cloud KMS manages encryption keys without exposing them
- KeyRings group related CryptoKeys by environment or purpose
- Data is base64 encoded before being sent to the KMS API
- CryptoKeys and KeyRings cannot be deleted in Cloud KMS

## Resources
- GCP Cloud KMS Docs: https://cloud.google.com/kms/docs
- Lab ID: GSP079
