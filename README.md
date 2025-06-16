# Project: Docker Apache Web Server

## Overview
This project sets up a simple **Apache HTTP Server** inside a **Docker container** using **Docker Compose**. It serves a static website stored in a local `html/` directory.

## Features
- **Apache (httpd) Server** running inside Docker.
- **Docker Compose** for easy management.
- **Volume Mounting** to serve local HTML content.
- **Bridge Network** for flexible container communication.

## Getting Started

### 1. **Clone the Repository**
```bash
git clone git@github.com:rafaelnogueiradev/dio-docker-project.git

cd dio-docker-project
```

### 2. **Structure**
```
dio-docker-project/
│-- html/
    │-- index.html
    │-- style.css
|-- compose.yaml
|-- LICENSE
|-- README.md
```

### 3. **Run the Server**
Execute the following command:
```bash
docker compose up -d
```

### 4. **Stopping the Server**
To stop and remove the containers:

```bash
docker compose down
```

## **Customization**
You can update **HTML**, **CSS** files inside the ``html/`` folder to modify the website. Changes will reflect immediately after restarting the container.

## Troubleshooting
Check logs if Apache isn't running correctly:
```bash
docker logs apache_server
```
Ensure the html/ folder exists and has correct permissions.

## License
This project is open-source and can be modified or extended as needed.
