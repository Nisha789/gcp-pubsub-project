# GCP Pub/Sub

## Description
This project demonstrates the use of Google Cloud Pub/Sub, a messaging service for building event-driven systems. The project consists of two main components: a producer that sends messages to a Pub/Sub topic and a consumer that listens for and processes messages from a subscription. This setup enables efficient and scalable communication between different parts of your application.

## Features
- **Producer**: Generates mock order data and publishes it to a specified Pub/Sub topic. It handles message acknowledgments and includes a callback function to manage the publishing results.
- **Consumer**: Pulls messages from a Pub/Sub subscription, deserializes the JSON data, and processes the messages accordingly. The consumer acknowledges messages after processing to prevent them from being received again.

## Getting Started

### Prerequisites
To run this project, you will need:
- Python 3.x installed on your machine.
- The following libraries:
  - `google.cloud.pubsub`: This library allows you to interact with Google Cloud Pub/Sub services.
  - `json`: For handling JSON data.

### Installation
Install the required library using pip. Open your terminal or command prompt and run the following command:

```bash
pip install google-cloud-pubsub