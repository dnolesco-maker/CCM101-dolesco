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
