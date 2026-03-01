# CI/CD Pipeline Project

A complete CI/CD pipeline implementation with Docker containerization, AWS CodeBuild, automated backups, and monitoring scripts.

## Features

- Dockerized application deployment
- AWS CodeBuild integration with buildspec.yml
- Automated backup scripts
- System monitoring with cron jobs
- Infrastructure automation

## Tech Stack

- **Containerization:** Docker
- **CI/CD:** AWS CodeBuild
- **Scripting:** Python, Bash
- **Scheduling:** Cron

## Project Structure

```
CICDproject/
├── Dockerfile          # Container definition
├── buildspec.yml       # AWS CodeBuild specification
├── backup_script.py    # Automated backup script
├── monitor_script.py   # System monitoring
└── mycron              # Cron job definitions
```

## Getting Started

### Build Docker Image
```bash
docker build -t cicd-project .
docker run -p 8080:8080 cicd-project
```

### AWS CodeBuild
Configure CodeBuild to use the `buildspec.yml` for automated builds and deployments.
