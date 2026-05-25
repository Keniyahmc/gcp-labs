# 📨 Lab 07: Pub/Sub Qwik Start - Console

## Overview
Set up a Pub/Sub topic and subscription using the Google Cloud
Console. Published a Hello World message and pulled it using
Cloud Shell to confirm delivery.

## Objectives
- ✅ Create a Pub/Sub topic via the console
- ✅ Create a pull subscription to the topic
- ✅ Publish a Hello World message to the topic
- ✅ Pull and view the message using Cloud Shell

## Key Commands Used
gcloud pubsub subscriptions pull --auto-ack MySub

## What I Learned
- A publisher sends messages to a topic and a subscriber
  receives via a subscription
- Pull subscriptions require the subscriber to request
  messages manually
- The --auto-ack flag automatically acknowledges messages
- Pub/Sub is asynchronous, senders and receivers are decoupled

## Resources
- GCP Pub/Sub Docs: https://cloud.google.com/pubsub/docs
- Lab ID: GSP096
