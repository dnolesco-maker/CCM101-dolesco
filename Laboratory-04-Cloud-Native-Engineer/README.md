# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory focuses on understanding the difference between traditional Virtual Machines and containers. Using the KillerCoda Docker environment, I practiced basic Docker commands and deployed an Nginx web server in a container. I also learned how to manage the container lifecycle and document the procedures using Markdown.

## Objectives

- Differentiate between Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate a containerized Nginx application.
- Create technical documentation using Markdown.
- Continue developing an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3

```bash
docker --version
docker info

### Checkpoint 4
```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080

### Checkpoint 5

```bash
docker ps
docker stop nginx-server
docker ps -a
docker rm nginx-server

## Skills Learned

- Comparing Virtual Machines and Containers.
- Using the Docker CLI in a Linux environment.
- Pulling Docker images from Docker Hub.
- Running a container in detached mode.
- Mapping host and container ports.
- Testing a containerized web server using curl.
- Managing the Docker container lifecycle.
- Creating technical documentation using Markdown.
- Organizing and maintaining a GitHub Cloud Computing Portfolio.

## Challenges Encountered

One challenge I encountered was trying to run the Nginx container when the container name `nginx-server` was already in use. I learned that an existing container should be checked with `docker ps -a` before creating another container with the same name. I also learned how to stop and remove the existing container so that the container lifecycle could be completed correctly.
