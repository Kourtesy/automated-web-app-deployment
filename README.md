# Automated Web App Deployment (Docker + GitHub Actions)

![Build Status](https://github.com/Kourtesy/automated-web-app-deployment/actions/workflows/deploy.yml/badge.svg)

A lightweight Python Flask web application containerized using Docker and continuously 
integrated using GitHub Actions.

## Features
- **Containerization**: Standardized Docker runtime environment.
- **Continuous Integration**: GitHub Actions workflow builds and smoke-tests the container image on every commit.

## Local Setup & Execution
1. Clone the repository:
   ```bash
   git clone https://github.com/Kourtesy/automated-web-app-deployment.git
   cd automated-web-app-deployment
   ```
2. Build the Docker image:
   ```bash
   docker build -t flask-app .
   ```
3. Run the container:
   ```bash
   docker run -p 5000:5000 flask-app
   ```
4. Access `http://localhost:5000` in your web browser.
