# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This laboratory demonstrates how to deploy a multi-container application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as its database.

## Objectives

- Understand the concept of a two-tier architecture.
- Configure Nextcloud and MariaDB using a `docker-compose.yml` file.
- Deploy and verify multiple containers using Docker Compose.
- Access the Nextcloud setup page through a web browser.
- Document the deployment process and reflect on the skills learned.

## Commands Executed

| Command | Purpose |
|---|---|
| `docker --version` | Check the installed Docker version. |
| `docker-compose --version` | Check the installed Docker Compose version. |
| `mkdir nextcloud-deployment` | Create the project directory. |
| `cd nextcloud-deployment` | Enter the project directory. |
| `docker-compose config` | Validate the Compose configuration. |
| `docker-compose up -d` | Create and start the services in the background. |
| `docker-compose ps` | Check the status of the containers. |
| `docker-compose down` | Stop and remove the containers and the Compose network. |

## Skills Learned

- Creating a Docker Compose configuration file.
- Deploying a web application and database as separate services.
- Configuring environment variables for database connectivity.
- Checking container status and accessing a web application through a mapped port.
- Documenting deployment evidence and managing project files using GitHub.

## Evidence

Screenshots for the deployment, Nextcloud setup page, and container teardown are stored in the `screenshots/` directory.

## Related Documentation

- [Multi-Tier Architecture](multi-tier-architecture.md)
- [Docker Compose Guide](docker-compose-guide.md)
- [Reflection](reflection.md)
