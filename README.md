# Couchbase Docker Project

## Introduction

Couchbase is a high-performance, open-source NoSQL database designed for modern application development. It combines the flexibility of JSON document storage with the power of SQL-like querying, full-text search, and real-time analytics. Couchbase is widely used for building scalable, distributed applications.
In this project, Couchbase is containerized using Docker, making it easy to set up, manage, and access a local instance for development or testing purposes.

## Steps to Setup and Run Couchbase

**Step 1: Pull the Couchbase Docker Image**
To begin, the official Couchbase image was pulled from Docker Hub:

    docker pull couchbase

**Step 2: Create and Run a Docker Container**
A container was created from the pulled image, mapping the local machine’s port 8091 to the container’s port 8091:

    docker run -d --name db -p 8091-8097:8091-8097 -p 9123:9123 -p 11207:11207 -p 11210:11210 -p 11280:11280 -p 18091-18097:18091-18097 couchbase

**Step 3: Accessing Couchbase in Browser**
After the container started successfully, Couchbase was accessed in a browser by navigating to:

    http://localhost:8091

## Video

https://github.com/user-attachments/assets/b0b0bcea-6db2-4419-99c6-9efb7838afc8
