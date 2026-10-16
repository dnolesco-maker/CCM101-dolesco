# Docker Compose Guide

## 1. The Services Block

The `services` block in the `docker-compose.yml` file defines the containers that make up the application. In this deployment, there are two services: `database` and `app`.

- **Database Service:** Uses the `mariadb:10.6` image to store the Nextcloud data. It also defines the database name, username, and passwords through environment variables.
- **App Service:** Uses the `nextcloud` image and maps port `8080` on the host to port `80` inside the container so the Nextcloud web interface can be accessed through a browser.

## 2. How MYSQL_HOST Connects the Containers

The environment variable `MYSQL_HOST=database` tells the Nextcloud application where to find the MariaDB database. The value `database` matches the name of the database service in the Compose file. Docker Compose creates a network for the services and allows them to communicate using their service names.

## 3. Docker Run vs. Docker Compose

The `docker run` command is commonly used to create and start an individual container. When an application requires multiple containers, each container may need its own command and configuration.

The `docker-compose up -d` command reads the `docker-compose.yml` file and starts the services defined in it. The `-d` option runs the containers in the background. This makes it easier to deploy and manage an application with multiple connected services, such as Nextcloud and MariaDB.
