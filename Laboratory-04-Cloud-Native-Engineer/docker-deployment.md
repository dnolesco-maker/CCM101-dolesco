# Docker Deployment

## Container Lifecycle

### 1. List Running Containers

```bash
**`docker ps`**  
> This command lists the Docker containers that are currently running.

**`docker stop nginx-server`**  
> This command stops the running Nginx container named `nginx-server`.

**`docker ps -a`**  
> This command lists all Docker containers, including stopped containers, to verify that `nginx-server` is no longer running.

**`docker rm nginx-server`**  
> This command removes the stopped `nginx-server` container completely.
