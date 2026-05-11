# CSC424 Final Exam

## DevOps Setup

```bash
docker-compose up --build -d
```

Port:
Only Nginx exposes port 80 to the host.

Test URLs:
```bash
http://localhost
```
React frontend

```bash
http://localhost/api/ping
```
{"status":"ok","message":"pong"}




## CI/CD Pipeline
On every push to main:

Builds Docker images

Pushes to Docker Hub

Deploys to QA server via self-hosted runner


## Repository Structure
<img width="353" height="212" alt="image" src="https://github.com/user-attachments/assets/6403bef9-d4ec-4dc0-a5ac-c041554dae05" />

## Author
Hualin
