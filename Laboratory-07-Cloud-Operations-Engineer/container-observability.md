# Container Observability

## Application Logs

The application logs were retrieved using the following command:

```bash
docker logs client-website
```

The logs show successful HTTP requests with status code 200 and failed requests with status code 404.

## HTTP 404 Error Log

```text
172.17.0.1 - - [16/Oct/2026:03:18:02 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

## Importance of Application Logs

Application logs are vital for troubleshooting because they record incoming requests, HTTP status codes, and errors that help identify problems. They allow a Cloud Operations Engineer to investigate failed requests, understand what went wrong, and determine the appropriate corrective action.

The docker stats command was used to monitor the live resource usage of the client-website container.

Container Name: client-website
CPU Usage: 0.00%
Memory Usage: 2.73 MiB
Memory Limit: 1.859 GiB
Memory Usage Percentage: 0.14%
Network I/O: 6.21 kB received / 10.5 kB transmitted
Block I/O: 0 B read / 12.3 kB written
Running Processes (PIDS): 2

These metrics help determine whether a container is consuming excessive system resources. Monitoring CPU, memory, and network activity helps a Cloud Operations Engineer detect unusual behavior and investigate potential performance problems.
