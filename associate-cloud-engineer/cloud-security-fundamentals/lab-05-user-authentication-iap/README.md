# 🔑 Lab 05: User Authentication - Identity-Aware Proxy

## Overview
Built a Python web app on App Engine and used IAP to restrict
access, retrieve user identity from headers, and
cryptographically verify identity to prevent spoofing.

## Objectives
- ✅ Deploy a Python App Engine web application
- ✅ Restrict access using IAP
- ✅ Retrieve user identity from IAP request headers
- ✅ Cryptographically verify IAP identity

## What I Learned
- IAP intercepts requests and authenticates users before the app
- IAP adds X-Goog-Authenticated-User headers to every request
- Without IAP these headers can be spoofed by anyone
- JWT cryptographic verification prevents identity spoofing

## Resources
- GCP IAP Docs: https://cloud.google.com/iap/docs
- Lab ID: GSP499
