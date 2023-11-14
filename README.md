# Dockerized Varnish and Nginx

This project sets up a Dockerized environment with Varnish as a caching HTTP reverse proxy and Nginx as a web server. Nginx is configured to return different HTTP response codes on different paths. You can then test the behavior of Varnish when it receives different HTTP response codes from the backend.

### Prerequisites

- Docker
- Docker Compose

## Usage

Once the services are up and running, you can access the following paths to get different HTTP response codes:

- `/502`: Returns a 502 Bad Gateway response.
- `/301`: Returns a 301 Moved Permanently response and redirects to a specified URL.
- ... add more in `nginx.conf`
