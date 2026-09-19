# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory introduced the role of a Cloud-Native Engineer through hands-on experience with Docker containers. The activities focused on understanding the differences between Virtual Machines and Containers, launching a Docker Playground environment, deploying an Nginx web server container, and managing the container lifecycle. Through these tasks, I learned how containers provide a lightweight and efficient way to package, deploy, and manage applications.

## Objectives

- Understand the differences between Virtual Machines and Containers.
- Verify that Docker is installed and operational.
- Deploy and manage a Docker container.
- Access a web application running inside a container.
- Learn the basic Docker container lifecycle.
- Practice documenting cloud-native activities using GitHub.

## Docker Commands Executed

### Checkpoint 3 - Verify Docker Installation

```bash
docker version
docker info
```

### Checkpoint 4 - Deploy an Nginx Web Server

```bash
docker run -d --name my-nginx -p 8080:80 nginx
docker ps
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx
```

## Skills Learned

- Understanding the differences between Virtual Machines and Containers.
- Using Docker to deploy containerized applications.
- Running and managing Docker containers.
- Accessing services through port mapping.
- Monitoring container status using Docker commands.
- Stopping and removing containers safely.
- Creating technical documentation using Markdown.
- Organizing laboratory activities in a GitHub repository.

## Challenges Encountered

One challenge I encountered was understanding how Docker containers differ from Virtual Machines and how they share the host operating system. I also experienced issues when attempting to stop and remove a container that had not been created yet, which resulted in an error message. Through troubleshooting, I learned the importance of verifying that a container is running before performing lifecycle management commands. This experience improved my understanding of Docker workflows and container management.
