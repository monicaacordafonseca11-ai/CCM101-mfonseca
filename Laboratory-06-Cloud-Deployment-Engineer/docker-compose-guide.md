# Docker Compose Technical Guide

## Key Concepts

### What does the services: block do?
The `services:` block defines the individual containers that make up your multi-container application stack[span_9](start_span)[span_9](end_span). Each service under this block represents a distinct container (in this deployment, `database` and `app`) that Docker Compose will build, configure, and network together[span_10](start_span)[span_10](end_span).

### How did the Nextcloud app container know how to find the database container?
The Nextcloud app container locates the database container via Docker’s built-in internal DNS resolution[span_11](start_span)[span_11](end_span). By setting `MYSQL_HOST=database`, we explicitly pointed the application to the service name defined under the `services:` block, allowing them to communicate securely over the Docker network[span_12](start_span)[span_12](end_span).

### What is the difference between docker run and docker-compose up -d?
* **`docker run`**: Used to manually launch a single container at a time with inline command-line flags[span_13](start_span)[span_13](end_span).
* **`docker-compose up -d`**: Reads a declarative multi-container YAML configuration blueprint and deploys an entire architecture stack simultaneously in the background with a single command[span_14](start_span)[span_14](end_span).
* 
