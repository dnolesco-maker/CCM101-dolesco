# Mission 7: The Cloud Operations Engineer

## Mission Overview

This laboratory focuses on the responsibilities of a Cloud Operations Engineer in monitoring system resources, managing containers, and troubleshooting application issues. Using the KillerCoda Ubuntu Playground and Docker, I deployed an Nginx container and monitored its application logs and resource usage.

## Objectives

- Check the host system's memory, disk space, and running processes.
- Deploy an Nginx container named `client-website`.
- Test HTTP requests and identify successful and failed responses.
- Inspect container logs to investigate HTTP errors.
- Monitor container CPU, memory, network, and block I/O metrics.
- Document the results and reflect on the importance of cloud operations and monitoring.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check system memory usage. |
| `df -h /` | Check root filesystem storage usage. |
| `top` | Observe running processes and CPU activity. |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx container in the background and map port 8080 to port 80. |
| `docker ps` | Check running containers and port mappings. |
| `curl http://localhost:8080` | Test the Nginx website. |
| `curl http://localhost:8080/hidden-admin-page` | Test a nonexistent page and observe the HTTP 404 response. |
| `docker logs client-website` | Inspect application logs and investigate failed requests. |
| `docker stats` | Monitor live container resource usage. |

## Skills Learned

- Linux system resource monitoring.
- Docker container deployment and management.
- HTTP request testing using `curl`.
- Application log analysis and error troubleshooting.
- Container resource monitoring using Docker.
- Technical documentation and evidence collection.

## Evidence and Documentation

Screenshots and supporting documentation for this mission are stored in this folder.

- `system-baseline-report.md`: Host system resource measurements.
- `container-observability.md`: Application logs and container resource metrics.
- `reflection.md`: Reflection on the laboratory activities.
- `screenshots/`: Screenshots collected as evidence for the completed checkpoints.
