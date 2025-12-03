# Chat-shared-services.

Shared infrastructure layer for the distributed chat platform

A collection of essential infrastructure services used across the entire distributed chat system — message broker, caching layer, reverse proxy, and shared configurations packaged into a single, easy-to-run environment.

## 🚀 Overview

Chat-shared-services provides the common infrastructure foundation required by every backend microservice in the platform.
Instead of duplicating configs across repositories, this project centralizes the critical shared components:

**RabbitMQ** — message broker for events and real-time communication

**Redis** — caching, ephemeral state, presence tracking

**Nginx** — reverse proxy, routing, and static entrypoint for local development

These services form the backbone of the system, enabling reliable communication between Chat-auth, Chat-transport, Chat-messaging, and other components.

The repository is optimized for local development, making it effortless to spin up the entire stack with a single command.

## 🧩 Features

- RabbitMQ with full configuration

Exchanges, queues, bindings

Management UI enabled

Ready for real-time messaging workloads

- Redis

Used for caching, deduplication, presence, and ephemeral data

Minimal configuration for maximum speed

- Nginx reverse proxy

Central entrypoint for routing HTTP/WebSocket traffic

Clean proxying setup for development

Ideal for working with multiple services behind a single hostname

Unified infrastructure environment
All shared dependencies defined in one docker-compose file.

Consistent development experience
Each microservice relies on the same standardized RabbitMQ, Redis, and Nginx configs.

## ⚙️ Usage.

1) Clone the repository.
2) Create .env file in the backed directory using the env_example.txt as an example.
3) ```docker-compose up --build``` in the directory where docker-compose.yaml file is located.

## Recent updates.

None yet released.

## 🔗 Back to the Main Index Repository

Explore the full distributed chat system:
https://github.com/aleksandrshaulskyi/chat-index
