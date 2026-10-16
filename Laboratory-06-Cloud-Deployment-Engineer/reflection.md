# Mission 6 Reflection: The Cloud Deployment Engineer

Docker Compose made deployment easier because I could define the Nextcloud application and MariaDB database in one YAML file. Instead of starting and configuring each container separately, I used the `docker-compose up -d` command to deploy both services. This made the deployment process more organized and convenient.

One important thing I learned about YAML is that proper indentation is necessary for the configuration to work correctly. Incorrect spacing can cause errors or prevent services and their settings from being recognized properly. I needed to maintain consistent indentation under the `services`, `database`, and `app` sections to ensure that the configuration was valid.

Environment variables helped configure the connection between Nextcloud and MariaDB by providing the database name, username, and password. The `MYSQL_HOST=database` setting was especially important because it identified the MariaDB service that Nextcloud needed to connect to. Docker Compose allowed the two containers to communicate through their shared network using the service name.

My experience deploying Nextcloud helped me understand how multiple containers work together as one application. I successfully started the Nextcloud and MariaDB containers, checked their status using `docker-compose ps`, and accessed the Nextcloud setup page through port 8080. After capturing the required screenshots, I used `docker-compose down` to stop and remove the deployment resources.

Since Mission 1, my understanding of cloud computing has improved through hands-on activities and practical exercises. This mission helped me understand containerization, multi-tier architecture, environment variables, and application deployment using Docker Compose. I also learned the importance of checking container status, documenting the process, and saving evidence of completed tasks in my GitHub portfolio.
