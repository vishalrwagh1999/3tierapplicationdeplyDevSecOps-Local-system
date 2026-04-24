# 3-Tier Application Deployment with DevSecOps



## Table of Contents
1. [Project Overview](#project-overview)
2. [DevSecOps Architecture](#devsecops-architecture)
3. [Pre-Requisites](#pre-requisites)
4. [Environment Setup](#environment-setup)
5. [Security & Analysis Tools](#security--analysis-tools)
6. [CI/CD Pipeline Integration](#cicd-pipeline-integration)
7. [Database Layer](#database-layer)
8. [Troubleshooting & Debugging](#troubleshooting--debugging)

---

# Project Overview

## Introduction
This project demonstrates a robust **DevSecOps** implementation for a 3-tier monolithic architecture. By integrating security at every stage of the lifecycle—from initial environment setup to container image scanning—we ensure that the application is not only functional but also secure and production-ready.

### Key Features
- **Automated Infrastructure**: Shell scripts for rapid environment provisioning.
- **Vulnerability Management**: Automated container scanning using **Trivy**.
- **Static Analysis**: Real-time code quality checks via **SonarQube**.
- **Container Orchestration**: Standardized Docker environment for application tiers.

---

# DevSecOps Architecture



The workflow follows a "Shift-Left" security approach:
1. **Code**: Developers commit code to the repository.
2. **Scan**: Source code is analyzed by SonarQube for bugs and vulnerabilities.
3. **Build**: Docker images are created for the Web, App, and DB tiers.
4. **Secure**: Trivy scans the Docker images for OS-level CVEs before deployment.

---

# Pre-Requisites

### 1. System Requirements
- Linux-based environment (Ubuntu recommended).
- Minimum 4GB RAM to run SonarQube and Jenkins concurrently.

### 2. Tools & Access
- **Docker**: Container runtime.
- **Trivy**: Security scanner.
- **Jenkins**: CI/CD automation server.
- **Docker Hub Account**: For image registry management.

---

# Environment Setup

### 1. Script Permissions
Ensure all automation scripts have the necessary execution rights:
```bash
chmod 755 *.sh
ls -ltrh
