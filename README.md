# Nginx Load Balancer

This project sets up a Docker environment comprising an NGINX web server and a PHP application in four replicas using Docker Compose.

## Prerequisites

- Docker
- Docker Compose

## Configuration

The `docker-compose.yml` file includes two services:

1. `webserver`: An NGINX web server configured to listen on port 80. It uses custom configurations located in the `./nginx` folder.
2. `app`: A PHP application executed with Apache, accessible via the NGINX server. This service is configured to start with 4 replicas.

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/Jean-Quenault/nginx-load-balancer/tree/main
   ```

2. Navigate to the project directory:

   ```
   cd nginx-load-balancer/
   ```

## Deployment

Execute the following command to start the services using Docker Compose:

```
docker-compose up -d
```

The application then displays the ID of the requested container (by the load balancer).

## NGINX Configuration

NGINX configurations are stored in the `./nginx` folder. You can modify them as needed to manage how NGINX handles incoming requests and redirects them to the PHP application.
