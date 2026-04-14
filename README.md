# NGINX-Docker-Static-Site

Containerized static website served using NGINX and Docker

### Overview

This project demonstrates how to serve a static website using NGINX inside a Docker container.

### Features

* Static HTML website
* NGINX web server
* Containerized using Docker

### Project Structure

```
.
├── Dockerfile
├── index.html
└── README.md
```

### How It Works

The NGINX server runs inside a Docker container and serves the static `index.html` file on port 80.

### Dockerfile Explanation

* Uses official NGINX image
* Copies static HTML file to NGINX default directory
* Exposes port 80 for web access

### How to Run

#### 1. Build Docker Image

```
docker build -t nginx-static-site .
```

#### 2. Run Container

```
docker run -p 8080:80 nginx-static-site
```

#### 3. Access Application

Open in browser:

```
http://localhost:8080
```

### Learning Outcomes

* Understanding Dockerfile basics
* Running containers using Docker
* Serving static content with NGINX
* Port mapping in Docker

### Output

The browser displays the static webpage served by NGINX.

### Future Improvements

* Add custom NGINX configuration
* Use Docker Compose
* Add reverse proxy setup
