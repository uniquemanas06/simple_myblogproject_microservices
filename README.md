# Microservices Blog Application

Welcome to the Microservices Blog Application! This repository contains a set of microservices that collectively form a blog platform. Each microservice focuses on a specific aspect of the application.

## Microservices Overview

### 1. Post Microservice
- Manages blog posts.
- RESTful API for creating, updating, and retrieving posts.
- Utilizes H2 database for simplicity.

### 2. Comment Microservice
- Handles comments on blog posts.
- Allows users to add, edit, and retrieve comments.
- Stores data in MongoDB.

### 3. API Gateway
- Serves as the entry point to the microservices architecture.
- Routes requests to the appropriate microservice.
- Implements circuit breaker pattern using Hystrix.

### 4. Eureka Server (Service Registry)
- Manages service registration and discovery.
- Allows microservices to find and communicate with each other dynamically.

## Features

- **Circuit Breaker (Resiliance4j):**
  - Implemented on critical microservices to prevent cascading failures.
  - Provides fault tolerance and isolation of services.

- **Aspect-Oriented Programming (AOP):**
  - Used for logging, monitoring, and error handling aspects.
  - Enhances modularity and maintainability.

## Configuration

- **YAML Files:**
  - Each microservice includes a `application.yml` file for configuration.
  - Modify these files to suit your environment and requirements.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/microservices-blog.git
