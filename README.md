# Flask Demo CI/CD Pipeline

This project demonstrates a complete CI/CD pipeline for a containerized Flask application using:
- Git-based workflows
- Automated builds with GitHub Actions
- Docker image publishing to Docker Hub
- Kubernetes deployment using Helm


## Architecture
1. Code is pushed to GitHub
2. GitHub Actions builds Docker image
3. Image is pushed to Docker Hub
4. Kubernetes pulls and deploys the image


## Tech Stack
- Python (Flask)
- Docker
- GitHub Actions
- Kubernetes
- Helm


## Project Structure

./
└── ci-cd-kubernetes-pipeline/
    ├── CHANGELOG.md
    ├── Dockerfile
    ├── README.md
    ├── app.py
    ├── .github/
    │   └── workflows/
    │       └── pipeline.yml
    ├── helm/
    │   └── flask-demo/
    │       ├── Chart.yaml
    │       ├── templates/
    │       │   ├── deployment.yaml
    │       │   └── service.yaml
    │       └── values.yaml
    ├── kubernetes/
    │   ├── deployment.yaml
    │   └── service.yaml
    ├── requirements.txt
    └── test_app.py

