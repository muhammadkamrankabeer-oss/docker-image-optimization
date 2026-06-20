![CI/CD Status](PASTE_BADGE_LINK_HERE)
## 🔄 CI/CD Pipeline

#🌱 EcoDocker — Reducing Carbon Footprint with Lightweight Containers 

![CI/CD](https://github.com/muhammadkamrankabeer-oss/docker-image-optimization/actions/workflows/deploy.yml/badge.svg)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Alpine](https://img.shields.io/badge/Alpine-Optimized-0D597F?logo=alpinelinux&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A DevOps experiment demonstrating how Docker image optimization reduces resource usage, speeds up deployments, and supports more sustainable infrastructure practices.

## 🚀 Overview

EcoDocker compares a standard vs. an optimized Docker image for the same Flask application, showing how choosing the right base image (e.g. Alpine Linux) can drastically cut:

- Image size
- Bandwidth usage
- Storage cost
- Indirect energy consumption

## 🎯 Problem Statement

Modern containerized applications often ship with heavy base images, leading to:

- Large Docker image sizes
- Slower deployments
- Higher cloud storage and bandwidth usage
- Unnecessary resource consumption at scale

## 💡 Solution

This project compares two approaches:

**🟥 Standard Docker Image**
- Based on `python:3.10`
- Larger footprint (~1.6 GB)

**🟩 Optimized Docker Image**
- Based on `python:3.10-alpine`
- Lightweight (~97 MB)
- Minimal dependencies

## 🧱 Architecture

```
Flask App
   │
   ├── Docker (Standard Image)
   └── Docker (Alpine Optimized Image)
```

## 📦 Tech Stack

- Python 3.10
- Flask
- Docker
- Alpine Linux
- DevOps principles

## 📊 Results

| Image Type     | Size     |
|-----------------|----------|
| Standard Image  | ~1.6 GB  |
| Alpine Image    | ~97 MB   |

👉 **~16x reduction in size**

## 🌍 Why This Matters

Optimizing container size helps:

- Reduce cloud infrastructure load
- Improve CI/CD performance
- Save storage and bandwidth
- Contribute to greener software engineering practices

## 🚀 How to Run

**1. Clone repo**
```bash
git clone https://github.com/muhammadkamrankabeer-oss/docker-image-optimization.git
cd docker-image-optimization
```

**2. Build images**
```bash
docker build -f docker/Dockerfile.normal -t eco-normal .
docker build -f docker/Dockerfile.alpine -t eco-alpine .
```

**3. Run container**
```bash
docker run -p 5000:5000 eco-alpine
```

## 📸 Demo

Flask app runs at: `http://localhost:5000` — shows the eco-friendly container demo.

## 🔄 CI/CD Pipeline

This project includes an automated CI/CD pipeline using GitHub Actions (`deploy.yml`):

- Code pushed to repository
- Docker image builds automatically
- Container is tested in the CI environment

**Benefits:** no manual deployment, faster and more consistent builds, fewer human errors.

## 🧠 Key Learnings

- Docker base image choice directly impacts performance and size
- Alpine Linux is a powerful tool for optimization
- Small DevOps changes can have a big infrastructure impact
- Real-world sustainability starts at the engineering level

## 🔮 Future Improvements

- Add Kubernetes deployment manifests
- Add automated image benchmarking
- Add CO₂ estimation metrics

## 👨‍💻 Author

**Muhammad Kamran Kabeer**
Focus: DevOps | Linux | Cloud | Automation

- Dev.to article: [Reducing Carbon Footprint with Lightweight Docker Containers](https://dev.to/muhammadkamrankabeeross/reducing-carbon-footprint-with-lightweight-docker-containers-a-devops-experiment-on-image-2068)
- GitHub: [@muhammadkamrankabeer-oss](https://github.com/muhammadkamrankabeer-oss)
