# docker-nginx
# https://hub.docker.com/r/katarzynadasilva/nginx-custom

# NGINX Custom Image

This repository contains a Dockerfile to build a custom NGINX image with a simple HTML page. The HTML page displays a multilingual greeting message.

## Usage

To use this custom NGINX image, follow these steps:

1. Build the Docker image:

    ```bash
    docker build -t katarzynadasilva/nginx-custom .
    ```

2. Run a container based on the custom image:

    ```bash
    docker run -p 8080:80 katarzynadasilva/nginx-custom
    ```

3. Open your web browser and navigate to [http://localhost:8080](http://localhost:8080) to view the greeting message.

## Dockerfile Description

### Base Image

- Uses the official NGINX image from Docker Hub (`nginx:latest`).

### Working Directory

- Sets the working directory inside the container to `/usr/share/nginx/html`.

### Copy HTML

- Copies the local `index.html` file to the container's working directory.

### Exposed Port

- Exposes port 80 to allow access to the NGINX web server.

### Labels

- Adds metadata labels to the image, including maintainer information, version, and a brief description.

## Maintainer

This NGINX custom image is maintained by katarzynadasilva.

