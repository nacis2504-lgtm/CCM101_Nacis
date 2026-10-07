# Mission 6 - The Cloud Deployment Engineer

## Mission Overview

This mission focused on deploying a multi-tier private cloud storage system using Docker Compose. The system consists of Nextcloud as the Web/Application Tier and MariaDB as the Database Tier. Docker Compose was used to deploy and manage both containers together.

## Objectives

- Understand multi-tier architecture.
- Create a `docker-compose.yml` file.
- Configure Docker services using YAML.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access Nextcloud using port 8080.
- Understand Infrastructure as Code (IaC).
- Document the deployment process.

## Commands Executed

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

## Skills Learned

- Creating Docker Compose files.
- Writing YAML configuration.
- Using Docker Compose.
- Deploying multiple containers.
- Connecting Nextcloud with MariaDB.
- Using environment variables.
- Managing Docker containers.
- Checking container status.
- Understanding multi-tier architecture.
- Applying Infrastructure as Code concepts.
- Using Linux terminal commands.
- Creating technical documentation using Markdown.
