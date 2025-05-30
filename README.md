# Build a Sample Web App in a Docker Container

A simple Flask web application containerized using Docker, demonstrating basic web application deployment and containerization concepts.

## Project Overview

This project showcases how to:
- Create a basic Flask web application
- Containerize a web application using Docker
- Set up automated deployment using shell scripts
- Handle static files and templates in a Flask application

## Prerequisites

- Python 3.x
- Docker
- Flask (installed automatically in the container)

## Project Structure

```
labs/devnet-src/sample-app/
├── templates/           # HTML templates
├── static/             # Static files (CSS, JS, images)
├── sample_app.py       # Main Flask application
├── sample-app.sh       # Docker build and deployment script
└── user-input          # User input configuration
```

## Quick Start

1. Clone the repository:
```bash
git clone https://github.com/[your-username]/Build-a-Sample-Web-App-in-a-Docker-Container.git
cd Build-a-Sample-Web-App-in-a-Docker-Container
```

2. Navigate to the sample app directory:
```bash
cd labs/devnet-src/sample-app
```

3. Run the deployment script:
```bash
chmod +x sample-app.sh
./sample-app.sh
```

The script will:
- Create necessary directories
- Copy application files to a temporary directory
- Create a Dockerfile
- Build the Docker image
- Run the container on port 8080

## Accessing the Application

Once the container is running, you can access the web application at:
```
http://localhost:8080
```

## Docker Container Details

- The application runs on port 8080
- The container is named "samplerunning"
- The Docker image is tagged as "sampleapp"

## Managing the Container

To stop the container:
```bash
docker stop samplerunning
```

To remove the container:
```bash
docker rm samplerunning
```

To view container status:
```bash
docker ps -a
```

## Contributing

Feel free to fork this repository and submit pull requests to contribute to this project.


