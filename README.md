# DevOps Real-time Project 🚀

## Workflow
1. Developer pushes code to GitHub.
2. Jenkins pipeline builds Docker image.
3. Image is pushed to DockerHub.
4. write  Ansible playbook.
5. Ansible deploys latest container on Web Server.

## Tech Stack
- AWS EC2 (Jenkins, Ansible, Web Server)
- GitHub (Source code)
- Jenkins (CI/CD)
- Docker & DockerHub (Image registry)
- Ansible (Deployment automation)

## Setup
1. Create 3 EC2 instances (Jenkins, Ansible, Web).
2. Install required tools.
3. Configure Jenkins with GitHub webhook.
4. Run pipeline → check your app at `http://<web-server-ip>`
