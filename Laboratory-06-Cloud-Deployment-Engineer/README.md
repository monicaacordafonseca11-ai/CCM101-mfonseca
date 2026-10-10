# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview
Transitioning from manual single-container deployments to Infrastructure as Code (IaC) using Docker Compose to deploy a multi-tier private cloud storage application (Nextcloud and MariaDB)[span_23](start_span)[span_23](end_span).

## Objectives
* Explain the concept of a multi-tier application architecture[span_24](start_span)[span_24](end_span).
* Understand the purpose and structure of a `docker-compose.yml` file[span_25](start_span)[span_25](end_span).
* Use a Linux command-line text editor (`nano`) to create configuration files[span_26](start_span)[span_26](end_span).
* Deploy a multi-container application stack using Docker Compose[span_27](start_span)[span_27](end_span).
* Document deployment procedures and IaC principles using Markdown[span_28](start_span)[span_28](end_span).

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

