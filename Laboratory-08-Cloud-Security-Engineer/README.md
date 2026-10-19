# Mission 8: The Cloud Security Engineer

## Mission Overview

In this mission, I worked as a Cloud Security Engineer to secure an Ubuntu server using the Uncomplicated Firewall (UFW). I deployed an Nginx web application in a Docker container, configured firewall policies, and allowed only the required incoming services for SSH administration and web application access.

## Objectives

- Understand the Principle of Least Privilege and attack surface.
- Identify and manage network access to a Linux server.
- Configure UFW with a default-deny incoming policy.
- Allow SSH and TCP port 8080 through specific firewall rules.
- Document the security configuration and maintain my GitHub cloud computing portfolio.

## Commands Executed

### Docker and Web Application

```bash
docker --version
docker ps -a --filter "name=secure-web-app"
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps --filter "name=secure-web-app"
curl -I http://localhost:8080
```

### Firewall Configuration

```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl http://localhost:8080
```

## Skills Learned

- Deploying a web server using Docker.
- Testing web application responses using curl.
- Configuring UFW firewall rules on Ubuntu.
- Applying the principle of default-deny incoming traffic.
- Managing network ports to reduce the server's attack surface.
- Documenting cloud security procedures using Markdown and GitHub.
