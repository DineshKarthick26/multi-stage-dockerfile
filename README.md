# Flask Application Containerization using Docker

## Project Overview

This project demonstrates how to containerize a simple Flask web application using Docker and deploy it using Docker Compose.

The objective was to gain hands-on experience with Docker fundamentals, including image creation, container management, dependency handling, and service orchestration.

## Project Structure

```text
.
├── app.py
├── requirements.txt
├── Dockerfile
└── docker-compose.yml
```

## File Descriptions

### app.py

Contains the Flask application code and defines the web routes that are served to users.

### requirements.txt

Lists the Python dependencies required by the application. Docker uses this file to install the necessary packages during the image build process.

### Dockerfile

Defines the instructions required to build the Docker image:

* Uses a Python base image
* Sets the working directory
* Copies application files
* Installs dependencies
* Specifies the command to start the Flask application

### docker-compose.yml

Defines and manages the application service, making it easier to deploy and run the application using a single command.

## Build and Run

### Build the Docker Image

```bash
docker build -t flask-app .
```

### Run the Container

```bash
docker run -p 5000:5000 flask-app
```

### Run Using Docker Compose

```bash
docker compose up -d
```

## Learning Outcomes

Through this project, I learned:

* Docker image creation and management
* Writing Dockerfiles
* Container lifecycle management
* Port mapping
* Docker Compose fundamentals
* Managing application dependencies
* Troubleshooting container build and runtime errors

## Challenges Faced

During the implementation, I encountered and resolved several issues, including:

* Missing dependency files
* Docker build failures
* Container startup errors
* Docker Compose configuration issues
* Port mapping and accessibility troubleshooting

These debugging exercises helped strengthen my understanding of Docker beyond the basic commands.

## Future Enhancements

* Add Nginx as a reverse proxy
* Implement CI/CD using GitHub Actions
* Deploy to a cloud environment
* Add monitoring and logging

