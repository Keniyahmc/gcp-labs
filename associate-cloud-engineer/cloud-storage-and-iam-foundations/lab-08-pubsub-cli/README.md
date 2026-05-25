# 📨 Lab 08: Pub/Sub Qwik Start - Command Line

## Overview
Performed all Pub/Sub operations using gcloud commands.
Created and deleted topics and subscriptions, published
multiple messages, and learned how the pull command works
with and without flags.

## Objectives
- ✅ Create, list, and delete Pub/Sub topics
- ✅ Create, list, and delete Pub/Sub subscriptions
- ✅ Publish multiple messages to a topic
- ✅ Pull messages using the pull command
- ✅ Pull all messages at once using the limit flag

## Key Commands Used

### Topics
gcloud pubsub topics create myTopic
gcloud pubsub topics list
gcloud pubsub topics delete Test1

### Subscriptions
gcloud pubsub subscriptions create --topic myTopic mySubscription
gcloud pubsub topics list-subscriptions myTopic
gcloud pubsub subscriptions delete Test1

### Publish and Pull
gcloud pubsub topics publish myTopic --message "Hello"
gcloud pubsub subscriptions pull mySubscription --auto-ack
gcloud pubsub subscriptions pull mySubscription --limit=3

## What I Learned
- Pull without flags returns only one message at a time
- Once a message is pulled it cannot be pulled again
- The --limit flag sets how many messages to pull at once
- The --auto-ack flag automatically acknowledges messages
- Topics and subscriptions can be fully managed via CLI

## Resources
- GCP Pub/Sub Docs: https://cloud.google.com/pubsub/docs
- Lab ID: GSP095
