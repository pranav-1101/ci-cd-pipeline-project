# CI/CD Pipeline Project

## Overview
This project demonstrates an end-to-end Continuous Integration and Continuous Deployment (CI/CD) pipeline using industry-standard DevOps tools.

The pipeline automates the process of:
- Building application code
- Creating Docker images
- Pushing images to a container registry
- Deploying the application automatically

---

## Tools & Technologies Used
- GitHub – Source code management
- Jenkins – CI/CD automation
- Docker – Containerization
- AWS – Cloud infrastructure

---

## Project Architecture
1. Developer pushes code to GitHub
2. Jenkins is triggered via webhook
3. Jenkins builds the application
4. Docker image is created using Dockerfile
5. Image is pushed to a container registry
6. Application is deployed automatically

---

## Repository Structure
ci-cd-pipeline-project
│── app/ # Application source code
│── docker/
│ └── Dockerfile # Docker image instructions
│── jenkins/ # Jenkins configuration files
│── docs/
│ └── architecture.md # Architecture explanation
│── Jenkinsfile # Jenkins pipeline definition
│── README.md


---

## CI/CD Pipeline Flow
- Code changes are pushed to the `main` branch
- Jenkins automatically detects the change
- Pipeline stages execute sequentially:
  - Build
  - Test
  - Docker Image Creation
  - Deployment

---

## Future Enhancements
- Add automated testing stage
- Integrate Kubernetes for deployment
- Add monitoring and logging
