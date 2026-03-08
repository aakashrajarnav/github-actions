# GitHub Actions Flask App

This repository contains a sample **Flask web application** containerized using Docker and built through a CI/CD pipeline powered by GitHub Actions.

## Features

- Dockerized Flask application
- Automated CI/CD pipeline using GitHub Actions
- Multi-architecture Docker images (linux/amd64, linux/arm64)
- Image published to Docker Hub
- Deployment using Docker Compose on a self-hosted runner

## Live Application

The application is currently deployed and accessible at:

http://13.233.140.55/

The container runs on **port 80**.

## Docker Image

Pull the latest image from Docker Hub:

docker pull aakashrajarnav/github-actions-app:latest

## Run the Container

Run the application locally using Docker:

docker run -p 80:80 aakashrajarnav/github-actions-app:latest

Then open in your browser:

http://localhost

## Supported Architectures

- linux/amd64
- linux/arm64

## CI/CD Pipeline

The project uses GitHub Actions to automatically:

1. Build the Docker image
2. Push the image to Docker Hub
3. Deploy the application using Docker Compose on a self-hosted runner