# My App Docker Configuration

This repository contains the configuration files for setting up a web application using Docker and NGINX.

## Docker Compose (docker-compose.yml)

The `docker-compose.yml` file defines a Docker service for running an NGINX web server. Here's what each section does:

```yaml
version: '3.9'

services:
  nginx:
    image: gustavoloppes/my-app-nginx:1.0
    ports:
      - '80:80'
    volumes:
      - . /projetos/site:/usr/share/nginx/html

