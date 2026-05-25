# 🐍 Lab 09: Pub/Sub Qwik Start - Python

## Overview
Used the Python client library to create Pub/Sub topics and
subscriptions, published messages using gcloud commands, and
received messages using a Python subscriber script.

## Objectives
- ✅ Set up a Python virtual environment
- ✅ Install the Google Cloud Pub/Sub Python client library
- ✅ Create a topic and subscription using Python scripts
- ✅ Publish messages to the topic using gcloud
- ✅ Pull and view messages using the Python subscriber script

## Key Commands Used

### Setup
sudo apt-get install -y virtualenv
python3 -m venv venv
source venv/bin/activate
pip install --upgrade google-cloud-pubsub
git clone https://github.com/googleapis/python-pubsub.git

### Topic and Subscription
python publisher.py $GOOGLE_CLOUD_PROJECT create MyTopic
python subscriber.py $GOOGLE_CLOUD_PROJECT create MyTopic MySub

### Publish and Receive
gcloud pubsub topics publish MyTopic --message "Hello"
python subscriber.py $GOOGLE_CLOUD_PROJECT receive MySub

## What I Learned
- The Python client library simplifies Pub/Sub operations
- publisher.py and subscriber.py handle topic and subscription management
- Messages can be published via gcloud and received via Python
- The receive command listens continuously until stopped with Ctrl+C
- GOOGLE_CLOUD_PROJECT stores the project ID automatically

## Resources
- GCP Pub/Sub Python Docs: https://cloud.google.com/pubsub/docs
- Lab ID: GSP094
